- In this repository we have sample application code and dockerfile for 3 micro-services to get you started for excersice is  CI/CD pipeline.
- **Each micro-services build should be seprated from other** 

- Pipeline phases
  - Preview Build/Deploy
    - Create pipline for preview builds where individual developer can test their application in isolated environment, this kind of feature is usefull demonstrating unit testing.
    - For this developer is going to create seprate branch out of staging branch for each feature.
    
  - Stageing Build/Deploy :
    - In this phase code changes done by individual developers will be merged and deployed, and micro-service will be deployed in GKE cluster.
    - This phase is primarly used for performing intigration testing.
  
  - Production Build/Deploy :
    - In this phase the application will be deployed to production cluster.
    - As this is live environment, key requirenment for this phase id zero-down time deployments. 

- Primary phases for deploying application
  - Image build 
  - Push image
  - Deploy image
