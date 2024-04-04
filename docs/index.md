# Trusted Application Pipeline Software Template

This application, **dotnet-0404-master**, was created from a Trusted Application Pipeline Software Template.

The software templates create a new source and gitops deployment repositories with a sample source application. 

## Repositories

The source code for your application can be found in [https://github.com/stephanie-cy/dotnet-0404-master ](https://github.com/stephanie-cy/dotnet-0404-master ).
 
The gitops repository, which contains the kubernetes manifests for the application can be found in 
[https://github.com/stephanie-cy/dotnet-0404-master-gitops ](https://github.com/stephanie-cy/dotnet-0404-master-gitops ) 

## Application namespaces 

The default application will be found in the following namespaces. Applications can be deployed into unique namespaces or multiple software templates can also bet generated into the same group namespaces.  

|  Namespace   |  Description   |  
| -------- | -------- |   
| **rhtap-app-development** | The default application during development. Every build will be deployed to this namespace for testing. | 
| **rhtap-app-stage** | The staging namespace for this application. Promotion from development to stage is manual via an update to the [gitops repository](https://github.com/stephanie-cy/dotnet-0404-master-gitops ) in the components/dotnet-0404-master/overlays/prod directory |  
| **rhtap-app-prod** | The production namespace for this application. Promotion from stage to production is manual via an update to the [gitops repository](https://github.com/stephanie-cy/dotnet-0404-master-gitops ) in the components/dotnet-0404-master/overlays/prod directory | 