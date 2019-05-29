# kubesure = *kube*netes + sure 

Why Kubesure?? For the lack of a better name and for the love of kubernetes. Project name will change until a cool sanskrit, greek or a latin name is christened. 

Kubesure intents to build a _insuretech_ pay as you go insurance products. Also, a stable Kubesure will be contributed to Kubernetes community as a real world example for learning. Pls join innovate and spread knowledge. 

Features 0.1 to 0.4 sets the basic platform for Pay As You Model.

**0.1 features**  

1. Create new business apis' for to buy esyhealth (stp) and esytravel (stp) products - 
   - [x] premium - Go + Redis - Rest/Json
   - [x] quote - Go + Mongo  - Rest/Json
   - [x] party - Go + Mongo - GRPC  
   - [x] receipt - Go + Mongo - Rest/Json
   - [x] policy - Go + Mysql - Rest/Json
   - [ ] Gen Poilcy document - Kakfa Msg on policy issue
   - [ ] Send communication SMS and Email (pdf) Kafka Msg on policy issue
2. Deploy apis in kubernetes 
    - [x] Basic deployment no ingress other than kubernetes service
3. Review 
    - [x] Enchance model for richness in biz and refactor
    - [x] fix issues 
    - [x] Refactor repeat until all test pass 
4. Document 
   - [ ] Architecture 
   - [ ] Code
5. Create makefile script for all services
6. Update release

**0.2 features** 
 
1. Create UI with micro web deployment  
2. Log visibility with fluentd and elastic 
3. Pull biz events to Kakfa via Kafka Connect for data analysis. Biz moments is TBD
4. North-South API traffic to world through Kube ingress
5. Helm charts
6. CI CD Pipeline

**0.3 Features** 

1. West-East traffic on a service mesh  

**0.4 Features**

1. Pay As You Go model generation.
