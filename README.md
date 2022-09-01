# Microservices-application-on-k3s
This is a microservices application build for practice kubernetes microservices deployment using microservices architecture.
The application converted into image and store into google container registry.

"confi.yml" file contains the deployment and service manifest file by using them we can deploy the microservices application.


 # Deployment process
 
 This application is deployed in civo cloud using k3s 
  
 create a k3s cluster in civo cloud and download the kubeconfig file ( I used lens to manage kubernetes cluster ) connect lens to k3s cluster using lens application
 deploy using confi.yml file using command 
    
    
    kubectl apply -f confi.yml
    
    
after use command to check all pods up and running.


   
    kubectl get pods
    
next connect to the cluster from internet by using this command port number of frontend microservices 


     kubectl get svc -n microservices
     
now using cluster ip address from civo and port number check the application has access from internet.    
     
    
    
    
   
   
   
   
