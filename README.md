<h1>Kubernetes Demo Project5</h1>
<h2>Technologies used</h2>

- <b>Kubernetes</b> 
- <b>Redis</b>
- <b>Linux</b>
- <b>Linode LKE</b>



<h2>Detailed Description of Project </h2>
1. Create K8s minifests for Deployments and Services for all microservices of an online shop application <br/>
2. Deploy microservices to linode managed kubernetes cluster<br/>


   <p align="">
   <h2>step1</h2>
   Key information before deploying microservice application<br/>
   1. How the services are connected<br/>
   2. If the application requires any third party service eg databases<br/>
   3. Which Service is accessible from outside the cluster<br/>
   4. The image name for each microservice<br/>
   5. Environment vaiable required for each microservice<br/>
   6. Ports on which each microservice starts<br/>
   7. Namespace in which microservice is deployed<br/>

   From the above information, a connection graph is generated 
   <img src='./cam/m1.png' height="80%" width="80%" alt="Disk Sanitization Steps">



   <h2>step2</h2>
   Create Deployment and Service for all microServices 
   <img src='./kam/im5.png' height="80%" width="80%" alt="Disk Sanitization Steps">
  

   <h2>step3</h2>
   Create a secret for kubernetes cluster with the secret token<br/>
   copy the content of the the (.docker/config.json) file in minikube to the host (.docker/config.json) dir<br/>
   minikube cp minikube:/home/docker/.docker/config.json ~/.docker/config.json<br/>

   create a secret with the access token in base64 encoded<br/>
   <img src='./kam/im6.png' height="80%" width="80%" alt="Disk Sanitization Steps">
   

 <h2>step4</h2>
 Create a deployment for the application to pull the image from the registry using the secret created in minikube<br/>
 <img src='./kam/im7.png' height="80%" width="80%" alt="Disk Sanitization Steps">

 Deployment is created <br/>
 <img src='./kam/im8.png' height="80%" width="80%" alt="Disk Sanitization Steps">

  pod is running in minikube<br/>
 <img src='./kam/im9.png' height="80%" width="80%" alt="Disk Sanitization Steps">



  
 

   
    
    
   
     

</p>
