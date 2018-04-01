---
layout: post
title: Device Status &ndash; April, 2018
category: blog
excerpt: Current status of bq Aquaris devices on LineageOS
author: brinly
---

Hello all and welcome to the second aquaris-dev team update of 2018,

We're starting to rememeber to make blogs once a month and we're sorry about the delay in our news updates, but real life comes first, and we barely remember to update this..

If you like to read more regular news on this website, please consider joining the team as a [developer](/contribute.html).

LineageOS Status
----------------

The LineageOS team is much better than us at remembering to do doing status reports, as they regularly publish news which you can find on their [website](https://www.lineageos.org).
The entire LineageOS project is continuously improving not only feature and design wise but also under the hood (infrastructure, team organization and documentation).. The team recently announced the Lineage SDK (https://lineageos.org/Introducing-the-LineageSDK/) for Lineage 15.1 devices, so we're not eligble currently, but this is something we are looking forward to releasing for you (...[hint ;) ](http://aquaris-dev.org/images/bardock151.png)..)..

### Some numbers:

The total number of active LineageOS [installations](https://stats.lineageos.org/) is now 1.8 Million devices (April 2017: compared to 1.4 million).

- piccolo (bq Aquaris M5): 1195 (compared to September 2017: 1668)
- paella (bq Aquaris X5): 1126 (compared to September 2017: 1162)
- vegetalte (bq Aquaris E5 LTE): 839 (compared to September 2017: 725)
- gohan (bq Aquaris X5 Plus): 452 (compared to September 2017: 231)
- chaozu (bq Aquaris U): 25
- tenshi (bq Aquaris U Plus): 289 (compared to September 2017: 45)

Similar stats as before :)

Weekly Releases
---------------

We released "Aquaris U aka chaozu" last month, so new builds are now released every week for the following devices:

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
We're added support for this device - as it's very similar to tenshi.

"chaozu" weekly builds  are available from the [LineageOS download server](https://download.lineageos.org/chaozu) now.

We're spread pretty thin on time already, but we are welcoming patches for the chaozulite device as it is also quite similar to the other "chaozu/tenshi" devices. (several of us have a device, but not much time)


Aquaris X Pro Status (bardockpro)
----------------------

We're still working on our device tree (we renamed our tree) for our LineageOS 15.1 release. It actually boots but there are a few bugs that we can resolve when we get official Oreo kernel source (we're using a frakenstein kernel), then we’ll work on getting it merged into mainline LineageOS. We don't recommend using unofficial builds that are floating around on the internet for the device (we can't vouch for the quality and our 15.1 branch requires special non publicly available firmware). We'll start with "bardockpro" support first, but we'll look at supporting the non "Pro" variant later.
Developers interested in helping out - feel free to contact us as usual or submit patches (we've already had a few people submit patches to help speed progress on this project)..

Open Issues
-----------

If there are any issues with any of our supported devices, please report a bug on the [LineageOS issue tracker](https://jira.lineageos.org/).


