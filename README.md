### Cloud
  Cloud Terminology
  1. High Availability.
  2. Fault Tolerance.
  2. Scalability
  3. Elasticity.

### Aws Global Infrastructure Layers
  1. Region
  2. Availability zone
  3. Datacenter

### Storage service - S3
  Structure
    1. Buckets
    2. Folders
    3. Objects

  Storage Classes: It is the classification assigned to each object in s3.
    1. Standard
    2. Standard IA(Infrequent Access)
    3. One zone IA
    4. Intelligent Tiering
    5. Glacier

  Metrics
    1. Object Durability.
    2. Object Availability.

  Life cycle policies:
    You set your own parameters(mostly time) to automate the process of changing the storage classes.

  Features
      1. Object Sharing.
      2. Object life cycle.
      3. Object Versioning.

### Networking
  1. Virtual Private Cloud(VPC).
    * It will be inside a perticular region.
  2. Subnets.
    * It is a shorthand for subnetwork.
  3. Network Access control List(ACL).
    * A firewall/security layer on the subnet level.
  4. Security groups.
    * A firewall/security layer on the instance/server level.

### Computing Services
  1. Elastic compute cloud(EC2)
    * They are virtual server. In simple words the computers which are in cloud.
    * Basic Components
      - AMI(Amazon machine Images): Its the way to select operating system to your EC2.
      - Instance Type - Processing Power.
      - EBS(Elastic Block storage) - Local storage.
      - IP addressing.
      - Security Groups.
      - RAM
    * Buying Options
      - On demand
      - Reserved
      - Spot
  2. AWS Lambda
    * Lambda is serverless computing.
    * AWS Lmabda run your code on a high availability compute infrastructure and performs all the administration of the compute resources including server and operating system maintainance, capacity provisioning, automatic scaling, code monitoring and logging.

### Elastic Load balancing and Auto scaling
  These not the primary services in AWS. These are the features of networking and computing services.
  1. Elastic load balancer
    * It evenly distributes traffic between EC2 instances that are associated with it.
    * It is the foundational component of high availability and fault tolerant system.
  2. Auto Scaling Services.
    * Auto scaling automates the process of adding(scaling up) or removing(scaling down) the EC2 instances based on the traffic on your application.
    * You can specify the minimum and maximum number of insatnces in your autoscaling.
    * Scaling policies.
      Setting up the rules for scaling.
    * Autoscaling adds scalabilty and the elasticity.


### Content Delivery and DNS Services
  1. Route 53(Domain and DNS services)
    Route 53 is where you configure and manage web domains for websites or applications you host on AWS.

    The main 3 functions of Route S3 are;
      a. Domain registration.
      b. DNS service.
      c. Health checking.

    Multi-region failover.
  2. Cloudfront (content delivery network)
    Cloudfront is a CDN. It allows to cache your content at "edge locations" located all around the world.
    This allows the customer to access the content more quickly and also provides additional security against DDOS(Dedicated Denial of service) attacks.

    Edges locations are used to cache the data. They are separate from aws regions, but have datacenters that cache the important data.



### Monitoring and logging services
  1. Cloudwatch
    Cloud watch is a service that lets you monitor various elements of your AWS account.
    Metrics
    Alarms
  2. Cloudtrail
    Cloudtrail allows you to monitor all actions taken by IAM users.


### Notification Services
  1. SNS(Simple notification service)
    An AWS service that automates the sending of email or text message or other type of notifications, based on the events that happen in your AWS account.

### Database Service
  1. RDS(Relational database services)
    It is a SQL database service that provides a wide range of SQL database services to select from(Aurora, mysql, oracle etc).
  2. DynamoDB (NoSQL db)
    It is a NoSQL database service. Unlike RDS it doesnt provide other NoSQL software options.
    It can replace Mongodb, cassandraDB, oracle NoSQL
    It is super fast.
    It can automatically scale and serverless.
    Supports both document and key-value store models.
  3. ElastiCache
    ElastiCache is a data caching service used to help improve speed performance of web applicactions running on AWS.
    ElastiCache supports two open source in-memory services
    * Redis
    * memcacheD
  4. Redshift
    Redshift is a data warehouse database service designed to handle petabytes of data for analysis.


### AWS Billing and support
  1. AWS Organizations
    Organizations allow you or your company to manage billing and access to multiple AWS accounts.
    Place where you can centrally manage access policies of multiple AWS accounts.

    **Consolidated Billing** allows you to view, manage, and pay bills for multiple AWS accounts in one user interface.

    Main features of consolidated billing;
    * Central location to manage billing across all your AWS accounts.
    * Gain volume discounts for usage across all your AWS accounts.

    In AWS the more you use, the cheaper it becomes.

  2. AWS Pricing model
    AWS pricing principles
    * Pay as you go.
    * No long term contracts or licencing is involved.
      - Exceptions are reserved EC2 instances.
    * Volume discounts are available
    * There are no termination fees.
    * AWS offers a free tier options to those who are new to AWS.

  3. AWS billing and cost tools
    **Total Cost of Ownership(TCO) Calculator:** It is a free tool provided by AWS that allows you to estimate the cost savings of using the AWS cloud vs using an on-premisis database.

    **AWS Cost Explorer:** It is a free tool that allows to see the charts of your costs.
    You can also forecast how much you can spend for next 3 months.

  4. AWS Shared responsibility Model
    Shared responsibility model defines what you and Amazon web services are responsible for when it comes to security and compliance.

    AWS services with built-in DDoS Protection
     * Route 53
     * Cloudfront
     * WAF(Web appliction firewall)
     * Elastic load balancing
     * VPC and Security groups

    **Penetration Testing:** You must request permission from AWS before doing the penetration testing.
    Pernetration testing is allowed for some of the AWS services like EC2, lambda, RDS etc.

  5. AWS support plans and trusted advisor.
    AWS account support plans:
    Basic, developer, business and enterprise.

    **AWS Trusted Advisor:** It is a service that advises and helps you optimize aspects of your AWS account.

    Trusted advisor categories:
    * Cost optimization.
    * Performance.
    * Security.
    * Fault tolerance.

    AWS trusted advisor has different level of support based on the type of AWS support account.

  6. AWS whitepaper and documentation
    * Whitepapers: These are collection of technical documents that outline many AWS relevant topics such as 
      - Architecture best practises
      - Security best practises
      - Cloud computing economics
      - Serverless architecture
    * AWS service documentation: It is a collection of document specific to each service and features.






























