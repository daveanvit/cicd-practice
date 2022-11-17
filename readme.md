#Assignment Details
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

Referance links:-
- https://blog.searce.com/micro-service-specific-build-in-monorepo-google-cloud-build-3c1be8edf4c
- https://cloud.google.com/run/docs/tutorials/configure-deployment-previews
- https://cloud.google.com/architecture/accessing-private-gke-clusters-with-cloud-build-private-pools
- https://cloud.google.com/build/docs/overview
