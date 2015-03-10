#[r/linux_mentor](http://reddit.com/r/linux_mentor) Knowledge Database
===================
The purpose of this project is to collect tutorials related to administration of linux systems in a unified, consistent format. We will also attempt to present information in a logical progression, so that someone with little or no knowledge or background in Linux Administration can start at the beginning and progress to a competent administrator.

----------
How This Book is Organized
-------------
####Getting Started
This section will outline the various options you have to complete the tutorials that follow.
####Core Skills
Things discussed in this section will be old hat to anyone who has any sort of background in Linux administration. We will go over the basics of git and SSH, installing VirtualBox, creating a local VM, and using it as a local administration environment.
####Monolithic Servers
The book will then progress into tutorials concerned with creating monolithic servers. A monolithic server is one in which all of the programs required to provide a service run on one computer. A computer with a LAMP (Linux Apache MySQL PHP) stack installed is an example of a monolithic server because all of the software required to provide the the service (a database backed dynamic website) are running on a single computer.
####Clustering, Load Balancing, and High Availability
After we have a good understanding of how to create single servers to provide a service, we will move on to scaling our applications by creating clusters of machines that provide the same service to a larger number of clients. It is worth noting that each of these topics could easily have books devoted to them alone - we will only be touching on the basics.
####Configuration Management
After you have manually configured a few clusters, you will quickly start to realize that much of the work is repetitive - so why repeat it? In this section we'll look at at Ansible and Puppet for automating the deployment of our servers.


