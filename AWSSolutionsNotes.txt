# Topic Weight
- Designing HA, cost efficient, fault tolerent, scalable systems - 60%
- Implementing/Deploying  - 10% 
- Data Security - 20%
- Troubleshooting - 10%

# About the Exam
- 80 minutes
- 60 Questions
- Multiple Choice
- Pass based on Bell Curve
- Qualification valid for 2 years
- Scenario Based questions


# Services related to exam
- Messaging
- Desktop & App Streaming
- Security & Identity
- Management Tools
- Storage
- Databases
- Networking & Content Delivery
- Compute
- AWS Global Infrastructure

# AWS Global Infrastructure
- 14 regions (2016)
- 38 Availability Zones (2016)
- 4 more Regions (2017)
- 11 more Availability Zones (2017)

### What is a region? 
- A region is a geographical area.
- Each region consists of 2 or more availability zones

### What is an AZ?
- Simply a data center

### What is an edge location?
- They are CDN end points for CloudFront
- Currently there are 66 edge locations
- Used for caching purposes

# AWS - 10,000 Feet Overview
### Networking & Content Delivery
- VPC 
    - Virtual Private Cloud
    - Think of as a Virtual data center
    - Know how to build a VPC from memory for exam
- Route53
    - DNS Service
- Cloud Front
    - CDN 
    - Edge Locations 
    - Cache Videos, Photos, media
- Direct Connect
    - Connect Office or Physical Datacenters using telephone line to AWS
    - Need reliable internet connection

### Compute
- EC2
    - Elastic Compute Cloud 
    - VMs in the Cloud
- EC2 Container Service
    - Highly Scalable container management service
    - Supports docker containers
- Elastic Beanstalk
    - Deploy code without knowing EC2
    - Elastic Beanstalk analyzes code to deploy to EC2
- Lambda 
    - Serverless Computing
    - Functional Programming
- LightSail 
    - Out of the Box Cloud
    - VPS via AWS

### Storage
- S3
	- Simple Storage Service
    - Virtual Disk in the Cloud
    - Files referenced as Objects
    - Object Based Storage
- Glacier
    - Archive files from S3
- EFS
	- Elastic File Storage
	- Block Based Storage
- Storage Gateway
	- Connecting S3 to on Prem data center

### Databases
- RDS
	- Relational Database Service
		- MySQL
		- PostgreSQL
		- MariaDB
		- SQLServer
		- Oracle
		- Aurora
			- Comes in 2 Flavors
				- MySQL
				- PostgreSQL
- DynamoDB
	- Non-Relational Database Service
	- Scalable
	- NoSQL
- Redshift
	- Big Data Storage
	- Data Warehousing
- Elasticache 
	- Take heavy loads off of DB using caching

### Migration
- Snowball
	- Import/Export to AWS
	- An appliance to transfer data to AWS
	- Snowball Edge
		- On prem compute from AWS
- DMS 
	- Migrate onprem DB to cloud
	- Migrate DB from regions in AWS
	- 0 Downtime
	- Don't have to keep same DB type
		- Migrate from Oracle to Aurora Oracle (Cut Licensing Costs)
- Server Migration Service
	- Move VMWare VMs to AWS
	- 50 Concurrently at a time

### Analytics
- Athena
	- Run SQL queries on S3
	- CSV files in buckets can be queried
- EMR
	- Big Data Processing
	- Log Analysis
	- Frameworks used:
		- Hadoop
		- Apache Spark
		- Presto
		- Flunk
		- Apache HBase
- Cloud Search
	- Fully Managed for Search Capabilities
- Elastic Search
	- Self Managed for Search Capabilities
- Kinesis
	- Stream and Analyze Real-Time data
- Data Pipeline
	- Move data from one place to another
		- From S3 to Dynamo
- QuickSight 
	- Business Analytics tool
	- Build Dashboards for viewing data

### Security & Identity
- IAM
	- Identity Access Manager
	- Authenticate to AWS
- Inspector
	- Agent installed to VMs for Security 
- Certificate Manager
	- Free SSL Certs for Domains
- Directory Service
	- Use AD with AWS
- WAF
	- Web Application Firewall
	- Application level protection
		- XSS
		- SQL Injection
- Artifacts 
	- Documentation for security certification
	- Compliance Documents

### Management Tools
- Cloud Watch
	- Monitor Performance in AWS Services
- Cloud Formation 
	- Turn Infrastructure into Code
	- Document that describes your infrastructure
	- Configure entire production setup using only code
	- IAAS
- Cloud Trail 
	- Record actions in AWS Environment
- Opsworks
	- Automate deployment using CHEF
- Config 
	- Automatically monitor environment
	- Set alerts for conflicting events in AWS environment
- Trusted Advisor
	- Tips on optimization
		- Performance 
		- Security

### Application Services
- Step Functions
	- Visualize what is going in an Application
		- Processes
		- Services
- SWF 
	- Simple Workflow Service
	- Automated tasks 
	- Human led tasks
- API Gateway
	- Apps to access backend data
		- Lambda
		- DB
- AppStream
	- Stream desktop applications to users
- Elastic Transcoder
	- Changes video format based on streaming device

### Developer Tools
- CodeCommit
	- Git in AWS
- CodeBuild
	- Compile code 
	- Pay by minute
- CodeDeploy
	- Deploy code
- CodePipeline
	- Keep track of code versions

### Mobile Services
- Mobile Hub
	- Add, configure, design features for mobile app
	- Console for mobile apps
