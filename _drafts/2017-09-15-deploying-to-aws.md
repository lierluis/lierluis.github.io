So I'm currently in the process of learning about AWS.

A LAMP stack project I worked on ([ShopU]) at my university was initially
hosted on the class server, but has since been taken down. Now I'm trying to
deploy it back to AWS since I have the [Free Tier] for about a year.

##### Features
* Elastic Beanstalk: service that allows for easy deployment of an application.
Creates an environment to manage other AWS services, e.g., EC2 & S3
  * Deployed with .zip file; plan on using CodeDeploy
* EC2 (Elastic Compute Cloud) instances: virtual servers that host site
* RDS (Relational Database Service): service for using relational databases
  * Accessed DB through [MySQL Workbench] and tested locally using [MAMP]
* S3 (Simple Storage Service): cloud storage
  * Going to be using S3 bucket for storing images for my blog posts

##### Challenges faced
* Spent quite a long time figuring out why I couldn't access the database until
I realized I wasn't allowing the database to be accessed from within its
security group! (thx stackoverflow)

<!-- Links -->
[ShopU]: {{ site.url }}{% link projects/shopu.md %}
[Free Tier]: https://aws.amazon.com/free/ "Amazon Free Tier"
[MAMP]: https://www.mamp.info/en/
[MySQL Workbench]: https://www.mysql.com/products/workbench/
