
# Database
Amazon DynamoDB is a fully managed NoSQL database service offered by AWS (Amazon Web Services). It is designed to provide high performance (fast read/write operations), scalability, and reliability for applications that need to handle a lot of data and traffic with low latency.


### Key Features of DynamoDB:

1. NoSQL Database:
 Stores data in a flexible, non-relational format (key-value or document-based).

2. Fully Managed: 
AWS handles server maintenance, scaling, replication, backups, and security.

3. High Availability and Durability: 
Data is automatically replicated across multiple availability zones.

4. Auto-Scaling: 
It can automatically scale up or down based on traffic without manual intervention.

5. Serverless: 
No servers to manage — you focus only on using the database.

6. Fast and Predictable Performance: 
Single-digit millisecond response times.

7. Fine-Grained Access Control: 
Integrated with AWS IAM (Identity and Access Management).

8. Built-in Security: 
Encryption at rest and in transit.

### Main Uses of DynamoDB:

1. Real-Time Applications:
Like chat apps, gaming leaderboards, or live-stream analytics.

2. E-Commerce: 
Product catalogs, shopping carts, order tracking systems.

3. IoT Applications: 
Handling sensor data and device communication.

4. Mobile and Web Apps: 
For managing user profiles, sessions, and preferences.

5. Content Management Systems: 
Blogs, news articles, media metadata.

6. Financial Services: 
Fraud detection systems that require rapid data access and updates.

7. Gaming: 
Storing player profiles, scores, and game state. 


Practicale on aws 

create a dynamodb database

step1: create  table 
       table name as dynamodb1
       partition key as uid 
       default setting 
       create table 
step2: GO TO Tables and select table 
       explore table items 
       create item name String
       create item course redhat
step3: scan or query items
       goto scan select table and add attribute can select multiple attributes 
       gives compleate data 
step4 run query that finds perticular attribute data 
       run the query 
       
