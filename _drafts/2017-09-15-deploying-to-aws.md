So I'm currently in the process of learning about AWS.

A LAMP stack project I worked on ([ShopU]) at my university was initially
hosted on the class server, but has since been taken down. Now I'm trying to
deploy it back to AWS since I have the [Free Tier] for about a year.

I'm writing this as clearly and concisely as I can (mainly for my own
understanding of the topic), so here I go:

##### Features
* EB (Elastic Beanstalk): application container service
  * Creates an environment to manage other AWS services, e.g., EC2 & S3
  * Deployed with .zip file; plan on using CodeDeploy
* EC2 (Elastic Compute Cloud) instances: virtual servers that host site
* RDS (Relational Database Service): service for using relational databases
  * Accessed DB through [MySQL Workbench] and tested locally using [MAMP]
* S3 (Simple Storage Service): cloud storage
  * Going to be using S3 bucket for storing images for my blog posts
* Elastic IP address: static IPv4 address (can be remapped to different instances)
* Route 53: domain (DNS) and traffic management (not using this)
* ELB (Elastic Load Balancer): traffic manager
* CloudWatch: resource and application monitoring

<hr>

* EC2 (Elastic Compute Cloud): service to create virtual machines (instances) in the cloud
  * AMI (Amazon Machine Image): a template which contains a software configuration (e.g.,
    OS and additional software) from which you launch instances, which are copies of the AMI
  * Instance type determines hardware of host computer used for your instance
    * t2.micro: T2 instance type (Burstable Performance Instance)
      * 1 vCPU, 6 CPU credits/hour, 1 GiB (gibibyte) memory, EBS-only storage
  * Key pair: public & private keys used to log into an instance
    (AWS stores public key, you store private key)
  * Instance store volume: storage volumes for temporary data
  * EBS (Elastic Block Storage) volume attached to instance: persistent storage for data
    * Volume type: General Purpose SSD (8 GiB, baseline 3 IOPS (I/O operations per sec) per GiB)
    * Snapshot (backup of volume) stored in S3
  * Region and Availability Zone (AZ): US West (Oregon) 2a, 2b, 2c
  * Availability Zone (AZ): Amazon's data centers
  * Security group: virtual firewall with a set of rules that control traffic for an instance
    * Web servers require rules that allow unrestricted access to HTTP/HTTPS ports
    * Apply the principle of least privilege (only open up permissions that you require)
      * Restrict SSH access by restricting incoming traffic on port 22
      * Disable password-based logins for instances
  * Elastic IP address: static IPv4 address for dynamic cloud computing (can be
    remapped to different instances to mask the failure of an instance?)
  * Tags: metadata
  * VPC (Virtual Private Cloud): virtual network logically isolated from the rest of
    the AWS cloud, that you can create and connect to your own network
  * Instances can be stopped (shutdown), terminated (deleted)

<hr>

* ssh -i ~/.ssh/MyKeyPair.pem ec2-user@IP-address
  * common user names: ec2-user, root, ubuntu, fedora

##### Challenges faced
* Spent quite a long time figuring out why I couldn't access the database until
I realized I wasn't allowing the database to be accessed from within its
security group! (thx stackoverflow)
* When deploying with Elastic Beanstalk, make sure to upload the ZIP file of
the <em>contents</em> of the project, as opposed to the ZIP file of the
<em>folder</em> containing the contents (downloading ZIP file from GitHub
will be the latter!)

<!-- Links -->

[ShopU]: {{ site.url }}{% link projects/shopu.md %}
[Free Tier]: https://aws.amazon.com/free/ "Amazon Free Tier"
[MAMP]: https://www.mamp.info/en/
[MySQL Workbench]: https://www.mysql.com/products/workbench/
