---
title: "My lil' Linux box - Part 2"
date: 2024-03-27T11:16:00-07:00
draft: false
cover: "/img/blog_lil_linux_desk.png"
coverAlt: "My lil' linux laptop - Part 2. Going old school with Window Maker on Linux Mint 21.3."
coverCaption: "Going old school with Window Maker on Linux Mint 21.3"
description: "I still had some more research to do before I flashed my firmware. At this point, all I knew about the Chromebook was that it was small, lightweight and manufactured..."
---

I still had some more research to do before I flashed my firmware. At this point, all I knew about the Chromebook was that it was small, lightweight and manufactured by HP.  I was still uncertain exactly what the specs were or even if after flashing the firmware, would it be worth the effort to install linux on it (due to not knowing the hard drive/SSD size). I just really knew it was possible.

So back to the interwebs to search for information to determine the model and and hard drive space from within ChromeOS. 

“In ChromeOS open your Chrome browser and enter chrome://system and press enter. On the “About Chrome Page” just press Ctrl+F and search for “model_name”. It will scroll down and show you the model name of the Chromebook.” I now had the model name. Which of course led to more searching of the interwebs. Fairly quickly, I worked out that I had an HP Chromebook 11 G6 EE with an Intel Celeron N3350 processor and Intel HD Graphics 500. It definitely was the “Snappy” model. However, this did not make the Chromebook a powerhouse, but it would suffice. Checking via the Files app in ChromeOS, I was able to piece together that the Chromebook had between the used and unused space, a whopping 32gb to play with.

Not a lot, but better then the 16gb model. 

Now that I knew I had more space to play with, I could’ve gone with a simple, lightweight distro like PuppyLinux, TinyCore or a few others to conserve hard drive/SSD space. All of them equally good. But I decided to cut the other way, in more of a “for shits and grins, fuck around and find out” I chose a larger Distro. I mean, come on? If wiping your firmware and installing Linux on a Chromebook isn’t the geek epitome of “fuck around and find out” I mean, “What is?” 

My selection criteria for the distro was simple: Stable, with a straight forward install that did not have a track record of breaking easily post install. I had survived a few too many instances of that using Ubuntu. I though that maybe one of the Ubuntu derivatives might work. At one point I thought about even maybe installing a striped down version of Debian. Eventually, I settled on Linux Mint an Ubuntu derivative, mostly because I was already familiar with the package manager (apt) and everything that I read about it indicated that it was:  

> - Rock solid enough to be recommended to Linux newbies and experienced users alike.
> - Was well thought out in terms of being a very complete and curated distro with a good selection of open source software as part of the install.
> - Has a reputation, that once installed, you will have a stable, complete OS, ready to go.   

Distro selected, I proceeded to update the firmware. Once that was completed, I could solely focus on installing Linux. A half hour or so later, I had Linux Mint on my Lil’ laptop. I actually had a geek-gestalt moment. My gawd, it worked! More to the point, it went smoothly. 

#### Modern problems require modern solutions

Again, with this set up there were still things I had to take into consideration. My hard drive/SSD was tiny to begin with. Installing Mint had reduced the space to a little under half.  With the hard drive/SSD soldered onto the motherboard, and Chromebooks basically being glued together, I wasn’t going to attempt to take it apart. I had a couple of external hard drives, I could simply just use them via the USB ports. But that meant lugging additional peripherals and cables and such. Which kind of defeated the portability of said laptop. I wanted something a little more practical, dare I say it “elegant”. It was then I decided I would simply buy a microSD card and slap that right into the microSD slot. A day or so later I picked up a microSD card with 512gb. The storage space was solved. Well, sort of...

I’ll try to explain this as simply as possible. Basically, your Home folder on any computer is where your personal folder resides, with your personal files, your music, your videos, you pictures of Na-Na at G-Ma's b-day. Plus it’s where hidden files and folders holding your personalized settings reside. Overtime your personal folder grows in size. I knew that this would be true in my case and very quickly would overwhelm the space on the internal hard drive/SSD. Another consideration was all OS’s have log files, literally files that log the health of the system. This can also grow and impact space as well.  So, I really wanted to keep as much of the internal hard drive/SSD free, while using the microSD card as storage.

Luckily, Linux has a solution for that. In short, you basically move your personal folder within the Home folder to the external drive you want it on (in this case the microSD). Think of folders as being the branches to a tree that attach to a root. All you really are doing is telling your system that this branch (the location of the microSD card) now contains your personal folder and should be mounted (attached) to/inside the Home folder on root. So, when you boot the next time, it automagically mounts the microSD inside of the Home folder and assumes this your personal folder. You can learn how to do this [here](https://www.howtogeek.com/442101/how-to-move-your-linux-home-directory-to-another-hard-drive/).

Once I did the above, I now had plenty of space for personal stuff, leaving the internal hard drive space alone.

Another consideration was log files for the system. The log files reside in another folder on the root called “var” short for “variable”, in var is a folder called log, in the log folder is the aforementioned log files. Since it is not recommended that you delete your log files as it could cause bad voodoo to your system, the simple solution for me was a script that basically zeroed out all the files to having zero bytes. Thus keeping the log files from taking any space. I knew that if something went wrong, it meant I would be limited in my ability to diagnosis the issue via the log files. But at the end of the day I went with it. Logically, once my personal folder was moved to the microSD, the entire system could go up in smoke for all I cared. All I would have to do is re-install the OS and re-attach the personal folder to the Home folder on root and I’d be set to go. So, the log files while needed for the OS, where not that big of a concern.

Also, it bears mentioning that with microSD cards, they can burn out. So, back up you personal folder on the microSD card as a precaution. My microSD is still going strong, but your mileage may vary. I back up about once a month.

The last thing to keep in mind is that the big major updates, not the day to day incremental updates and patches that Linux Mint releases. But, the major version number updates/releases will not be possible from within the updater with a tiny internal hard drive/SSD. They are dependent on the internal hard drive to have a vast amount of space so the updater has room to basically update the system. So, again having your personal folder on a separate drive makes sense. Usually, I just make a new Live install USB with the new version of Linux Mint on it and reboot off it and do a complete re-install, then re-attach the personal folder to Home again. Added bonus, since my personal folder on the microSD has all those hidden files/foldes/settings already within, I do not have to reconfigure my system to my personal likings.

So for the last year using this setup, has provided me with a solid, great little Linux box to tinker with and get reacquainted with Linux. I've used it as a daily driver for awhile with no issues, I've also used it to build the blog you are reading, (the original repo was hosted on it.) All the images and coding was done on it. So, it’s been quite useful. It's pretty much handled anything I've thrown at it.  

Currently for DE’s I run the default Cinnamon DE included with Linux Mint, plus being a gray beard I also run Window Maker, (yeah, I know … okay, boomer) which I’ve lightly riced to my personal liking.

After spending the last 10 years dividing my time between MacOS and Windows, this whole process has been a great way to get back into Linux and the Linux community. And, yes, it’s really good to be back hacking away.

Places to learn more:

[https://mrchromebox.tech](https://mrchromebox.tech)  
[https://www.reddit.com/r/chrultrabook](https://www.reddit.com/r/chrultrabook)  
[https://docs.chrultrabook.com/](https://docs.chrultrabook.com/)  


-- E’nuf said, Love and Rockets

{{< chat cactus-comments >}}





