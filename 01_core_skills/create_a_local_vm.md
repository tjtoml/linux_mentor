Create a Local VM
-------------
We will have to assume that you have at least a somewhat modern computer running a 64-bit Operating System that has enough system resources for creating at least one **Virtual Machine** (VM). A virtual machine is a complete computer that is defined by software on your computer. It is effectively a computer within a computer, and is limited to a user-defined allotment of system resources. Virtual Machines are ubiquitous in modern linux administration, and being able to understand and use VMs effectively is essential. We will create a VM using commonly available software (unless you are already using a linux system, but if that's true, you don't really need to be here).

###What operating system are you currently using?

####**Windows**
You should install [VirtualBox for Windows](http://download.virtualbox.org/virtualbox/4.3.22/VirtualBox-4.3.22-98236-Win.exe). This is an automated installation that provides good defaults. After installation is complete you will likely need to reboot.

####**Mac**
You should install [VirtualBox for Mac](http://download.virtualbox.org/virtualbox/4.3.22/VirtualBox-4.3.22-98236-OSX.dmg).

####**Linux**
You're good, as far as having an appropriate environment to work in is concerned. If you wish to install virtualbox or another hypervisor, you should consult the documentation for your distribution of choice.

First VM: Your Environment
------
 These instructions assume that you have successfully installed VirtualBox and have rebooted your computer if you were requested to. We will be installing Ubuntu 14.04 because it is easy to use, especially for beginners, has excellent documentation, and a large collection of packages are available for it. As you progress in your linux education, you may wish to change your Administration VM to another distribution, such as [Arch](http://archlinux.org) or [CentOS](http://centos.org).
####Step 1: Download Ubuntu .iso
You can either do a direct http download using your web browser: [Click here](http://mirror.pnl.gov/releases/14.04/ubuntu-14.04.2-desktop-amd64.iso)

Or download a torrent (recommended): [Click Here](http://releases.ubuntu.com/14.04.2/ubuntu-14.04.2-desktop-amd64.iso.torrent)

This file is quite large, so make sure you understand what you're getting in to if you have a slow internet connection or limited bandwidth. It will also take quite a while, so we'll take a second to discuss .iso files. ISOs are disc images (a perfect, compressed copy of a CD or DVD). Most linux distributions are provided in the form of .iso files, and no matter which (major) distribution you select, the .iso will include everything you need to install the operating system on a machine, physical or virtual. It is very useful to have a copy of the .iso files for each distribution that you use regularly.

####Step 2: Create Virtual Machine
Once the Ubuntu .iso is finished downloading, open VirtualBox. These instructions are (as far as I know - I don't have a Mac to test with) the same regardless of the operating system that you have VirtualBox installed on (the  VirtualBox **host**). In this situation, Ubuntu 14.04 will be the VirtualBox **guest**.

![VirtualBox Top Bar](http://i.imgur.com/AFtjxD4.png)

Click "New" and make the settings match this:

![New VM](http://i.imgur.com/E47OBGY.png)

You will be presented with a slider that allows you to select the amount of memory (RAM) that the VM is allowed to use. It should be noted that the VM does not use all of this memory all the time - this is the maximum that the VM is allowed to use. For this specific purpose (a management VM that will use a GUI), you should drag the slider to the far right of the green section. Other VMs with different purposes will have different settings. If VirtualBox says that the maximum recommended amount of RAM is less than 1024, you will probably have issues.

After that is done, you should be presented with a window similar to this:

![New Hard Drive](http://i.imgur.com/y4IEBop.png "Hard Drive")

Select "Create a new virtual hard drive now".

The default format of VDI is fine. I would recommend using a dynamically allocated virtual hard drive to save disk space, but if your computer is slower or older, it might be a good idea to preallocate the hard drive.

I also recommend increasing the size to at least 20GB (provided that you have space available on your hard disk). 8GB is the bare minimum.

####Step 3: Change VM Settings

Once the VM is created, we still need to edit a few settings before we are ready to proceed. Select the newly created VM and click "Settings" at the top of the VirtualBox Window.

Click "System" on the left, then the "Processor" Tab. Drag the "Proccessor(s)" slider to the edge of the green, giving your VM as much power as VirtualBox says is safe.
![Processors](http://i.imgur.com/Nbf0qLG.png)


Click "Network" on the left, then change the "Attached To" on Adapter 1 to "Bridged Adapter". This will allow your VM to communicate with other devices on your local network, such as printers and other computers. This step is optional.

![Network](http://i.imgur.com/R7yUAgY.png)

Finally, click "Storage" on the left. Click the "Empty" underneath "Controller: IDE".  With that selected, click the disc icon on the far right, and navigate to where you saved your Ubuntu iso.

![DiscInserted](http://i.imgur.com/HxzGLO2.png)

You are now ready to start your brand new VM and install Ubuntu. Click OK and move on to Installing Ubuntu.
