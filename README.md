# kubesure = *kube*netes + sure 

Why Kubesure?? For the lack of a better name and for the love of kubernetes. Project name will change until a cool sanskrit, greek or a latin name is christened. 

Kubesure intents to build a _insuretech_ platform.

**0.1 features**  

1. create new business apis'for to buy esyhealth (stp) and esytravel (stp) product 
    - premium - Go + Redis - Rest/Json
    - quote - Node + Mongo  - Rest/Json
    - party - Go + Mongo - GRPC  
    - receipt - Go + Mongo - ??
    - policy - Go + Mysql - ??    
    - Generate policy PDF - Async Kakfa on policy issue
    - Send communication on SMS and Email (pdf) Async Kafka on policy issue
2. Deploy apis in kubernetes 
    - Basic deployment no ingress other than kubernetes service
3. Review 
    - Enchance model for richness in biz and refactor
    - fix issues 
    - Refactor repeat until all test pass 
4. Document architecture, design and code
5. Create build script for all go services
6. Update install and release notes 

**0.2 features** 
 
1. Create UI with micro web deployment  
2. Logging with fluentd and elastic 
3. Post events to Kakfa for data analysis biz moments is TBD
4. Kube ingress 
5. Fix defects

**0.3 Features** 

1. Deploy on kubernetes with a service mesh  
2. Prepare helm charts
3. CI CD Pipeline
4. API Exposure to world

**0.4 Features**

1. Throw Enhance and Grow???
