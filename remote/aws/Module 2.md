### Module 2
EC2: virual servers to power your needs
- AWS already owns the servers and you can use the powers you need whenever you need
Multitenancy: sharing hardware with multiple hosts. hypervisor is what delegate the shared resources
	- hosts don't have to set this up
EC2 has lots of flexibility due to lots of options to set up configuration
- user has complete control with what the server can be used for 
- the ec2 instances can be scaled <span style="background:#fff88f">vertically</span> where more ram etc can be added
- users can also decide the networking so what reached the server
CaaS(compute as a service model)
each instance type for EC2 is grouped in different categories that have different qualities for different purposes
Categories:
- general purpose
- compute optimized
	- batch processing
- memory optimized
	- lot of storage in memory
- accelerated computing
- storage optimized
	- big data
EC2 Purchase options:
- on-demand: pay for what you need
- savings plans: offers low prices for ec2 usage for commitment on usage terms -> up to 72% savings
	- terms are 1 and 3 years
- reserved instances: used for predictable usage which is more for consistent and known usage amount -> upfront/partial/no costs
- spot instances: offers spare ec2 instance usage but aws can reclaim the servers at any point
- dedicated hosts: physical servers dedicated for clients
Scalability/Elasticity:
- Scalability: automatically allocates the resources needed for the client
	- Auto scaling group: a method to set a minimum and maximum number of instances to acomodate the client's needs
Elastic Load Balancing:
- load balancer is what routes traffic to different servers to manage the traffic to the application so process don't become slow
Messaging and Queuing:
- tightly coupled architecture: when issue with one part of an app can cause an issue with another app -> monolithic application
- loosely coupled architecture: single failure won't cause a cascade of issues
	- using a message queue in between different apps will cause other apps to not fail if one app fails
- Amazon Simple Queue Service:
	- send, store, and receive messages between software components
	- think of data structure queue
	- where messages are places until app is able to pick it up
- Amazon Simple Notification Service:
	- used to send out messages to services but also send out notifications to customers
	- uses SNS topic which is a channel for messages to be sent
	- similar to kafka topic
	- publish and subscriber model
Additional Computer Services:
- Serverless compute: you cannot see or access the underlying infrastructure
	- AWS Lambda: where users can input their code into the service and the service computes the process
		- they are also known as lambda triggers
		- can run code under 15 minutes so more quick processing and not deep learning etc.
		- short running functions with no OS management
- Amazon Elastic Container Service:
	-  docker containers that uses os level virtualization to perform processes
	- these containers run on top of ec2 instances and are isolated -> host is ec2 instance
	- Container orchestration where multiple containers run as a cluster
	- orchestration pools aid the cluster running
- AWS Fargate
	- serverless environment where the clusters are managed for you
- Amazon Elastic Kubernetes Service:
	- similar to Amazon ECS



