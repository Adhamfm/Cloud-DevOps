# What Files create what Stacks
* **final-project.yml** creates the **Servers stack** 
* **ourinfra.yml** creats the **Infrastructure stack**

## Project Diagram
![alt text](https://github.com/Adhamfm/Cloud-DevOps/blob/main/FinalProject.jpeg "Project Diagram")

ourinfra.yml creates:
1. 1 VPC with 2 public subnets and 2 private subnets deployed in 2 different AZs 
2. Internet gateway
3. Nat Gatway in each public subnet to provide internet connectivity to the private subnets

final-project.yml creates:
1. Launch Configuration  
2. Autoscaling group that deploys the instances inside private subnets
3. Load Balancer 
4. Security Groups for the Load Balancer and the Servers

# Images showing the working Stacks
## The Following Images shows the created stacks from final-project.yml
![alt text](https://github.com/Adhamfm/Cloud-DevOps/blob/main/resources1.png "Servers Resources 1")

![alt text](https://github.com/Adhamfm/Cloud-DevOps/blob/main/resources2.png "Servers Resources 2")
## Shows that the Loadbalancer can reach the servers using the URL
![alt text](https://github.com/Adhamfm/Cloud-DevOps/blob/main/output.png "Servers Output showing LoadBalancer URL")

![alt text](https://github.com/Adhamfm/Cloud-DevOps/blob/main/workingTest.png "LoadBalancer Response ")

Thanks for your time!
Adham
