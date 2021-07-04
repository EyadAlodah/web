# Write-up for CMS system 

### Solution and resource analysis.

*We are going to use App services for our CMS for these reasons:*
- *App services will provide us with High availability and vertical scalability for our small application.* 
- *App services will help us to start quickly and deploy our app faster, and this what we need in a new web app.* 
- *Our CMS currently is a lightweight and does not contains to many proceeses and requests and it can be satisfied by App services*
- *Choosing App services will help us to save cost, becuase VM are more expensive*

*The following tables shows the differences in cost between App services and VM for basic, standard and premium Tiers*

*App Services:*
	
|  Tier         |  instance     | Cores        | RAM          | OS            | Storage       | Monthly     |
| ------------- | ------------- | ------------ | ------------ | ------------  |  ------------ |------------ |
| Basic         | B2            | 2 cores      | 3.5 GB RAM   |  Linux        | 10 GB Storage | $26.28      |
| Standard      | S2            | 2 cores      | 3.5 GB RAM   |  Linux        | 50 GB Storage | $138.70     |
| Premium V2    | P2V2          | 2 cores      | 7 GB RAM     |  Linux        | 250 GB Storage| $168.63     |



*Virtual Machine:*
	
|  Tier         |  instance     | Cores        | RAM          | OS            | Storage       | Monthly     |
| ------------- | ------------- | ------------ | ------------ | ------------  |  ------------ |------------ |
| Basic         | A2            | 2 cores      | 3.5 GB RAM   |  Linux        | 60 GB Storage | $59.13     |
| Standard      | A3            | 4 cores      | 7 GB RAM     |  Linux        | 185 GB Storage| $175.20     |


*Based in the table the cost of the two depends in the tier and instances that we are going to use*
*Prices represents only one instance can increase as instances added*
*Storage sizes options are more in VM*

*The following tables shows the differences in Scalability between the two solutions*

|  Criteria     |                       VM            | App Service          | 
|-------------  | ----------------------------------- | -------------        |
| Autoscaling   | Virtual machine scale sets          | Built-in service     | 
| Load balancer | uses azure load balancer            | integrated load balancer |
| limit         | for the platform image it has 1000 nodes per scale set and for the custom image it has 600 nodes per scale set | 30 instances  |



### App changes in future.

*However, In future our app could get bigger and we might need to use and develop more services to enhance our CMS website.* 
*So we could change our cloud computing plan to VM to meet our needs and satisfy the different requierments of our CMS system such as more CPU, RAM and storage*  
