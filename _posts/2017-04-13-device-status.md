---
layout: post
title: Device Status &ndash; April 13, 2017
category: blog
excerpt: Current status of bq Aquaris devices on LineageOS
author: stucki
---

Hola amigos! 

it's been a while since our latest update. Time to share some news... 

This is the second report where we like to give you an overall update of the things that are going on about LineageOS right now. 

LineageOS Status
----------------

The community around LineageOS has grown [quite notably](https://stats.lineageos.org/), and with this has our user-base: In February, the LineageOS download server identified 592 active installations of the piccolo port (bq Aquaris M5). Now in April, the number almost three times as high  
(April 12: 592 active installations). 

It is anyway great to see that the total number of active LineageOS installations is currently at more than 1.4 Million devices.  
(Source: [web.archive.org](http://web.archive.org/web/*/https://stats.lineageos.org/)) 

Besides this, you can always read the latest news about what's happening around LineageOS on their own blog at [lineageos.org](https://lineageos.org/).

Weekly Releases
---------------

Meanwhile, new builds are released every week for all of the three supported devices:

* paella (bq Aquaris X5)
* piccolo (bq Aquaris M5)
* vegetalte (bq Aquaris E5 LTE)

Open Issues
-----------

So far, there are are no open issues (except 2 with pretty low priority) reported in the [LineageOS issue tracker](https://jira.lineageos.org/). 

One major blocker over the last months has been [BUGBASH-72](https://jira.lineageos.org/browse/BUGBASH-72) where the loss of mobile data connectivity when leaving the Wifi was reported. This issue has happened for many users and we spent __a lot__ of time into investigating and fixing it. Some weeks back, the issue, which occured also on other devices, was [fixed for some of them](https://review.lineageos.org/#/c/163824/), however this didn't work for our devices... 

Finally, after lots of trying and testing, a (rather simple) workaround was found that [fixes the issue](https://review.lineageos.org/#/c/168163/). We're happy to say that new releases after April 10 will have this issue fixed! If you still encounter any problems as described in [the report](https://jira.lineageos.org/browse/BUGBASH-72), please let us know...

If there are any other issues with any of the three supported devices, please report a bug on the [LineageOS issue tracker](https://jira.lineageos.org/). 
(You may also remember that there used to be another issue track on our own Github project. This is no longer used and will soon be removed...)

Status of gohan & tenshi
------------------------

A lot of users have asked about the status of the bq Aquaris X5 Plus (gohan) and the bq Aquaris U Plus (tenshi).

We spent a lot of time into the development of these ports until March. Both device ports were first built with cm-13.0 (Android 6). 
So far, tenshi with cm-13.0 is technically buildable, but not recommended for daily use. gohan is also working with cm-13.0, however the speaker is not functional (and there may be other issues). For both ports, no builds have been released, but you can make your own build from sources.  
(Hint: [docker-lineageos](https://github.com/stucki/docker-lineageos)) 

At the end of the month, Android 7 has been released by bq for both devices, including kernel modifications that we've been waiting for. This means that from now on, our work for both devices will focus on the cm-14.1 branch which is based on Android 7. We will soon continue working on these devices, however until now there was no time for it since the release... 

It should be noted that the development for gohan is currently happening in a private repository (which will be published once the device boots again). Interested developers who know what this means can get in touch with [Christian](https://github.com/cmorlok) to get access to the private repository... 
