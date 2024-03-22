---
title: "My lil' Linux box"
date: 2024-03-21T11:52:06-07:00
draft: false
framed: true
cover: "/img/lil_linux_laptop.jpg"
coverAlt: "My lil' linux laptop'"
coverCaption: "Chromebook no  more"
description: "Not too long ago I was offered a free Chromebook that a friend had no use for. I gladly accepted it, then placed it on shelf for a while, not really knowing what to do with it. I already had a... "
---

Not too long ago I was offered a free Chromebook that a friend had no use for. I gladly accepted it, then placed it on shelf for a while, not really knowing what to do with it. I already had a few options for daily driver’s, both running both Mac OS. Since I really had no desire to run ChromeOS, mostly because it’s Google and dependent on Google for well, everything. It sat, forelorn on a shelf of  
good intentions.

But, I did feel compelled enough to boot it on occasion and at least mess around with it enough that I liked its lightweight, compact size. I just did not like the thought of being locked into another closed ecosystem as I already had that with my Mac’s, and what I could barely forgive with Apple,   
I wasn’t prepared to do so with Google.

So, if I was going to do anything with this notebook I wanted it to be able to do more than just email and casual web browsing. I knew ChromeOS was a fork of Linux so, I explored my options. I could use Crostini but I wanted more than just a terminal and a few developer tools running in ChromeOS, I could use chrx and dual boot ChromeOS and Linux, but that just seemed a silly waste of hard drive space and as we all know, hard drive space on a Chromebook is king. I could simply run Linux apps within ChromeOS which you can do now, but that meant running them while still being locked into Google’s ecosystem. All of these options felt limited and well clunky.

What I really wanted was a straight Linux install with no sign of ChromeOS. So, off to wilds of the interwebs. It didn’t take me long before I stumbled upon GalliumOS.

At this point I should mention there are some caveats about installing Linux on a Chromebook. 

>**First caveat** - Most Chromebooks come with SSD’s that are soldered to the motherboard and have just enough room for an OS and not much more, as such, you can not just swap out the SSD for something larger. 

My Chromebook came with a 32gb hard drive, the average Linux install with a usable desktop weighs in anywhere from 4gb to as high as 30gb depending on what distro you install. It’s a good idea to research the size of the average install for the distro you about to choose before installing it on a Chromebook.

More on this later, but be aware of storage space.  
(And, yes I'll discuss some of the other finer points in my next posting on post-install).

>**Second caveat** – you are about to update the firmware/UEFI to allow Linux to boot on a Chromebook. If you mess this up, your Chromebook will be toast, as in an un-bootable brick. Only do this if you feel you are well versed on this and have read the documentation. I take no responsibility for what happens if you mess this up. 

After some poking around (as mentioned before) I found GalliumOS, a fast and lightweight Linux distro for ChromeOS notebook/laptops. Unfortunately, there was this disclaimer 	at the top of the documentation: 

>**IMPORTANT**: Development on GalliumOS has been discontinued, and for most users, GalliumOS is not the best option for running Linux due to lack of hardware support or a kernel that's out of date and lacking important security fixes. 
>
However directly below that show stopper was this bulleted list:
  
>For most (EOL) Chromebooks, the recommended path forward is to.  
> - put the device into Developer Mode
> - disable firmware write protection  
> - flash MrChromebox's UEFI Full ROM firmware  
> - install ChromeOS Flex, Linux, etc.  
>  
>See [https://mrchromebox.tech](https://mrchromebox.tech/) and the [chrultrabook subreddit](https://reddit.com/r/chrultrabook) for more info.

I felt a little uncertain, but read on. What I basically could piece together was that development stopped somewhere around 2017 for Gallium OS. But that the documentation, the steps to actually flash the firmware/bios//UEFI still worked.
> - put the device into Developer Mode
> - disable firmware write protection  
> - flash MrChromebox's UEFI Full ROM firmware  
> - install ChromeOS Flex, Linux, etc. 

The last bullet point basically is saying once you’ve flashed the UEFI, you can install any Linux Distro by booting off a USB installer just like you would with any normal install and proceed from there, provided your firmware was supported and flashed first.

In my case the first two bullet points where not an issue. The second bullet point will vary depending on your Chromebook. 

The first step is to ID your Chromebook by processor name and see if it’s compatible for Linux, go here: [https://wiki.galliumos.org/Hardware_Compatibility](https://wiki.galliumos.org/Hardware_Compatibility) Once this page listing loads, locate your model name on this page, since I have a HP Chromebook 11 G6 EE. I simply did a find (Crtl+f) for my model, which identified my processor as “Snappy” which meant my computers processor is an “Intel Apollo Lake.” (Reading across the row for my model.) Click on the note ”Required[2](https://wiki.galliumos.org/Hardware_Compatibility#cite_note-Firmware-2)” this will link to the bottom of the modle listing page, under “2. Firmware Update” at the end of the sentence click on the "Firmware" link which will lead you to this page [https://wiki.galliumos.org/Firmware](https://wiki.galliumos.org/Firmware) at the bottom of this page, under “notes”, is the link to the actual instructions for your processors firmware, select “[Easy Install via the Firmware Utility Script](https://mrchromebox.tech/#fwscript)" then follow the instructions on the Mr.ChromeBox page and via curl on the command line under ChromeOS update the firmware according to the instructions outlined.

Basically after updating the firmware, reboot with/from your install media and install the linux distro of your choice. Good-bye ChromeOS, and Hello Linux!  


\- E'nuf said, Love and Rockets 

##### *A sidenote to above, there have been changes to ChromeOS that may have made this more difficult than I originally encountered when this was written. I offer this as the steps that I took a little over year ago with the intention of posting it back then. Due to site issues, I was unable to post this a year ago. So, definetly start with these two links: [https://mrchromebox.tech](https://mrchromebox.tech/) and the [chrultrabook subreddit](https://reddit.com/r/chrultrabook) for more up to date info.*



