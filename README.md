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
   Create a kubernetes cluster in linode<br/>
   change permission on kubeconfig.yaml file<br/>
   connect to the cluster<br/>
   
  
  
  

   <h2>step3</h2>
 
  Create Deployment and Service for all microServices in the created cluster
   <img src='./cam/m3.png' height="80%" width="80%" alt="Disk Sanitization Steps">
   

 <h2>step4</h2>
 All pod are running and application can be accessed in the browser using the node IP and <br/>
 configured external service IP with the frontend service<br/>
 <img src='./cam/m2.png' height="80%" width="80%" alt="Disk Sanitization Steps">
     

</p>
