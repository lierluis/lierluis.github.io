So I'm currently in the process of learning about AWS.

A project I worked on ([ShopU]) was initially hosted on a class server on AWS,
but has since been taken down.

Now I'm trying to deploy it back to AWS since I have the Free Tier for about a year.

* RDS (Relational Database System)
* Elastic Beanstalk
* Spent quite a long time figuring out why I couldn't access the database until I realized I wasn't allowing the database to be accessed from within its security group! (thx stackoverflow)
* Accessed DB through MySQL Workbench
* Tested locally with MAMP
* Deployed project in ZIP file
* ...

<!-- Links -->
[ShopU]: {{ site.url }}{% link projects/shopu.md %}
