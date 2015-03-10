# Before You Begin
You will need a few things before you get started.
##A Way to Provision VMs
There are a lot of ways to get the resources necessarry to create and configure VMs. You can buy a dedicated server at a remote datacenter. You can go to NewEgg and order the parts for a spare machine to act as a VM host. You can check the server listings on eBay.... and on and on. The way I learned, and I assume the way many people are learning, is on as little money as possible, which in my opinion leaves the two options detailed below.
####Your Local Computer
If you are hoping to follow along with the tutorials to follow for free (without using a cloud hosting provider), you will need a powerful computer capable of running many Virtual Machines at once. The more processor cores and RAM that your machine has, the more VMs you will be able to create. If you go this route, you'll need to be comfortable creating new VMs with base installs of operating systems.
####An Account with a Cloud Hosting Provider
If you go this route, you will provision new servers in the cloud for a low hourly rate. I like and use[^1]
 * [DigitalOcean](https://www.digitalocean.com/?refcode=d51e7458ca49) (referral link)
 * [Vultr](http://www.vultr.com/?ref=6825035) (referral link)


  They have all kinds of promotions and coupons for free server time - just google around. [LowEndBox](http://www.lowendbox.com) has also been of great help in the past. If you go this route, you should delete VMs after you have configured them so that your money or coupon goes further. If you have a `.edu` email address, the GitHub Student Developer Pack includes a domain and $100 in credit at DigitalOcean. This book is written with this route in mind. 
##A Domain
If you got the GitHub Student Developer pack, you'll get a free `.me` domain name from [NameCheap](http://www.namecheap.com/?aff=83584) (referral link). Even if you didn't get a domain for free, I recommend that you get one from NameCheap or another source. As long as your domain registrar allows you to register your own nameservers, it doesn't matter where you get it. You should have access to the email address provided by WHOIS (which is usually masked by your registrar). Having a domain is key for a lot of system administration topics. Take note that this does not necessarrily have to be a `.com` or `.me`. Whatever domain you can find cheapest is fine.

[^1] I like and use these because they are cheap and have datacenters near me geographically. Choose your cloud hosting provider accordingly.
