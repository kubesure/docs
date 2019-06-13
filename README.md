# kubesure = *kube*netes + sure 

Why Kubesure?? For the lack of a better name and for the love of kubernetes. Project name will change until a cool sanskrit, greek or a latin name is christened. 

Kubesure intents to build a _insuretech_ pay as you go insurance products. Also, a stable Kubesure will be contributed to Kubernetes community as a real world example for learning. Pls join innovate and spread knowledge. 

Features 0.1 to 0.3 sets the basic platform for Pay As You Model.

**0.1 features** https://github.com/kubesure/helm-charts/releases/tag/v0.1 

1. Create new business apis' for to buy esyhealth (stp) and esytravel (stp) products - 
   - [x] premium - Go + Redis - Rest/Json
   - [x] quote - Go + Mongo  - Rest/Json
   - [x] party - Go + Mongo - GRPC  
   - [x] receipt - Go + Mongo - Rest/Json
   - [x] policy - Go + Mysql - Rest/Json
2. Deploy apis in kubernetes 
    - [x] Basic deployment no ingress other than kubernetes service
3. Review 
    - [x] Enchance model for richness in biz and refactor
    - [x] fix issues 
    - [x] Refactor repeat until all test pass 
5. Helm charts
7. Update release

**0.2 features** 

1. Product features
   - [ ] Gen Poilcy document on policy issue event
   - [ ] Send communication SMS and Email (pdf) on policy issue 
2. Log visibility
   - [X] Cluster level logging with fluentd and elasticsearch 
3. Pull biz events to Kakfa via Kafka Connect for data analysis. Biz moments is TBD
4. North-South API traffic 
   - [X] k8s Ingress
   - [X] Ambassodor API gateway 
   - [ ] Rate limits 
   - [ ] Secure internet exposed API's
   - [ ] API authentication via API gateway
5. Makefile  
   - [X] Premium 
   - [X] Quote
   - [x] Party
   - [x] Receipt
   - [x] Policy      
6. CI CD Pipeline
7. Document 
   - [ ] Architecture 
   - [ ] Code

**0.3 Features** 

1. West-East traffic on a service mesh
2. Mobile app
   - [ ] Buy journey 
   - [ ] Click Stream capture   
  
**0.4 Features**

1. Pay As You Go model generation.

