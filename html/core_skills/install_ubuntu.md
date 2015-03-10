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

Select your timezone and keyboard layout. Enter your name where it asks, but I strongly recommend changing the default settings that Ubuntu extrapolates from your name:

![UnamePwd](http://i.imgur.com/lvVZaHY.png)

You may notice that I use a weak password. This VM is for my personal use, and will not come in to contact with any sensitive information. It is also located on my personal desktop computer, and I am not incredibly worried about that being compromised. Select a password with your environment in mind. 

You're almost done. Go grab a cup of coffee, because the actual installation takes a while. 

![InstallingNow](http://i.imgur.com/XS6XJYE.png)

##Rebooting into Your New System

Eventually, you will be presented with this screen: 
![Restart](http://i.imgur.com/ms4bnLW.png)

Go ahead and click Restart Now. Edit the VM settings to remove the .iso file. You may have to manually power off the VM by Right Clicking it in VirtualBox and selecting Close > Power Off before you can do this (I did). 

After this is done, you should boot into a fresh system, but the window will probably be incredibly small and un-resizable. Click inside the VM's window and press Ctrl+Alt+T to open a terminal window. Type these commands, pressing enter after each. You will have to confirm your choices [Y/n]. This can be bypassed without pressing Y, you simply need to press enter. The capital letter indicates that this is the default option.

`sudo apt-get update`
`sudo apt-get upgrade`
`sudo reboot now`

This will fetch updates from the server, install the newest versions of the software on your VM, and reboot the machine. Once this is done, click "Devices" in the VM menu (in VirtualBox) and select "Insert Guest Additions CD image". This should trigger a pop-up asking if you want to install the software on the disk. You should be using the most recent version of VirtualBox, or this may fail. Reboot once more, and you should have a linux VM with a GUI and the proper screen resolution. You can also set the VM to full screen, and you will have the equivalent of a desktop linux OS. 
