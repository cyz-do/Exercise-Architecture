# Modeule 4 - Solution Architecting

![Module4-SolutionArchitecting](https://github.com/cyz-do/Exercise-Architecture/blob/main/Module4-SolutionArchitecting.jpg)

### 1. Amazon Route 53
Amazon Route 53 routes end-user requests resolving Domain Name Service (DNS).

### 2. AWS Web Application Firewall
AWS Web Application Firewall integration with Application Load Balancer to mitigate OWASP top 10 application vulnerabilities.

### 3. Application Load Balancer
The Application Load Balancer routes HTTP/S requests to EC2 instances running on private subnets act as the seventh layer of the OSI model. Receives a request, evaluating the listener rules such as SSL/TLS certificates stores in AWS Certificate Manager.

### 4. Nginx Reverse Proxy Server
Providing an additional level of abstraction and control to ensure the smooth flow of network traffic between users and to the web application servers.

### 5. Network Load Balancer
The Network Load Balancer opens a TCP connection to the selected target on the port specified in the listener configuration and routes the traffic evenly to the target group. It functions at the fourth layer of the OSI model.

### 6. React & NodeJS application servers
The application server stores and runs both the React (frontend) and NodeJS (backend) configs. 

### 7. Auto Scaling Group
Amazon EC2 Auto Scaling helps to ensure that there are correct number of servers available to handle the load for the React & NodeJS application.

### 8. Amazon RDS for PostgreSQL
Multi-AZ enables high-availability. Application connects via DNS endpoint that handles failover automatically in case of failure.

### AWS Secret Manager
Database credentials are securely stored on AWS Secrets Manager.

### AWS CloudWatch Logs and Metrics
Logs and monitors Route 53, WAF, EC2 servers, load balancers and RDS, using alarms to alert when are anomaly detected.

### Database Bastion Server
Providing access to the PostgreSQL database, and also actting as a recovery server to access both proxy and application servers.

### AWS Backup
Automate the back up of data across AWS services (disaster recovery)

### Infrastructure-as-code
Using Terraform infrastructure as code tool enables safe and predictable provision and management of infrastructure

### Git 
