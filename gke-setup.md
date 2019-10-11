# kubesure pre-prod setup - GKE

## Create and configure pre-prod cluster

gcloud container clusters create kubesure-prepod

gcloud config set container/cluster kubesure-prepod

gcloud container clusters get-credentials kubesure-prepod --region YOURREGION --project YOURPROJECT

gcloud container clusters resize kubesure-prepod --size=3 --region YOURREGION --project YOURPROJECT

kubectl create clusterrolebinding YOURNAME-cluster-admin-binding --clusterrole=cluster-admin --user=YOUREMAIL@gmail.com

## Install Helm 

1. Install Helm CLI
2. kubectl -n kube-system create serviceaccount tiller
3. kubectl create clusterrolebinding tiller --clusterrole cluster-admin --serviceaccount=kube-system:tiller
4. helm init --service-account tiller 
  
## Install Ambassador chart

https://github.com/kubesure/helm-charts/tree/master/ambassador
  
## install argocd server 

kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

### install argocd cli

curl -sSL -o /usr/local/bin/argocd https://github.com/argoproj/argo-cd/releases/download/v1.2.3/argocd-linux-amd64
chmod +x /usr/local/bin/argocd

### Get argocd admin password
kubectl get pods -n argocd -l app.kubernetes.io/name=argocd-server -o name | cut -d'/' -f 2

### Proxy to API Server
kubectl port-forward svc/argocd-server -n argocd 8080:80

### Login as admin 
argocd login localhost:8080

### Install kubesure argocd apps

argocd app create premium \
  --repo https://github.com/kubesure/helm-charts.git \
  --path premium \
  --dest-server https://kubernetes.default.svc \
  --dest-namespace default \
  --revision preprod \

argocd app sync premium

argocd app create quote \
  --repo https://github.com/kubesure/helm-charts.git \
  --path quote \
  --dest-server https://kubernetes.default.svc \
  --dest-namespace default \
  --revision preprod

argocd app sync quote

argocd app create party \
  --repo https://github.com/kubesure/helm-charts.git \
  --path party \
  --dest-server https://kubernetes.default.svc \
  --dest-namespace default \
  --revision preprod     

argocd app sync party