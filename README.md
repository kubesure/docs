# kubesure = *kube*netes + sure 

Why Kubesure?? For the lack of a better name and for the love of kubernetes. Project name will change until a cool sanskrit, greek or a latin name is christened. 

Kubesure intents to build a _insuretech_ pay as you insurance product. Also, a stable Kubesure will be contributed to Kubernetes community as a real world example for learning. Pls join and spread knowledge. 


**0.1 features**  

1. create new business apis'for to buy esyhealth (stp) and esytravel (stp) product 
    - [x] premium - Go + Redis - Rest/Json
    - [x] quote - Node + Mongo  - Rest/Json
    - [x] party - Go + Mongo - GRPC  
    - [x] receipt - Go + Mongo - Rest/Json
    - [x] policy - Go + Mysql - Rest/Json
    - [] Generate policy PDF - Async Kakfa on policy issue
    - Send communication on SMS and Email (pdf) Async Kafka on policy issue
2. Deploy apis in kubernetes 
    - [x]Basic deployment no ingress other than kubernetes service
3. Review 
    - [x] Enchance model for richness in biz and refactor
    - [x] fix issues 
    - [x] Refactor repeat until all test pass 
4. Document architecture, design and code
5. Create build script for all go services
6. Update install and release notes 

**0.2 features** 
 
[] Create UI with micro web deployment  
[] Logging with fluentd and elastic 
[] Pull events to Kakfa for data analysis biz moments is TBD
[X] API Exposure to world through Kube ingress 
[] Fix defects

**0.3 Features** 

[] Deploy on kubernetes with a service mesh  
[] Prepare helm charts
[] CI CD Pipeline


**0.4 Features**

1. Throw Enhance and Grow???
