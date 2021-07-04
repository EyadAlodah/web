# Write-up for CMS system 

### Solution and resource analysis.

*We are going to use App services for our CMS for these reasons:*
- *App services will provide us with High availability and vertical scalability for our small application.* 
- *App services will help us to start quickly and deploy our app faster, and this what we need in a new web app.* 
- *Our CMS currently is a lightweight and does not contains to many proceeses and requests and it can be satisfied by App services*
- *Choosing App services will help us to save cost, becuase VM are more expensive*

*The following tables shows the differences in cost between App services and VM for basic, standard and premium Tiers*

*App Services:*
	
|  Tier         |  instance     | Cores        | RAM          | Storage       | Monthly     |
| ------------- | ------------- | ------------ | ------------ | ------------  | ------------|
| Basic         | B2            | 2 cores      | 3.5 GB RAM   | 10 GB Storage | $26.28      |
| Standard      | S2            | 2 cores      | 3.5 GB RAM   | 50 GB Storage | $138.70     |
| Premium V2    | P2V2          | 2 cores      | 7 GB RAM     | 250 GB Storage| $168.63     |



### App changes in future.

*However, In future our app could get bigger and we might need to use and develop more services to enhance our CMS website.* 
*So we could change our cloud computing plan to VM to meet our needs and satisfy the different requierments of our CMS system such as more CPU, RAM and storage*  
