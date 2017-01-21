---
layout: post
title: Device Status &ndash; January 21, 2017
permalink: 2017/01/21/device-status
category: blog
excerpt: Current status of BQ Aquaris devices on LineageOS
author: stucki
---

Hi folks! 

thanks for coming to our new website which we have just recently started for you! Our aim is to inform about the availability of LineageOS for various BQ devices, and give you the latest info about the status. 

In this first report, we like to give you an overall update of the things that are going on about LineageOS right now. 

LineageOS Status
----------------

As you might know, the new project "LineageOS" has been started to replace the great CyanogenMod project which is now discontinued. The new project can be considered as a friendly fork, therefore almost all developers who worked on CyanogenMod are now also working on LineageOS. This is good news for you as a user. Only a few things change, the most remarkable of it being the new name for you to remember… 

Although the LineageOS project was started only a few weeks ago, it is already in full swing today: Take a look at the latest blog post which was published earlier this week that gives an update from the LineageOS developers: [http://lineageos.org/Update-and-Build-Prep/](http://lineageos.org/Update-and-Build-Prep/) 

The Gerrit Review system (the place where most of the development happens) is already live and receiving lots of contributions for LineageOS. Most (if not all) devices have been rebranded to the new name, and so have we done. You can check the latest changes for all BQ devices here: [https://review.lineageos.org/#/q/project:%255ELineageOS/android_.*_bq_.*](https://review.lineageos.org/#/q/project:%255ELineageOS/android_.*_bq_.*) 

Meanwhile, some big parts of the infrastructure are still missing. Most notably, there are no releases yet. We can’t give you an ETA right now, but rest assured that they will come as soon as possible… 

IMPORTANT: Unfortunately, there are currently a few sites which try to mislead users who are impatiently waiting for the first releases. Some of these websites provide downloads of CyanogenMod as well as LineageOS. However, be very cautious when using them. These are not official releases and it cannot be guaranteed that the might even include malware. We strongly recommend that you don’t download builds from any of these sites. In fact, only trust the [official website](http://lineageos.org/) (and us, of course…). It will save you time and trouble. 

For more news about the status of LineageOS, please check the [official website](http://lineageos.org/) regularly. 

One of the cool things that are already available for LineageOS is a new stats page. On https://stats.lineageos.org/ you can find download statistics for each device that exists for LineageOS. We like to inform you that it is our goal and motivation to be on the top 25 of that list! Please help us and spread the word… :-) 

Weekly Releases
---------------

As written in the news on [http://lineageos.org/Update-and-Build-Prep/](http://lineageos.org/Update-and-Build-Prep/), there will no longer be daily (nightly) releases. Instead, releases are created once per week. 

Right now, there are no official releases that can be downloaded. However, you can always build your own release from the sources that are publically available. Instructions on building haven’t changed since CyanogenMod (except that the repositories have new URLs), so if you are familiar with this process, it should be an easy thing for you to build LineageOS. 

For all other users, we will publish a documentation on how to make your own build at a later time on this website… 

Issue Reporting
---------------

Right now, there is no common issue tracker for the LineageOS project. That means that upstream bugs cannot be reported yet. 

Meanwhile, we used to have our own issue trackers for device specific issues. They are currently missing too but will be up again later this week…

Known Issues & Next Steps
-------------------------

### BQ Aquaris M5 (piccolo)

* This device will soon get official releases by LineageOS.
* cm-13.0: This version builds fine and has no known issues. However it won’t get a new release with LineageOS.
* cm-14.1: This version builds fine. There are currently some issues which are known and have already existed with CyanogenMod in version cm-14.1:
  * Data connectivity is broken after leaving a Wireless LAN. If you don’t get any mobile connection, a restart of the phone is currently needed.
  * AGPS is still broken.
  * The Camera is not fully functional.

### BQ Aquaris E5 LTE (vegetalte)

* This device will soon get official releases by LineageOS. Again, no new cm-13.0 release will be published.
* The device uses the same repositories for kernel and common modifications like the Aquaris M5. Therefore, it works just as good as piccolo does.

### BQ Aquaris X5 (paella)

* This device will soon get official releases by LineageOS.
* Currently, the device will still get cm-13.0 instead of cm-14.1.
* We are soon going to use the same repositories for kernel and common modifications like the Aquaris M5 and the E5 LTE. From then on, the device will work just as good as piccolo and vegetalte do (applies to both releases, cm-13.0 and cm-14.1).
* (Background notice: There used to be two projects for this device in the past. One was developed with the device codename "paella" which was based on the X5 CyanogenOS edition. Paella was officially supported also for CyanogenMod and is the codename which was better known for this device. However, work on this tree has stopped. Meanwhile another project used the codename "picmt". It was based on the stock ROM that is released by BQ and was not officially supported by the CyanogenMod project.)
* Although the CyanogenOS edition for the X5 is officially discontinued, we will continue to support this device with LineageOS. The device name in LineageOS will be "paella" for both editions of the Aquaris X5. Most likely, a wipe will be necessary before this device can be used again with LineageOS…

### BQ Aquaris X5 Plus (gohan)

* This device will soon get official releases by LineageOS
* So far, the cm-13.0 branch builds fine. Many things work, the speaker (and probably more things) is currently broken with cm-13.0.
* The project can be built from sources and will boot. Right now, many things work, but there are still lots of issues. At the moment, cm-13.0 still works better than cm-14.1, however new updates are only made for cm-14.1 right now.
* We currently do not recommend that you use this version for daily use.
* If you know what you’re doing, feel free to give it a try and help us to get the remaining issues fixed. We are looking forward to your contributions…!

### BQ Aquaris M5.5 (namek)

* This device is currently work in progress. We have started a port just for the fun of it. We currently don’t know if we are going to provide regular releases (unofficial or official) for this device. This means that you need to build it yourself from the sources (on our github).
* At the moment, only cm-13.0 is available and can be built from sources. According to our member Kra1o5 the build is running just fine.
* A port for cm-14.1 is not available yet, but you may want to try that yourself and let us know about your work… :-) (submit your changes upstream to us)

### BQ Aquaris U Plus (tenshi)

* This device is currently work in progress. We have started a port just for the fun of it. We currently don’t know if we are going to provide regular releases (unofficial or official) for this device. This means that you need to build it yourself from the sources (on our github).
* So far, there is only a branch for cm-13.0 (because this release is more mature at the moment). However, at the moment this branch does not run without a lot of hacks, so leave your hands from it unless you know what you’re doing. (Nevertheless, we are looking forward to your contributions!)