- Cognito
	- User auth for mobile apps
- Device Farm
	- Test mobile apps on hundreds of real devices
- Mobile Analytics
	- Collect & Analyze app usage data
- Pinpoint
	- Engage with app users
	- Gather what users are using the app for
	- Understand user behavior

### Business Productivity 
- WorkDocs
	- Store work docs in the cloud
		- uses s3
	- WorkMail
		- Exchange for AWS

### Internet of Things
- IOT
	- Tracking iot devices

### Desktop & App Streaming
- WorkSpaces
	- VDI
	- Desktop in the Cloud
- AppStream 2.0
	- Stream Desktop apps to users

### Artificial Intelligence
- Lex
	- Amazon Voice service
- Polly 
	- Text to Speech 
- Machine Learning
	- Give AWS Data set and outcomes 
	- Analyze data based on dataset and act upon it based on machine learning decisions
	- Predict data based on previous performance
- Rekognition
	- Upload image and give you data based on picture 
	- Facial Recognition
	- Percentage of Recognition

### Messaging
- SNS
	- Simple Notification Service
	- Email , SMS, HTTPS Endpoints
- SQS
	- Simple Queue Service
	- Post jobs to a queue
- SES
	- Simple Email Service
	- Send emails using AWS

# Identity Access Management (IAM)
- Configure who uses AWS
- Allows you to manage users and their level of access to the AWS console. 
- What does IAM give you?
	- Centralized control of your AWS account
	- Shared Access to your AWS account
	- Granular Permissions
	- Identity Federation
		- AD
		- Facebook
		- LinkedIn
	- Multifactor Authentication
	- Provide temporary access for users/devices and services where necessary
	- Allows you to set up your own password rotation policy
	- Integrates with many different AWS services
	- Supports PCI DSS Compliance
- Critical Terms
	- Users
		- End Users (Think People)
	- Groups
		- A collection of users under one set of permissions
	- Roles
		- You create roles and can then assign them to AWS resources
	- Policies 
		- A document that defines one or more permissions

# Identity Access Management 101 - Lab
- Console > Services > Security, Identity, & Compliance > IAM
- Notice IAM doesn't have a region
	- IAM is a global service 
- IAM users sign in link available here
	- Able to be customized
- Set up MFA 
	- Using either physical or virtual token
		- Virtual
			- Authy
			- Google Authenticator
		- Physical 
			- Phone
			- FOB from AWS
- Set up user
	- User Name
	- AWS Access type
		- Programmatic Access
			- for users that will use the AWS API, CLI, or SDK
		- AWS Management Console Access
			- for users that will access the AWS Console
	- Console Password
		- Autogenerated Password
		- Custom Password
	- Require Password reset
	- Add Permissions
		- Add users to group
			- Create group
				- Group Name
				- Policies
					- EX. (DB Access, S3 ACCESS, EC2 Read Only)
		- Copy permissions from existing user
		- Attach existing policies directly
	- User Table
		- Access Key 
		- Secret Access Key 
		- Password
	- To login to the console the username and password would be used
	- To login programmatically you would use the access key and secret access key
    - 


# Questions 
### AWS - 10,000 Feet Overview
- What is an AWS region?
	- A region is a geographical area that consists of different availability zones. Each region consists of 2 (or more) Availability Zones.
- What does an AWS Region consist of? 
	- An independent collection of AWS computing resources in a defined geography.
- Which statement best describes Availability Zones?
	- Distinct locations from within an AWS region that are engineered to be isolated from failures.
- An AWS VPC is a component of which AWS service?
	- Networking Service.
- What is a VPC?
	- Virtual Private Cloud
- Which AWS service is specifically designed for developers to upload their code to and then it will automatically handle the provisioning of those resources that are required to host that code?
	- Elastic Beanstalk
- Which AWS service allows you to run code without having to worry about provisioning any underlying resources (such as virtual machines, databases etc)
	- Lambda
- Amazon's highly scaleable DNS service is known as...
	- Route 53
- Which AWS compute service is specifically designed to assist you in processing large data sets?
	- Elastic Map Reduce
- What is the difference between Elastic Beanstalk & CloudFormation?
	- Elastic Beanstalk automatically handles the deployment, from capacity provisioning, load balancing, auto-scaling to application health monitoring based on the code you upload to it, where as CloudFormation is an automated provisioning engine designed to deploy entire cloud environments via a JSON script.
- Which AWS service is used a CDN to distribute content around the world?
	- CloudFront
- Where would be a durable place to store flat files on the AWS platform?
	- S3
- Which AWS service would be the best choice for long term data archival?
	- Glacier
- What AWS service consists of the following database services; SQL, MySQL, MariaDB, PostgreSQL, Aurora, Oracle?
	- Relational Database Services (RDS)
- What AWS service would you use primarily for data warehousing?
	- Redshift
- What AWS service is used for collating large amounts of data streamed from multiple sources? 
	- Kinesis
- You need to create new users to access the AWS console and to set password rotation policies for these new users. Which AWS service would best fit your requirements?
	- Identity Access Management (IAM)
- You need to supply auditors with logs as to who provisions which resources on your AWS platform. Which service would best suit this?
	- CloudTrail
- You need a configuration management service to allow your system administrators to configure and operate your web applications using Chef. Which AWS service would best suit your needs?
	- Opsworks
- You are a digital media agency and you need to convert your media files in to different formats to suit different devices. Which AWS service should you consider using to meet these needs?
	- Elastic Transcoder









