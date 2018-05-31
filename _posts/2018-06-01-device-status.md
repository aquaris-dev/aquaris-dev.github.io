---
layout: post
title: Device Status &ndash; June, 2018
category: blog
excerpt: Current status of bq Aquaris devices on LineageOS
author: brinly
---

Hello all and welcome to the June aquaris-dev team update of 2018,

Another 2 months has passed, with not too much excitement publicly (apart from that April Fools drama) - big news this month arrives. We missed a May update, but we were hard at work regardless. We won’t cover the stats this time, but you can see the stats of how popular our BQ devices are by checking on the LineageOS [stats](https://stats.lineageos.org) site.

If you like to read more regular news on this website, please consider joining the team as a [developer](/contribute.html).

We're aware of the new BQ (Aquaris X2 series) devices (please stop emailing asking us to support them) but we have nothing to announce at this point (they aren't even out yet).

Our BQ device news now
-----------------

This month, we only really have news about the BQ Aquaris X/X Pro (bardock/bardockpro) device (it's our first 64bit device) as we haven't had a whole bunch of time to work on our projects.

We did some small security patches and maintenance fixes for our older devices. We added SSL/TLS (https) to our website too.

We want to share our appreciation to BQ as they released the Aquaris X/X-Pro Oreo [kernel](https://github.com/bq/aquaris-X-Pro/commit/27a6f892c943e7ac073373238e8b7f4f8ad5f732) source code before the shipping public OTA (as the their final BETA build was the same as the shipping GMS build) which is a great step for any OEM.

We'll look into at supporting our older devices (msm8937 based as they MAY receive Oreo from BQ at some point) first with Android Oreo (Lineage 15.1) but as always, we are not promising support for these devices - if you have contributions to make, please get in contact to help speed up this project..

If the community is interested, we might do a blog post in the future explaining some of the challenges of porting LineageOS to devices so our readers can learn about why things take so long..


Aquaris X / Aquaris X Pro - Status (bardock/bardockpro)
----------------------

![bardockproimg]({{ site.url }}/images/bardockproteaser.png)

We started with "[bardockpro](https://github.com/lineageos/android_device_bq_bardockpro)" support first, but Eloi also got his hands on a non "[pro](https://github.com/lineageos/android_device_bq_bardock)" variant later, so progress was speeded up with 2 developers on this project. We eventually decided to make a common device tree where a majority of the device code is stored (the devices are extremely similar).

Android 8.1 was released for the BQ Aquaris X and X Pro - so we can share our work soon. Luckily our kernel that we implemented/updated from scratch (see past blog posts) was very similar to the official release (mostly due to reverse engineering of binary kernels) so the merge was very minor and we are pretty pleased with BQ’s source release. 

We're getting extremely close with our project (with all known hardware "working" - some weird quirks exist - fixing up SElinux rules and cleaning up config files etc, setting up WIKI pages, forus threads) - you can see our work moved the official LineageOS GitHub (from Brinly's personal GitHub) at this [link](https://github.com/lineageos/android_device_bq_msm8953-common) and [here](https://github.com/lineageos/android_kernel_bq_msm8953).

We're going to require 2.0 (Android 8.1) firmware/bootloader/radio/TZ to flash LineageOS as our drivers need the latest base firmware to function correctly (Baseband, Encryption, Camera, Wi-Fi, IMS won’t work on N based firmware).

We’ll work on getting final [things](https://github.com/LineageOS/charter/blob/master/device-support-requirements.md) tuned for a official LineageOS 15.1 release in the very near future. We don't recommend using unofficial builds that are floating around on the internet for the device as we'll be working on supporting official builds later :).

Developers interested in helping out - (contact us) - but as always feel free to submit patches to the Lineage project's gerrit (we've already had a few people submit patches to help speed progress on this project)..


Open Issues
-----------

If there are any issues with any of our supported devices, please report a bug on the [LineageOS issue tracker](https://jira.lineageos.org/) and we'll look into them ASAP..

