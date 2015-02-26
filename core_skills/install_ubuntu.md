Installing Ubuntu 14.04 Desktop as a VirtualBox Guest
------
If you followed the instructions in the tutorial on [installing VirtualBox and creating a management VM](https://github.com/tjtoml/linux_mentor/blob/master/core_skills/create_local_vm.md), you are ready to continue. 

##Start the VM
This one is easy. Just select your VM on the left and click "Start" at the top of the VirtualBox window. The VM will boot from the .iso image you provided, and after a minute or two you will be presented with a screen that looks like this: 
![UbuntuLive](http://i.imgur.com/rLHjRK1.png)

At this point, you should select your language on the left. 

##Install 
Click "Install Ubuntu", then check the box to download updates:
![Install1](http://i.imgur.com/cUIeIXv.png)

We just created the VirtualBox disc image that the VM sees as its hard drive. Since there is no danger to our computer, we can accept the defaults that Ubuntu uses. Select "Erase disk and Install Ubutnu" and click "Install Now": 
![Install2](http://i.imgur.com/ynOvHmH.png)

If you followed the recommendation to make the VirtualBox hard drive 20GB, this should proceed without a problem. If you did not, the installer may create a swap partition that takes up too much space, and the installer complains about not having enough disk space. If this is a problem, delete and recreate the VM with a larger hard drive.  

Select your timezone and keyboard layout.