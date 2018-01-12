---
layout: post
title:  "Linux Photo Editing Workflow"
date:   2013-12-12 08:43:59
author: Eli
disqus_disabled: false
categories: Linux Photography
---


##### This is an archive of a post from my previous website.  I am reposting it here with some updates.


Photography is a hobby for me, but like most of my hobbies, I am not one to skim the surface.  I tend to learn as much as I can to become proficient in those things I enjoy.  While not an expert in all things photography related, I have had many conversations about cameras, techniques, photo editing, and anything else photography related.  I am also a bit of a Linux geek.  I have even talked to a number of people about Linux as it relates to photography, but that is nothing compared to the amount of time I have spent on Google, on forums, or talking to other Linux geeks trying to figure out how to make things work properly.  I thought it was about time I gave back to the community by placing some of my solutions online where they would be searchable by other photographers using or considering a switch over to Linux.  When I first started trying to use Linux for my photography, I ran into many problems, but it has gotten much easier to work with as the OS has matured.  Most of my experience has been with Debian based OS’s, so my advice will be understandably [Ubuntu](https://www.ubuntu.com/)/[Linux Mint](https://linuxmint.com/)-centric, but most of this should still be applicable to [Debian](https://www.debian.org/), [Fedora](https://getfedora.org/), [openSUSE](https://www.opensuse.org/), [Arch Linux](https://www.archlinux.org/), [Gentoo](https://www.gentoo.org/), or whatever Linux flavor you prefer.  Many of the programs I recommend have also gone cross-platform, so much of this advice will be applicable to [Windows](https://itvision.altervista.org/why-windows-10-sucks.html) and [Mac](https://www.infoworld.com/article/2940860/mac-os-x/microsofts-quiet-campaign-to-undermine-the-mac.html) users as well.

#### My Linux story:

First a little background…  I am not a super computer geek.  I am not a programmer and I rarely write code.  I can work with the command line if I need to or have a good reason to, but I generally prefer a nice GUI.  I am, however, open to trying new things.  A friend in college first turned me on to Linux in late 2003.  Windows 95 was sucking pretty bad (was it ever good), and my friend offered to install Fedora Core 1/Red Hat 9 for me.  We backed up all my files to an external HDD (not too hard since I only had a few Gigs of data at the time), installed the new OS, put all my files back on my computer, and I was a happy camper.

A couple years later I got a new computer and it came with Windows XP.  At the time, I had no experience installing Linux by myself, and it was more hassle to wipe the computer and start over than to just use Windows, so I stuck with what I had.  I upgraded computers again, and again just used what it came with.  Well, as is inevitable with windows, the spyware, Trojans, and viruses stacked up, and my computer screeched to a halt.  It was early 2008 and one of my roommates at the time was running Ubuntu on his laptop.  He said I should give it a try, and having someone else around who was knowledgeable in the OS, I decided to give it a go.  I downloaded the Ubuntu 7.10 (Gutsy Gibbon) ISO, burned it to a CD, backed up my files, and said F.U. to Windows.  I played with it for a couple months until 8.04 (Hardy Heron) came out, did a clean install, and rocked that for a while.

It was around this time, I started to get into photography.  I was having some issues with not being able find the programs I needed to manipulate the images the way that I wanted.  I was also having trouble getting dual-screens to work with the 26″ monitor I had bought for photo-editing, which was a bit of a deal-breaker, so I sold that computer and got an iBook G4 because I heard they were great for photo editing (also, one of my other roommates who repaired Mac laptops gave me a good deal).  After using OS-X for a few months and having nothing but frustration, I decided to go back to Linux.  I sold the G4, bought another laptop, wiped Windows and installed Ubuntu 8.10 (Intrepid Ibex).  Fortunately 8.10 included some critical updates, and I was able to get the dual-monitors working (after plenty of frustration of course), so I was in business.  Since that time, I have built numerous computers, installed numerous variations of Ubuntu/Debian/Mint, tried more programs than I can remember, and learned many lessons along the way.

#### When to upgrade your OS:

The first lesson I would like to stress as a photographer is don’t be in a rush to try to latest-greatest version of the OS.  Unless you have a specific reason to upgrade (such as a program that is only available for the latest OS), then stick with the LTS releases, and upgrade every two years instead of every six months.  Your computer is a tool that you want to use to edit photos, not something you want to spend all your time upgrading.  Once you have a good workflow, you can focus on the art without having to learn the technical details of how to do what you want.  Any time you update your OS or your photo-editing programs, there is always a chance that something will break.  It’s better to stick with what you have than to spend time fixing it, or even worse, having to change your work-flow because some program you use no longer works properly and you have to find a different program for that purpose.  By all means, do the security updates and update those programs that interact with the web (browser, email, ftp client, etc.), but unless it’s broken, leave it alone.

#### Which version of the Linux OS:

~~I am currently running Linux Mint 13 MATE Edition (which is based on Ubuntu 12.04 Precise Pangolin).~~  I switched over to [Mint](https://linuxmint.com/) because I hate the Unity desktop environment and Gnome 3 shell only sucks marginally less IMHO.  [Linux Mint](https://linuxmint.com/) absorbed the Gnome 2 project under the new title of [“MATE”]() and is maintaining and updating that desktop environment, for which many people are grateful.  While it is nice not having to install all the codecs and such every time you install a new OS, the main reason I went to Mint is the Gnome 2 desktop.  This comes with its own issues, and I will probably be forced to move to Gnome 3 eventually, but it’s working for now, so I’ll take it.  If you don’t mind Gnome 3 shell or actually like Unity [*gasp*], then Ubuntu is a perfectly good option. **2017 update: apparently I am not the only one who thinks [Unity sucks hard](https://insights.ubuntu.com/2017/04/05/growing-ubuntu-for-cloud-and-iot-rather-than-phone-and-convergence/).  Looks like Ubuntu is abandoning Unity in favor of Gnome 3, which is exactly what Mint did years ago.**  [Debian](https://www.debian.org/) or [LMDE](https://linuxmint.com/download_lmde.php) are great for people who need a very stable OS or have a computer with limited resources such as a netbook, but as a photographer, sometimes you need programs or libraries that are not available in the Debian repositories, so that has the potential to cause problems.  There are any number of other Linux OS’s out there (all good in their own ways), but not having much experience with any of them as they relate to photography, I will avoid further comment and leave you to try whatever you want (but that’s the nice thing about open source – you have the ability to try anything you want, and it’s all free :-)

**2017 update: now running Mint 17.3 [Cinnamon](https://en.wikipedia.org/wiki/Cinnamon_(software)) on my photo-editing machine and it's been great.  I switched over from MATE to Cinnamon a couple years ago, and everything just seems to work better with Cinnamon.  I must also commend the Mint Development Team for moving to LTS-only releases.  No one wants to be forced to upgrade their OS every six months.**

#### Calibrating your monitor:

One of the first things you are going to want to do as a photographer is to calibrate your monitor.  You will need some hardware for this, but fortunately you can get that hardware for a much better deal than you could less than a decade ago.  Color calibration tools used to cost several hundred dollars, but there are now several good options at reasonable prices.  Personally, I have a Pantone Huey because it was the only reasonably priced option available when I started all this, but there are several good options out there these days that should work fine with Linux.  As far as software, if you are running Gnome 3, you can use [Gnome Color Manager](https://github.com/GNOME/gnome-color-manager) to create an ICC profile for your monitor-videocard combination.  Before Ubuntu moved away from Gnome 2, it used to work flawlessly, but under MATE I had issues with it.  **2017 update: Gnome Color Manager seems to work flawlessly under the Cinnamon desktop.**  There is also another option called ~~DispcalGUI~~ [DisplayCal](https://displaycal.net/) which I have used before and had success with.  **2017 update: in addition to changing the name, it looks like the program has matured significantly, so if GCM doesn't work for some reason, defintiely give DisplayCal a shot.**  You also have the option of using the back-end for both these programs directly: [ArgyllCMS](https://www.argyllcms.com/).  Argyll is cross-platform, so if you are moving from Mac or Windows, there is a good chance you have already used this program.  All these programs should be available under your distro’s repositories, but if not or you need a different version, they are easy enough to find.  The third option, if you are running a dual-boot machine, is to simply calibrate the monitor under your other OS and import the ICC profile into Linux.  However you decide to do it, once you have your monitor properly calibrated, you should not have to re-calibrate for some time.  The color response on monitors can change over time (its a hardware problem, not a software problem), so it’s generally recommended that you re-calibrate every so often… when you upgrade your OS every two years or so seems to be a good time.


#### Getting photos off your cards:

As a photographer, you are probably all too familiar with downloading the photos off your SD or CF cards before you start sorting and editing.  This can either be a simple or complicated task depending on how you go about it.  One program that I use is [Rapid Photo Downloader](https://www.damonlynch.net/rapid/). I initially tried this program because I ran across it and thought "why not?"  I did not think much of it at the time, but now I don’t know how I managed without it.  This program allows you to download all the files from your cards, re-name them using any number of criteria, save them to a folder, and many other abilities as well.  It simply automates an entire process, saving you time and effort from something so mundane.  I rename using date and time so that my photos get organized chronologically, even if I am using two cameras.  I also have it unmount the card once it is done, which is a nice feature, especially if you have several cards you need to download from, it just saves you one more step.  There are too many features to list here, but suffice to say that I am a big fan of this program and highly recommend it to anyone using a digital camera.

#### Sorting your photos:

As any photographer knows, sorting through all the crap to find the good images is one of the most time-consuming tasks.  There are any number of programs available for this (including gThumb, Geeqie, F-spot, etc.), ~~but the one I use is [FastStone Image Viewer](http://www.faststone.org/FSViewerDetail.htm).~~ It is a program I found back in my windows days (I think I first started using it in version 1.x), and I still have not found anything that matches the functionality that this provides for the purposes of sorting through all your photos.  It is a Windows program (freeware, but not open-source), but every version I have tried runs just fine under every version of WINE I have ever tried, so I don’t feel bad for including it here.  I can easily view and scroll through my RAW images using the arrow keys on they keyboard, view images full-screen by pressing the Enter/Return key (you can scroll through images in full-screen view), and delete images by simply pressing the Delete key (even in full-screen view).  Using this program, I can sort through a couple hundred images in only a few minutes, easily deleting all the images that are out of focus or just plain crap.  With subsequent passes, by toggling back and forth between photos that are similar to each other, I pick the best few images and delete the inferior ones.  In very little time, I can have a large collection of photos narrowed down to just the best ones before I even start messing with them.  There are some glitches here and there, and not everything works flawlessly under WINE, but for the simple purpose of sorting though your RAW photos, it’s fantastic.  It works just fine on Linux via WINE, and it will obviously work on Windows, but considering that WINE is also available for OS-X, I think this is a tool that every photographer would benefit from, regardless of what OS you are using.  I am hopeful that one of the native Linux programs can eventually provide the same functionality, but for now this works just fine.

**2017 Update: I finally found a native Linux application for sorting photos! [XnView MP](https://www.xnview.com/en/xnviewmp/) is a fantastic program that does essentially the same thing that FastStone I.V. did, but without all the glitches associated with running under WINE.  It too is FreeWare (for private, educational, or non-profit use), not Open Source, but I'll take it.  If you make money with your photography, you need to buy a license, but the licenses are relatively cheap.  It's also available in Linux, Mac, or Windows, so you have no excuses.  The ability to scroll through RAW photos, in full-screen mode, using the arrow keys, and easily delete the crap photos is just essential for a good workflow.  This fits the bill perfectly!**

#### Adjusting your Photos:

These are probably the programs that photographers are most familiar with.  These are the Lightroom-type programs for adjusting the values on your raw files before you export to JPG/PNG/TIF.  Unfortunately the good folks at Adobe like to embrace their inner duchebag by refusing to port Lightroom (or Photoshop) to Linux, so that is not an option unless you can get it to run under WINE, on a virtual Windows machine, or on a dual boot machine.  You could also try installing the software that came with your camera under WINE, but this is usually pretty buggy.  I shoot with Canon, and for years I used an older version of Digital Photo Professional that came with my Rebel XTI because it still worked better than anything at the time, but I have since moved to native applications because they are more stable.  I tried using [UFRaw](http://ufraw.sourceforge.net/) (it also works as a plugin for [GIMP](https://www.gimp.org/)) for a while, but at the time, the adjustments were not all that great, so I looked elsewhere.  I’m sure it has improved (that’s what open-source does after all), but I have found other programs I like better and see no reason to change.  One program worth mentioning, even though it is closed-source and will cost you money, is [Corel AfterShot Pro](http://www.aftershotpro.com/en/products/aftershot/pro/) (formerly Bibble Pro).  I started using this after I moved away from Digital Photo Professional, and it seems pretty good ~~(I still use it)~~, but considering the quality of some of the open-source options these days, it might not be worth the money when you can get something comparable for free (I would like to commend them for porting it to Linux though).  Another option that I tried way back in its infancy and seemed pretty promising is [RAW Studio](https://rawstudio.org/).  I heard that it has come a long way, but have not tried it, so I can’t comment further.  The program I currently use is [RAW Therapee](http://rawtherapee.com/).  This program used to be closed-source until the source-code was released under the GPL in 2010, and has since become the favorite of many photographers on all OS’s.  I can highly recommend this program, regardless of what OS you are running (since it runs on all of them).  All these open-source programs should be available under your distro’s repository.  With several good open-source options, there is little reason to go with a closed-source program for adjusting your RAW images.  Adobe Lightroom can suck it.

#### More advanced image manipulation:

Like I said earlier, you are not going to find Adobe Photoshop running well on Linux under WINE, so unless you have a dual-boot machine, you are better off with some of the native options.  The go-to program in Linux for more advanced photo editing is typically the [GIMP](https://www.gimp.org/).  It does most everything you need it to, and if it doesn't, there is probably a plugin that does.  It’s been around forever, simply because it’s such a great program and there’s not much else like it.  It’s also cross-platform, so you can use it on every OS.  ~~Unfortunately GIMP can only handle 8-bit images, so if you really need to work with 16-bit or greater, a program to consider is CinePaint.  While not as mature as GIMP, it is still a great program and well worth having around.  Getting it installed and working can be a bit challenging (especially finding all the dependencies), but once you do it works well.~~  **2017 Update: As of version 2.9.2 (released 2015) GIMP now supports greater color depth, so you can use 8, 16, 32 (32 is native), or even 64 bit for those scientists analyzing telescope data. Since CinePaint was essentially just a fork of GIMP with greater color depth, there's really no reason to use CinePaint anymore.**   

For stacking images from a bracketed exposure, you should check out [Luminance HDR](http://qtpfsgui.sourceforge.net/?page_id=10) (formerly QTPFSGUI).  It works well and gives you many options in both creating the HDR and tone-mapping it back into a LDR image, which is what gives you the cool effects.  **2017 Update: It now supports RAW formats, so you don't have to convert into TIFF first, which will both save you a step and give you higher quality finished images.**  

If you need to stitch some photos, edit perspectives, or do some focus stacking, your tool of choice is going to be [Hugin](http://hugin.sourceforge.net/).  You can stitch vertically, horizontally, or even tile several images to make one large one.  You can do perspective corrections such as to remove or simulate a fisheye effect, give a tilt-shift effect, or even skew your photos for artistic effect.  If you are into macro photography, you are going to love the ability to focus-stack your images, giving a final image with the entire subject in focus where you might normally only get 0.1mm DOF. There is also a program called [Enfuse](http://enblend.sourceforge.net/), which can be used through Hugin, and allows for some HDR-like effects without actually creating an HDR.  I’m sure there are many other good programs I'm missing, but these are my typical bread-and-butter.

#### Watermarks, resizing, reformatting, etc.:

Once you have your images the way you want them, then comes the tedious task of re-formatting them, re-sizing them, adding watermarks, and applying any kind of boarders or effects you might want before you post them on the web, print them, send them to clients, or whatever you are going to do with the photos… or you could just use [Phatch](http://photobatch.wikidot.com/). Phatch is a nice simple program that does all that stuff that would have taken you hours to do to each individual photo and does it with just a couple mouse clicks.  You can save different action lists for everything you might conceivably want to do to your photos, then all you have to do is open the appropriate action list, select a folder or file(s) you want converted/watermarked/etc., and it does everything for you, even saving them in a sub-folder to keep you nice and organized.  This program uses quite a few powerful command-line tools as the back-end, but makes them all nice and user friendly with an ultra-simple GUI.  I started using it back when [Stani](https://en.wikipedia.org/wiki/Stani_Michiels) was first developing it and you had to get it though his PPA, but it is now a mature program and widely available in the main repositories.  It is also cross-platform, so you can use it on any computer, regardless of OS.  I really can’t say enough good things about this program, and if you aren’t already using it, you are missing out.

#### Backing up your files:

Now of course spending all this time editing your photos would not be much use without a good backup solution to make sure you still have a copy ~~if~~ when your hard-drive dies.  There are numerous fantastic backup solutions available for Linux, but the one I use the most is [Grsync](https://sourceforge.net/projects/grsync/).  It is simply a user friendly front-end for the powerful back-end command line tool rsync.  It works on a file-system-level, so it’s easy to back up your whole computer, just the folder with all your photos, or backup one external HDD to another HDD.  It’s also incremental, so you can easily do a quick backup after every photo-editing session, and unlike drag-and-drop, it won’t be a major pain if there is an error midway through.  Looks like it is now cross-platform too, so that is good news for the Mac and Windows users as well.

That’s about it.  Please let me know if there are any programs you particularly like using in your photo-editing routine, or if you have any suggestions.
