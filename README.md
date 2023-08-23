# Ubuntu Dual Boot
Windows 11 and ubuntu dual booting procedure 

1) download [ubuntu](https://ubuntu.com/download/desktop) lts .iso file. (aprrox 4.7Gb)
2) You need to allocate space from memory for the Linux to reside in.
3) Go to start and search create and format hard disc partitions
   
 ![image](https://github.com/manavshah-28/dellInspiron7572_ubuuntu_dualboot/assets/82638448/ee8ce437-2d88-4d85-a735-d5bec529a535)

 4) Shrink a drive and allocate a name to the new space created (linux in my case with around 200Gb space allocated).
 5) You need a bootable drive for this process.
 6) Format the pen drive (~8Gb) an install [rufus](https://rufus.ie/en/) software. This allows to make a bootable drive.
 7) Restart your Laptop and press f2 while you see the dell logo, this takes you to the bios settings.
 8) Go to boot configuration, check ufie before windows boot manager and turn of secure boot.
 9) Under storage section of boot configuration deselect Raid on and select AhCI.(newer standard)


Do them later (after Ubunut is setup)
     //the problem is that windows runs on raid on while linux requires AhCI. So to solve this we install AHCI drivers on windows and then run both OS using that.
) Now go to safe mode to install AHCI driver.
) Open system configuration. 
