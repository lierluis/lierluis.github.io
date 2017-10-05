So I'm currently in the process of learning about AWS.

A LAMP stack project I worked on ([ShopU]) at my university was initially
hosted on the class server, but has since been taken down. Now I'm trying to
deploy it back to AWS since I have the [Free Tier] for about a year.

I'm writing this as clearly and concisely as I can (mainly for my own
understanding of the topic), so here I go:

##### Features
* Elastic Beanstalk: service that allows for easy deployment of an application.
Creates an environment to manage other AWS services, e.g., EC2 & S3
  * Deployed with .zip file; plan on using CodeDeploy
* EC2 (Elastic Compute Cloud) instances: virtual servers that host site
* RDS (Relational Database Service): service for using relational databases
  * Accessed DB through [MySQL Workbench] and tested locally using [MAMP]
* S3 (Simple Storage Service): cloud storage
  * Going to be using S3 bucket for storing images for my blog posts

<hr>

* EC2 (Elastic Compute Cloud): service to create virtual machines (instances) in the cloud
  * AMI (Amazon Machine Image): a template which contains a software configuration
  (e.g. OS, application server, applications) from which you launch instances,
  which are copies of the AMI
  * t2.micro: T2 instance (Burstable Performance Instance)
    * 1 vCPU, 6 CPU credits/hour, 1 GiB (gibibyte) memory, EBS-only storage
    * EBS (Elastic Block Storage) volume attached to instance: basically like a hard-drive
      * Volume type: General Purpose SSD (8 GiB, baseline 3 IOPS (I/O operations per sec) per GiB)
      * Snapshot (backup of volume) stored in S3
    * Security group: virtual firewall with a set of rules that control traffic for an instance
      * Web servers require rules that allow unrestricted access to HTTP/HTTPS ports
    * Key pair: public & private keys used to log into an instance

##### Challenges faced
* Spent quite a long time figuring out why I couldn't access the database until
I realized I wasn't allowing the database to be accessed from within its
security group! (thx stackoverflow)

<!-- Links -->
[ShopU]: {{ site.url }}{% link projects/shopu.md %}
[Free Tier]: https://aws.amazon.com/free/ "Amazon Free Tier"
[MAMP]: https://www.mamp.info/en/
[MySQL Workbench]: https://www.mysql.com/products/workbench/
