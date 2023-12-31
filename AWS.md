# What is a cloud?
Cloud is a shareable server over the internet.

# What is cloud computing?
Use of remote servers over the cloud to store, manage and process data rather than a local
server or personal computer.

# Advantages of Cloud Computing:
- on demand availibility
- on demand delivery
- advanced security
- access resources instantly
- almost no hardware requirements
- pay as you go model
- provision only the size you need
- higher performance

# Disadvantages of Cloud Computing:
- limited control
- service dependant
- migration challenges
- vendor lock-in
- cloud expertise
- unforeseen costs

# Public Cloud
- A cloud computing environment where infrastructure is shared by multiple organisations
- Companies like Amazon, Microsoft and Google provide public cloud services

# Private Cloud
- A cloud computing environment dedicated to a single organization
- Softwares like OpenStack and OpenNebula provide private cloud

# Public vs Private Cloud
![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/654e8105-5ed4-4cd4-9f14-5c936b8523e4)


![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/b6d7f31b-f497-4251-ad90-643a1cfa9f2c)

# Hybrid Cloud
- A combination of computing, storage, and services in different environments public, private and on-premises data centres
- VMware and IBM provide hybrid cloud infrastructure and operations

![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/aba90ba5-4ec5-4a80-9dc4-4e5bd149ebf9)


# AWS(Amazon Web Services)
A public cloud computing platform provided by Amazon that uses distributed IT infrastructure to provide different IT
resources available on demand. It provides various kinds of services like Infrastructure as a Service(IaaS), Platform as a Service(PaaS) and Software as a Service(SaaS).

![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/e02d1949-1e32-4c7d-8abc-a1698892bf30)

# Some major domains that AWS provides its services in:
- Compute: Used to process data on the cloud by making use of powerful processors which serve multiple instances at a time.
- Storage and Content Delivery: Storage services are used to store data in the cloud, content delivery on the other hand is used to cache data nearer to the user so as to provide low latency.
- Database: Database domain is used to provide reliable relational and non-relational database instances managed by AWS.
- Networking: Services which provide a variety of networking features such as security, faster access etc.
- Management Tools: Services which can be used to manage and monitor AWS instances.
- Security and Identity: Services for user authentication or limiting access to a certain set of audience on your AWS resources.
- Application Services: Simple services like notifications, emailing and queuing come under application services.

# Compute Services:
- Amazon EC2(Elastic Compute Cloud)
  1) allows users to rent virtual computers to run their own computer applications
  2) uses EBS and instance storage to store data
  3) uses ELB to distribute data
  4) Types of EC2 instances- c type(for CPU intensive tasks), m type(for general purposes, balanced CPU and RAM), t type(for optimize usage of CPU and RAM, burst type instance), r type(for RAM intensive tasks), d type(Huge instance store), i type(Fastest Input Output Operations per second provider)
- Amazon Elastic Container Service(ECS) and Amazon Elastic Kubernetes Service(EKS) - Container orchestration services
- AWS Lambda- A serverless compute service that lets you run code for virtually any type of application without provisioning or managing servers.
- Elastic Load Balancing(ELB)
1) Load Balancer: It is a virtual machine or appliance that balances your web application load that could be http or https traffic that you are getting in. It balances a load of multiple web servers so that no web server crashes. A web server can also be consumed as a load balancer and web servers can do virtual hosting.

**Virtual Hosting**- A method for hosting multiple domain names on a single server. Eg: An apache web server can be used to deploy multiple applications/websites on different ports and works on layer 7.

**Proxy Servers**- It is a server that sits in front of one or more web servers, intercepting requests between users and the internet.
 - Forward proxy - Traffic flows from a client to the internet through a proxy server hence it accepts requests from the client.
 - Reverse proxy - Traffic flows from the internet to a web server through a proxy server hence it accepts requests from the internet servers.

<img src="https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/7a1704a3-ba0b-4c57-8dd2-0b306c7ace86" width = "500" height = "500">


2) ELB automatically manages the workload on your instances and distributes them to other instances in case of an
instance failure.

3) There are three types of load balancers:
     a) Classic Load Balancer - works on both layer 7 and 4. It routes the traffic between clients and backend servers based on IP address.
   
     b) Application Load Balancer - works on layer 7(application layer), supports path based virtual hosting. It is best suited for load balancing of HTTP and HTTPs traffic.
   
     c) Network Load Balancer - works on layer 4(network layer), supports port based virtual hosting. It is best suited for load balancing the TCP traffic when high performance is required.

**Note** - The Layer 4 load balancing can also be used for applications that rely purely on the TCP protocol.

