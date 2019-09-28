Features 0.1 to 0.3 sets the basic platform for Pay As You Model.

**0.1 features** https://github.com/kubesure/helm-charts/releases/tag/v0.1-aplha

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
5. - [x] Helm charts
7. - [x] Update release

**0.2 features** https://github.com/kubesure/helm-charts/releases/tag/v0.2-aplha

1. Product features
   - [X] Gen Poilcy document on policy issue event
   - [X] Send communication SMS and Email (pdf) on policy issue 
2. Log visibility
   - [X] Cluster level logging with fluentd and elasticsearch 
4. North-South API traffic 
   - [X] k8s Ingress
   - [X] Ambassodor API gateway
   - [X] Secure internet exposed API's
   - [ ] API authentication via API gateway
5. West-East traffic on a service mesh - Linkered 2
   - [X] Premium 
   - [X] Quote
   - [X] Party
6. Makefile  
   - [X] Premium 
   - [X] Quote
   - [x] Party
   - [x] Receipt
   - [x] Policy
   - [X] Comms
   - [X] Publisher 
8. CI CD Pipeline 
   - [X] Premium
7. Document 
   - [X] Architecture 
   - [X] Code

**0.3 Features** 

1. North-South API traffic - Istio service mesh
   - [ ] Rate limits 
   - [ ] Secure internet exposed API's
   - [ ] API authentication via API gateway
2. West-East traffic - Istio service mesh
   - [ ] Inter servcie security 
   - [ ] Loadbalancing
   - [ ] 
3. Mesh Visibility - Istio   
4. Mobile app
   - [ ] Buy journey 
   - [ ] Click Stream capture
5. CI CD Pipeline 
   - [ ] Pre-Prod
   - [ ] Prod
6. Setup Environment
   - [ ] Pre-Prod
   - [ ] Prod
  
**0.4 Features**

1. Pay As You Go model generation.
