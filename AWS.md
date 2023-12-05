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

## Some major domains that AWS provides its services in:
- Compute: Used to process data on the cloud by making use of powerful processors which serve multiple instances at a time.
- Storage and Content Delivery: Storage services are used to store data in the cloud, content delivery on the other hand is used to cache data nearer to the user so as to provide low latency.
- Database: Database domain is used to provide reliable relational and non-relational database instances managed by AWS.
- Networking: Services which provide a variety of networking features such as security, faster access etc.
- Management Tools: Services which can be used to manage and monitor AWS instances.
- Security and Identity: Services for user authentication or limiting access to a certain set of audience on your AWS resources.
- Application Services: Simple services like notifications, emailing and queuing come under application services.

## Compute Services:
- Amazon EC2(Elastic Compute Cloud)
  1) allows users to rent virtual computers to run their own computer applications
  2) uses EBS and instance storage to store data
  3) uses ELB to distribute data
  4) Types of EC2 instances- c type(for CPU intensive tasks), m type(for general purposes, balanced CPU and RAM), t type(for optimize usage of CPU and RAM, burst type instance), r type(for RAM intensive tasks), d type(Huge instance store), i type(Fastest Input Output Operations per second provider)
- Amazon Elastic Container Service(ECS) and Amazon Elastic Kubernetes Service(EKS) - Container orchestration services
- AWS Lambda- A serverless compute service that lets you run code for virtually any type of application without provisioning or managing servers.
- Amazon Elastic Container Registry
- Amazon EC2 Auto Scaling
- Amazon Lightsail
- AWS Batch
- AWS Elastic Beanstalk
- AWS Fargate
- AWS Serverless Application Repository
- AWS Outposts
- VMware Cloud on AWS

## Storage Services:
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

## Network Services:
- Amazon VPC(Virtual Private Cloud) - A service that provides a virtual private cloud by provisioning a logically isolated section of AWS Cloud
- Amazon Route 53 - Amazon's Domain Name System
   1) DNS converts URL to IP address and vice versa
   2) DNS works on port number 53
- AWS Direct Connect - 
- Amazon CloudFront
- AWS Private Link
- AWS Global Accelerator
- Amazon API Gateway
- AWS Transit Gateway
- AWS App Mesh
- AWS Cloud Map
- Elastic Load Balancing
