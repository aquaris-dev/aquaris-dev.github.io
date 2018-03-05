---
layout: post
title: Device Status &ndash; March 2, 2018
category: blog
excerpt: Current status of bq Aquaris devices on LineageOS
author: eloimuns
---

Hello all and welcome to the first aquaris-dev team update of 2018,

Time to update our blog since latest update was on September and we're sorry about the delay in our news updates, but real life comes first, and we barely remember to update this..

If you like to read more regular news on this website, please consider joining the team as a [developer](/contribute.html).

LineageOS Status
----------------

The LineageOS team is much better than us at remembering to do doing status reports, as they regularly publish news which you can find on their [website](https://www.lineageos.org).
The entire LineageOS project is continuously improving not only feature and design wise but also under the hood (infrastructure, team organization and documentation).

### Some numbers:

The total number of active LineageOS [installations](https://stats.lineageos.org/) is now 1.6 Million devices (April 2017: compared to 1.4 million).

- piccolo (bq Aquaris M5): 1256 (compared to September 2017: 1668)
- paella (bq Aquaris X5): 1106 (compared to September 2017: 1162)
- vegetalte (bq Aquaris E5 LTE): 788 (compared to September 2017: 725)
- gohan (bq Aquaris X5 Plus): 453 (compared to September 2017: 231)
- tenshi (bq Aquaris U Plus): 274 (compared to September 2017: 45)


It seems we're growing on 2016 devices (tenshi and gohan) but we're still going down on 2014/2015 devices (piccolo, paella and vegetalte) which is expected as people switch to newer devices..


Weekly Releases
---------------

We'll release "Aquaris U aka chaozu" next week, so new builds are now released every week for the following devices:

* paella (bq Aquaris X5)
* piccolo (bq Aquaris M5)
* vegetalte (bq Aquaris E5 LTE)
* gohan (bq Aquaris X5 Plus)
* tenshi (bq Aquaris U Plus)
* chaozu (bq Aquaris U)

Our BQ devices news now
------------------

Aquaris U (chaozu)
------------------
We're adding support to this new chaozu device as hinted in previous blogposts.

We've split the tenshi device tree into a common msm8937 tree since both (tenshi and chaozu) devices are really similar (this saves us time while maintaining the devices).

"chaozu" weekly builds  will be they available from the [LineageOS download server](https://download.lineageos.org/chaozu) as we just [enabled](https://review.lineageos.org/#/c/207799/) them today..

Thanks to github user @mifl for the contributions for this [device tree](https://github.com/LineageOS/android_device_bq_chaozu).

Aquaris M5 (piccolo) & X5 (paella)
-----------------------------------

We have recently updated our kernel and blobs to latest stock release (5.1.0). That requires an FIRMWARE update in order to work correctly for our LineageOS distribution

We recommend that you update the base firmware before you install the next LineageOS build so we included a guide below.

We wanted to make it pretty simple to update your device's firmware, so we prepared firmware ZIP's that are linked directly below:

1 - Download FIRMWARE zip:

   - [piccolo - Aquaris M5](https://drive.google.com/file/d/1eAUIyxBFEgm-OwFt2qcGr3880LL9GnZG/view)
   - [paella - Aquaris X5](https://drive.google.com/file/d/197deE4hQ-STTSmG7gXra1OA7mX8t1x_U/view)

2 - Download the next* LineageOS build from the download [server](https://download.lineageos.org/).

3 - Optional: Download the latest bq Camera release:

   - [bq Camera for M5 & X5](https://drive.google.com/file/d/1URujpry0P4tt2VGDAAqOJGGxawYE6c9O/view)

3 - Reboot to recovery and copy FIRMWARE and ROM zip to internal storage.

4 - Flash FIRMWARE zip.

5 - Reboot to recovery mode and reflash FIRMWARE zip then flash the ROM too.

6 - Reboot to system.

Notes:

FIRMWARE flash requires a reflash if the modem partition didn't get written to correctly.

 * Next build will be at 03/03, make sure to update firmware at this time, if not before. - 03/03 build will be the first build requring stock N firmware.


Aquaris X5 (gohan)
------------------

We merged a [patch](https://review.lineageos.org/#/c/200886/) fixing an [issue](http://jira.lineageos.org/browse/BUGBASH-1202) affecting use of the camera/torch functionality for some users with camera sensor that was introduced by BQ recently (cmb087qr) that wasn't present on our test devices.

Aquaris X/X Pro Status (bardock)
----------------------

We're rebasing our device tree to use Oreo as base for our LineageOS 15.1 release. It actually boots but there are a few bugs that we can resolve when we get kernel source, then we’ll work on getting it merged into mainline LineageOS.
This process will be sped up once BQ releases Oreo source code (we have a beta build but not kernel source). Developers interested in helping out - feel free to contact us as usual.

Open Issues
-----------

We are aware that there is a whole bunch of security fixes missing in our kernels (see [LineageOS CVE Tracker](https://cve.lineageos.org/)).
These issues will be fixed within the next days with our kernel rebase that we intend to push soon but you should be warned about it.

Besides this, there are no open issues reported in the [LineageOS issue tracker](https://jira.lineageos.org/).

If there are any issues with any of our supported devices, please report a bug on the [LineageOS issue tracker](https://jira.lineageos.org/).

