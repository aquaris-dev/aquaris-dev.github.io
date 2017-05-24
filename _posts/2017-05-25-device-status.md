---
layout: post
title: Device Status &ndash; May 25, 2017
category: blog
excerpt: Current status of bq Aquaris devices on LineageOS
author: brinlyau
---

Hello friends! 

It's been a month since our latest update, so it's time to share some news...


Exciting news
-------------

As noted in last status update: Android 7.1 has been released by bq for both tenshi and gohan devices, including the kernel modifications that we've been waiting for. Once we had a bit of time, we jumped into cm-14.1 development. We’re now focusing our work for both devices on the cm-14.1 branch which is itself based on Android 7.1.

We've been hard at work at some of our mostly recently supported devices including the Aquaris X5 Plus (gohan) and Aquaris U Plus (tenshi) - both are quite special, as they are part of a new platform of devices (msm8976/msm8937) that we’re supporting.

We're very close to reaching a point on both devices when they have "official full support" rather than being in a limbo case of "WIP" - see sections below for more info :)

Both are targeted for cm-14.1/Android 7.1.2 release status, using the latest BQ release for firmware and kernel / driver binaries (thanks to BQ for promptly releasing the (GPL licenced) kernel source).


gohan
-----------
[gohan](http://aquaris-dev.org/images/gohan-may-screenshot.png) (or BQ Aquaris X5 Plus) has been getting very close to the official mark of support with our recent work on this [project](https://github.com/LineageOS/android_device_bq_gohan).

The only current issues are some issues with the Snap camera app and the setting/reading of the serial number from the /persist partition.

Special thanks to _cyclon1978_ for stepping up to contribute some very useful (including audio, camera and more) fixes to our project in addition to our usual contributors of _cmorlok_ , _stucki_ and _kra1o5_ for the initial bringup work of cm-14.1 (with the support of our entire team)..

We’re working on resolving these final issues, so we can enable official (support of) weekly builds.

Please use the latest firmware to avoid strange issues if you are testing our work (you can find testing releases posted by our members on htcmania and android-hilfe.de).

tenshi
-----------
[tenshi](http://aquaris-dev.org/images/tenshi-may-screenshot.png) (or BQ Aquaris U Plus) has also been getting very close to official builds too with recent work on our recent work on the cm-14.1 branch. We’re basing our release on the 7.1 release from BQ - so make sure you have the latest firmware (2.1 presently) before flashing LineageOS.

We’ve forked our [device tree](https://github.com/LineageOS/android_device_bq_tenshi) and [kernel](https://github.com/LineageOS/android_kernel_bq_msm8937) over to the LineageOS GitHub so if you're an interested developer, you’ll need to contribute changes upstream to gerrit code review server.

We’re not aware of any issues with the hardware support at this point so we’ll be flipping the [switch](https://review.lineageos.org/#/c/173139/) now for official weekly builds by the LineageOS build server.

reminder: chaozu/chaozulite are presently _not_ supported so we advise against flashing tenshi builds on those devices since it may brick your device..

Props to _eloimuns_ and _brinlyau_ for their work on enabling support for this device.


Security patches
-----------
We've updated all the devices kernels to include May’s security patches (some more detail can be found on [Android Security Bulletin](https://source.android.com/security/bulletin/2017-05-01)). We'll continue to update kernels regularly with new security patches supplied by Google. We recommend that you always use the latest firmware release to fix potential security issues in the radio/bootloader/tz firmware.


LineageOS Status
----------------

The community around LineageOS has grown [quite notably](https://stats.lineageos.org/), and with this, so has our BQ specific user-base.

Regardless, it is great to see that the total number of active LineageOS installations is currently at more than 1.6 million devices. 

You can always read the latest news about what's happening at LineageOS on their own blog at [lineageos.org](https://lineageos.org/).

Weekly Releases
---------------

Meanwhile, new builds are released every week at LineageOS for all of the three supported devices:

* paella (bq Aquaris X5)
* piccolo (bq Aquaris M5)
* vegetalte (bq Aquaris E5 LTE)

Open Issues
-----------

If there are any other issues with any of the three _supported_ devices listed above, please report a bug on the [LineageOS issue tracker](https://jira.lineageos.org/).
(You may also remember that there used to be another issue tracker on our own GitHub project. This is no longer used and will soon be removed...)

Wiki updates
------------------------

LineageOS wiki pages have been updated and added for our currently supported BQ devices. Go check it out (or fix mistakes/typos) on the [LineageOS wiki](https://wiki.lineageos.org).


New bq device support
----------------------
We’re stretched pretty thin already at the moment but we welcome any developer to step up with the work and get in contact with us. We don’t pre-announce support for any device - see the LineageOS wiki page [here](https://wiki.lineageos.org/device_requests.html) for more info. Let’s just keep waiting and we'll see what the future brings. :)


