### Module 3
- need high availability and fault tolerance to accomodate for different situation
	- you need a global infrastructure for people to use for the application
- doesn't make sense for companies to run their own data centers
- aws build the data centers in different regions
	- the data centers have different services that can be used and each are connected with high speed fiber networking
	- each region is isolated from each region so all data is very exclusive to each data center
	- regional data sovereignty is part of the critical design for the AWS regions
	- should take into consider your local compliance requirements
	- should take into consideration the latency of how far your server is from all your customers
	- feature availability: what services are available in your preferred data center
	- pricing is another factor
- AWS has lots of data centers and a region is multiple data centers
- Availability Zone is one more data centers and a region is multiple AZs
- The AZs are spaced in a region such that it maintains fault tolerance if one goes down and latency is low
Edge Locations:
- Amazon Cloud front: service to help deliver resources to customers across the world with low latency and high speed. The server utilizes edge locations from different regions to accelerate delivery
- Amazon Route 53: a DNS service to direct customers to the right location with low latency
- AWS outposts: service where AWS builds a small datacenter within the client's building
- Regions are geographically isolated zones and regions contain AZs
- Edge locations run Amazon Cloudfront
- you should deploy infrastructure across at least 2 AZs
Provision AWS resources:
- everything is an API to use services
- AWS management console, AWS command line interface(CLI) and AWS SDK to utilize the resources offered by aws
- AWS Elastic Beanstalk: Provide application code to build out the environment out for you. Lets you focus on business application rather than the infrastructure
- AWS Cloudformation: infrastructure as code tool to define a wide variety of AWS resources in a declarative way using json and yaml files
	- manages all the AWS apis for you and can be done across different environments
- CLI: to script your environments for application usage
- 
