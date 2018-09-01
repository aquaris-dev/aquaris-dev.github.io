---
layout: post
title: Device Status &ndash; September, 2018
category: blog
excerpt: Current status of bq Aquaris devices on LineageOS
author: brinly
---

Hello all and welcome to the September aquaris-dev team update of 2018,

Another 2 months has passed really quickly (Wow!, it's September 1st already), with big news this month. We missed a July and August update, but we were hard at work regardless. We won’t cover the stats this time, but you can see the stats of how popular our BQ devices are by checking on the LineageOS [stats](https://stats.lineageos.org) site.

If you like to read more regular news on this website, please consider joining the team as a [developer](/contribute.html).

Our BQ device news now
-----------------

This month, we have some news about several devices, but _bardock(pro)_  is the main star this month. We did some maintenance fixes for our older devices. We added some minor updates to our website too.

So let’s start!

We'll look into at supporting our devices with Android 9.0 at some point, but we want to get a stable base on 8.1 as the versions are very similar so bringup work between 8.1 and 9.0 is minimal especially on the newer devices.

Aquaris X / Aquaris X Pro - Status (bardock/bardockpro)
----------------------

We reached weekly [official](https://review.lineageos.org/#/c/LineageOS/hudson/+/216085/) status for both bardock and bardockpro devices for the LineageOS 15.1 branch recently - they should receive builds each Monday. 

We're going to require 2.0+ (Android 8.1) firmware/bootloader/radio/TZ to flash LineageOS as our drivers need the latest base firmware to function correctly (Baseband, Encryption, Camera, Wi-Fi, NFC won’t work on N based firmware).

Developers interested in helping out - feel free to submit patches to the LineageOS project's gerrit as that is now the official repo for this device for LineageOS..


BQ Aquaris U/U+  - Status (chaozu/tenshi)
-------------------------------
We just started the bring-up work to 15.1 on these msm8937-common devices but this is still very much a work in progress project. Feel free to jump into Slack if you are a developer with contributions to make.


BQ Aquaris X5 Plus  - Status (gohan)
-------------------------------
We [fixed](https://review.lineageos.org/#/c/LineageOS/android_device_bq_gohan/+/226349/) a bug affecting NFC payments via Android/Google Pay after finally tracking down a fix to a long standing JIRA issue. We will start the LineageOS 15.1 bring-up pretty soon (you may already know but it’s based on the MSM8976 chipset which is a strange platform to work on).


BQ Aquaris M5/X5 - msm8916 devices - Status (piccolo/paela )
-------------------------------

One contributor [“aymende7”](https://review.lineageos.org/#/q/owner:aymenbousselham%2540gmail.com+status:open,75) has done a whole bunch of work for bringup of these devices and patches are on LineageOS gerrit, we are reviewing these changes and planning to get this merged for weeklies soon. Feel free to check out his excellent work and jump into slack if you have contributions.

BQ Aquaris X2/X2 Pro  - Status (zangya/zangyapro)
----------------------------
Bringup has just started, but we have a lot of work to do and are mostly making sure that the older devices are supported first. We'll be opening up our device trees soon (hang around Slack if you're interested). It should be a well supported device because it is a new well supported "Treble" platform..

Website
----------------------
We added a slack invite button to the bottom of our site if you’d like to join our Slack community and we also added a PayPal link (if you’d like to support us - we receive no funding from BQ or anybody else and do this entirely as volunteers at our own cost ). We also have a downloads page.




Open Issues
-----------

If there are any issues with any of our supported devices, please report a bug on the [LineageOS issue tracker](https://jira.lineageos.org/) and we'll look into them ASAP (feel free to mention them on slack to get our attention)..
		
                               
