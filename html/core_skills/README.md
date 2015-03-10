[r/linux_mentor](http://reddit.com/r/linux_mentor) Core Skills
===================
This section will focus on familiarizing the complete neophyte with the linux operating system, the basics of using a terminal emulator, ssh, and virtualization. After completing this section, you should be prepared to provision a new VM (either locally or via a cloud-hosting service) and follow along in a tutorial. 

----------

##Creating a Local Work Environment
The first thing any linux administrator needs is an environment designed to interact with the servers he administers. Strictly speaking, one can get by with a SSH client like [PuTTy](http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html) that provides a console connection to a remote server, but I believe that the best way to learn is by immersion. Specifically, I think you should administer linux servers from a linux operating system. Why?

 * You can write and scripts on a local system
 * Key utilities are already included (a decent terminal emulator is key)
 * You can run software on your local machine that interacts with remote systems natively
 * Many more...
 
This can be accomplished in two ways: you can either install a linux distribution to your local hard drive, or you can create a Virtual Machine (VM). I am not prepared to give up essential programs that are Windows only, so I elected to use the Virtual Machine approach. 



To get started, [install VirtualBox and create a VM.](https://github.com/tjtoml/linux_mentor/blob/master/core_skills/create_local_vm.md) 

Once that is done, [install Ubuntu 14.04 on your new VM](https://github.com/tjtoml/linux_mentor/blob/master/core_skills/install_ubuntu.md). 

##Setting up SSH
Secure SHell (ssh) is the linux administrator's swiss army knife. It provides a secure connection to a remote system that makes it as if you are typing commands on a local machine. It's easy to set up: check out setting up SSH. 