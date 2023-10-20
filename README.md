# [Ubuntu Dual Boot](https://youtu.be/uqZIp4ay-3s?si=hGYDFGRALi4ozBev)
Windows 11 and ubuntu dual booting procedure 

1) download [ubuntu](https://ubuntu.com/download/desktop) lts .iso file. (aprrox 4.7Gb)
2) You need to allocate space from memory for the Linux to reside in.
3) Go to start and search create and format hard disc partitions
   
 ![image](https://github.com/manavshah-28/dellInspiron7572_ubuuntu_dualboot/assets/82638448/ee8ce437-2d88-4d85-a735-d5bec529a535)

 4) Shrink a drive and allocate a name to the new space created (linux in my case with around 200Gb space allocated).
 5) You need a bootable drive for this process.

### creating the bootable ubunut drive
 1) Format the pen drive (~8Gb).
 2) Install the [rufus](https://rufus.ie/en/) software. This allows to make a bootable drive
 3) connect your formatted hard drive. It should be visible on Rufus gui.
 4) Select the .iso ubunutu file you downloaded under the boot selection option.
 5) accept defaults and press start.

### booting ubuntu 
 1) Restart your Laptop and press f2 while you see the dell logo, this takes you to the bios settings.
 2) Go to boot configuration and turn of secure boot.
 3) Under storage section of boot configuration deselect Raid on and select AHCI.(newer standard supported on linux).
 4) Now restart device and press f10. This will show you the option to boot from the bootable drive just created.
 5) Install ubuntu and follow the instructions which are prompted by the setup.
 6) Finally you restart and ubuntu is now working.
 7) Now every time you start your computer a grub menu will ask you what you want to use Ubuntu or Windows.

### The problem
When you switched to AHCI from raid on, you broke the windows boot. 

### The solution
1)Shut down your laptop
2)While you start press f2 while on dell logo 
3)Change AHCI back to raid on and windows should start normally
4)Now go to start -> system configutation -> boot-> safe boot.
5)Now restart your computer and press f2 while dell logo dispays
6)under storage section, change raid on to ufie and restart.
7) windows should now start up in safe mode. 
8) now you turn of safe mode by going into tart -> system configutation -> normal startup

![image](https://github.com/manavshah-28/Ubuntu_Dual_Boot/assets/82638448/b864860f-b47b-4970-93c8-d03684eccec7)

Et VIOLA !!
You now have succesfully dual booted your dell laptop with windows 11 and ubuntu.


Removing Ubuntu safely 
https://youtu.be/KwcfzCfkQgc?si=HUq0CO5CTNSUETLm
    


