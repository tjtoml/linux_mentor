[r/linux_mentor](http://reddit.com/r/linux_mentor) Knowledge Database
===================
The purpose of this project is to collect tutorials related to administration of linux systems in a unified, consistent format. We will also attempt to present information in a logical progression, so that someone with little or no knowledge or background in Linux Administration can start at the beginning and progress to a competent administrator.

----------


Organization of this Repository
-------------
####Core Skills
This repository is separated into three[^change] major sections. The first is core skills and setup. This is intended to get you started if you have no previous experience using linux operating systems, and will provide the foundation for later tutorials. This section can probably be skipped if you feel comfortable installing and using a desktop distribution of linux, but it might be a good idea to read through even if you are very confident in your abilities. You never know when you might learn something.
####Tutorials
The tutorials section will assume that the knowledge and skills outlined in the core skills section are successfully configured. Absolute understanding is not necessary: you will learn more as you follow along. A tutorial is a standalone document: it should not depend on other tutorials in order to function.
>**Example of tutorial dependence:**
>Tutorial A details the setup of a bind based nameserver. Many custom options are configured, and the zone files are in a nonstandard format (this is a made-up example). Tutorial B details the setup of an nginx webserver and depends on the custom configuration from tutorial A, and includes instructions like "edit the zone file at `/non/standard/path` ".

>**Example of tutorial independence:**
>Tutorial A details the setup of a bind based nameserver. Many custom options are configured, and the zone files are in a nonstandard format (still made-up). Tutorial B details the setup of an nginx webserver and depends inludes instructions like "Add an A record pointing to web.example.com. If you do not know how to do this, please see the section on [DNS](#)."

Tutorials are intended to detail the installation and configuration of a *single* service or program. This gets a bit fuzzy when things like LAMP stacks come into play, but as a basic rule of thumb a tutorial should be for the configuration of a single **server**.  For instance, a tutorial should not be entitled
>**Load Balancing Multiple nginx Servers using haproxy**

Instead there should be two separate tutorials:

>**Installing and Configuring an nginx Web Server**

>**Using haproxy to Load Balance Web Traffic**

####Lessons
Lessons are the application of skills developed in the tutorial section. In contrast to a tutorial, a lesson will *always* depend on other lessons or tutorials - if it does not, it is a tutorial. In other words, a tutorial outlines the basic tenets of usage and installation for a linux program or service (nginx), while a lesson leverages those basic tenets to create something useful (Load-Balanced WordPress using nginx and haproxy).

On Linking, Reinventing the Wheel, and Plagiarism
------
 Obviously, any project that attempts to collect and organize tutorials on the internet will likely end up saying very nearly the same thing as a several hundred other people. In fact, many of my personal bookmarks are my favorite tutorials written by a great number of people. However, this repository is not a collection of links. A subreddit can handle that task.  If you have found an excellent tutorial elsewhere on the internet, and feel that it warrants inclusion into this repository, you should recreate it in markdown, including an attribution (the original author's name) and a link to the original tutorial. You should also contact the original author and ask for permission before submitting a pull request. For full details, please consult the [style guide](#ADDLINKLATER).


[^change]:This is subject to change as the project evolves.