- Amazon Elastic Container Registry
- Amazon EC2 Auto Scaling: It is used to scale up and down automatically as and when required. It can create and terminate instances automatically.
  
  a) Manual Scaling - We can update the capacity of autoscaling environment by ourselves.
  
  b) Dynamic Scaling - The capacity of autoscaling environment scales automatically as traffic change occurs.
    
     1) Simple/ Step Scaling - The process of adding an instance when the load increases beyond a set threshold and to delete an instance when load falls below a set threshold.
     
     2) Target Tracking Scaling - Maintaining certain threshold for the capacity of autoscaling environment. Eg: To keep an average of 50% CPU utilisation, when the utilisation goes beyond 50% another instance is created but in a way the utilisation remains close to 50% in the first instance.
     
     3) Scheduled Scaling - Generally used for predictable loads. Pre-warming is done so that the autoscaling environment scales at scheduled intervals.

**Pre-warming** - The process of preparing a load balancer for a surge in traffic. It involves initializing services so that they are ready to receive requests. Eg: Classic load balancers scale slowly so in order to cater spiky loads, it is pre-warmed by generating some artificial load so that it remains scaled up for the time of need. 

- Amazon Lightsail
- AWS Batch
- AWS Elastic Beanstalk
- AWS Fargate
- AWS Serverless Application Repository
- AWS Outposts
- VMware Cloud on AWS

# Using Amazon Load Balancer:

**Security Group** : A firewall for the resources on which it is attached which controls port based traffic. It can allow incoming traffic on a specific port as well as block incoming traffic from a specific port. 

![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/a843eaf3-26fa-4456-9beb-ffb0fb57ebfb)

![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/e9ca0860-7484-4b22-af42-40ec22e6a0b8)


**Traffic Port** : A certain port on which the load balancer is already receiving traffic.

- Load balancer routes the traffic to a target group which routes the traffic to a backend ec2 instances/ip address.

![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/bcdd8e2d-7e9c-4b9b-bec6-f092f508242a)


  
- Target groups route requests to individual registered targets, such as EC2 instances, using the protocol and port number that you specify.

![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/f5d3c15d-6689-4634-9832-e39f46d08c4b)


- If the load balancer is not receiving any traffic we need to override to a static port that makes the health check on that particular port instead of waiting for a request to come.
![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/1945cd56-df5f-4424-adff-601c8a1ff0a1)

- HTTP response codes: Codes starting with 4xx is client side error and 5xx type errors are server side error. 301 or 302 mean temporary or permanent redirection. 200 is the success code. ie. if everything is working fine.

![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/a1238a13-4f15-49f2-b688-fd312947633c)

![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/057aced2-e040-4d1a-9e64-cc81b395ee53)

![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/5709906f-f421-4acb-b3ee-d69e007c3a95)

![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/6d1aaa0b-dcc1-49be-8142-c9189eac1ca6)

# Using Amazon Auto Scaling:

Auto Scaling components:
- Auto Scaling Groups
![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/874260ae-a699-4a2a-90ea-4fff11749522)

- Launch template: Template for new instances
![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/d70ab055-0a52-4811-a5d2-0ed953c1db63)

- CloudWatch alarms: Triggered when a particular state occurs(eg: 80% resources are utilised) and sends notifications on that basis through SNS(Simple Notification Service)
![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/cf335320-e3a3-4f17-9225-f8fd9ed90d67)

![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/b72f9ac2-48b8-4921-8d00-0300200b7952)
![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/1b3246f2-0eaf-4efc-a012-c1e5829c88ce)

- Scaling Policies
![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/2ae6de8d-eb71-4226-b435-40ef3c9dd1db)

- CPU utilisation before
```
top
```
  ![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/c6ca2a01-7ba0-4f27-91d1-c01b57604bb8)

- Generating Artificial Load
```
seq 9999999999 > /dev/null &
```
- CPU utilisation after the load
![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/0f319f70-ce05-439d-bfa2-f6d2623f3089)

- Instance created by auto scaler
![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/96e1bdab-d1aa-412e-9ebe-98e3337d0338)

**Note** - Opening the IP adress of any of the instance and reloading the page will show different instances using Round Robin.

# Storage Services:
- Amazon S3(Simple Storage Service) - An object storage service where storage is done in chunks of data called buckets. Necessary authentications and authorisations can be applied for security.
   - Object Storage: A preformatted space to simply store files, movies, songs, etc.
   - S3 provides object storage with durability of 99.9999999% .ie. if 10 million objects are stored, an average of one object will be lost every 10,000 years.
   - It provides infinity scaling storage.
   - Only unique bucket names can be used.
   - S3 standard availibility is 99.99% .ie. it will not be available for a maximum of 53 minutes a year.
- Amazon Elastic Block Store(EBS) - Provides volumes that can be attached with EC2 instances. The size of each volume needs to be specified and it can be expanded manually.
   - Block Storage: A storage usually attached to the OS which can be later formatted by the OS for its convenience.
- Amazon Elastic File System(EFS) - Storage which is dynamically increased(keeps increasing automatically with use). It is used in shared file systems where multiple clients are writing on the same disk.
   1) It only works on Linux
   2) EFS Luster works on Windows
- Amazon S3 Glacier - It is an archival service. The data which is not in immediate use is stored here.
   1) Highly durable
   2) Cheapest storage
   3) Takes a day to fetch a file from glacier
- Amazon FSx for Lustre
- Amazon FSx for Windows File Server
- AWS Storage Gateway

# Network Services:
- Amazon VPC(Virtual Private Cloud) - A service that provides a virtual private cloud by provisioning a logically isolated section of AWS Cloud

### VPC Concepts: 

1) NACL(Network Access Control List): One of the three security services among security groups and route tables.
    - Security group: Directly attached to the instance. Stateful .ie. traffic which comes in has a way to go out.
    - NACL: Attached to a subnet. Stateless .ie. traffic which comes in may or may not go out depending on whether the outbound path is        open or not.
    - Route Table: Attached to the complete VPC.

2) VPC Peering: Connection between two different VPCs privately, similar to VPN.
   
3) VPC Endpoints: Connects two different services privately where one is private and the other one may be private/public.
   
4) VPC PrivateLink: Privately connects to a service in a 3rd party VPC. Eg: If customer and provider kind of relationship has to be established.
   
5) VPC Flow Logs: To enable network packet related tracking inside and outside VPC
    
6) Site to site VPN: To establish VPN between AWS VPC and on-premises Data Centre
    
7) Client VPN/Open VPN: Makes sure that data transfer between target and host is encrypted
    
8) Direct Connect: Direct private physical connection between data centre and AWS VPC
    
9) Transit Gateway: Connects thousands of VPCs and on-premises networks together
    
**Internet Gateway** : Virtual router that enables communication between VPC and the internet.

**NAT(Network Address Translation) Gateway** : An AWS service that allows instances in a private subnet to access the internet and connect to services outside the VPC. Only allows outbound access. 

**Subnetworking(Subnetting)** : Through subnetting, network traffic can travel a shorter distance without passing through unnecessary routers to reach its destination. When we add internet gateway to a subnet it becomes a public subnet.

**Public subnet** : Can receive traffic from outerworld. 

**Private subnet** : Cannot receive traffic from outerworld but may or may not send traffic to outerworld while remaining private.

- Amazon Route 53 - Amazon's Domain Name System
   1) DNS converts URL to IP address and vice versa
   2) DNS works on port number 53
      
   ![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/f02fea80-98e0-4094-a3c9-7f7ffd14fedc)

    
- Amazon CloudFront - Amazon's content delivery network
   1) Used for those applications whose users are spread acrosss the world
      
   3) Content is cached at the edge locations to reduce latency
      - **Edge location** is a data center that stores large data files near where users access AWS services. 216 edge locations are               available.
   4) Protection from DDoS(Distributed Denial of Service) attack with AWS shield
      
   5) CloudFront Geo-restrictions- Allow or deny users from approved or banned countries respectively

- AWS CloudFormation
  
  ![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/3b037e1a-ae04-4714-843a-8b99ba3df64d)

- AWS Global Accelerator
- Amazon API Gateway
- AWS Transit Gateway
- AWS App Mesh
- AWS Cloud Map

# Database Services:
- SQL databases: Good at transaction and concurrency control. Eg: MYSQL, Maria DB, Oracle, Aurora clusters, etc.
- Non-SQL databases: Fastest databases. Eg: Dynamo DB, Docu DB, etc.

## AWS CLI
- To interact with AWS services using commands in command line shell
- It is open source and an alternative to AWS management console
- Has direct access to public APIs
- Built on AWS SDK for Python .ie. boto or boto code
    - SDKs are Software Development Kits
    - They are used to develop and deploy applications on AWS using various languages
    ![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/80ca94fc-5fc6-45ed-b259-27b3b797901b)

# Using AWS CLI (on Cloudshell)
- Create Access Key

  ![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/28fef715-6d32-4fa9-be42-d8cced67651b)

```
aws configure
```
- Enter access key, secret key, region name and output format to get started
- Create an instance and run-
  ```
  aws ec2 describe-instances
  ```
![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/e5bdc517-140e-42fd-bb16-ccd4e211cd1b)

# Docker Containers
- Containers are like virtual machines that use the kernel of their host OS
- Cgroups- Allows control and enforcement of resources in virtual machines over a hypervisor. Eg: If a VM is allocated 2GB RAM cgroups     make sure that only 2GB is allocated to the VM and that it does not use more RAM from the host OS. 
- Namespaces- Set of characteristics which enables a VM to be a whole entity.
  
  ![image](https://github.com/Shehnaz-2005/Cloud-Computing/assets/142916147/5f60ddc9-ba7c-41d6-8445-2840e4c227d3)
