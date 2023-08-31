---
layout: post
title: Bike Mount for Garmin GPSMAP 66i
date: 2023-08-29 16:30:00-0100
description: A DIY 3D-printable mount for GPSMAP devices on 32 mm handlebars.
tags: diy bikes 3d-printing
categories: small-projects sports
thumbnail: assets/img/posts/2023-08-29-post-bike-mount/render.jpg
giscus_comments: true
related_posts: false
related_publications:
---

I wanted to mount my Garmin GPSMAP 66i device on my bike handlebars to stop always making wrong turns. I couldn't find anything readily available for the Garmin devices with the sliding belt-clip-style mount point (I believe this is all the larger GPSMAP devices and probably more). I remixed the Garmin mounting clip from [here](https://www.thingiverse.com/thing:3063518). The design allows the Garmin to be oriented parallel or perpendicular to the tube, allowing you to use this on the stem or handlebars with diameter around 32 mm.

<div class="col-sm-4 mt-3 mt-md-0" style="float:right;">
    {% include figure.html path="assets/img/posts/2023-08-29-post-bike-mount/render.jpg" class="img-fluid rounded z-depth-1" %}
</div>

## What you Need

- [STL]({{ 'assets/files/posts/2023-08-29-post-bike-mount/gpsmap-handlebar-mount.zip' | relative_url }}) or [Solidworks Assembly]({{ 'assets/files/posts/2023-08-29-post-bike-mount/gpsmap-handlebar-mount.SLDASM' | relative_url }}) file(s) for three parts: lower clamp, upper clamp, and Garmin interface
- 4 pieces of M4 x 15 mm machine screws
- M5 nut
- M5 x 10 mm socket head machine screw
- M4 tap

## Assembly

I printed the STL files out of PLA with 60% infill. It was necessary for me to slightly enlarge the channels that the Garmin slides into as well as sand down the "snap" that interfaces with the Garmin belt clip. After cleanup, the holes in the lower clamp need to be tapped for M4 thread. The M5 nut has a interference fit in the recess on the underside of the upper clamp piece. The two sides of the clamp can then be installed around the handlebar and the Garmin interface screwed into place with the short M5 screw.

## Finished Product

I recommend using a lanyard from the device to the handlebars as additional security!

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/posts/2023-08-29-post-bike-mount/mount-1.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/posts/2023-08-29-post-bike-mount/mount-2.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The custom mount with and without device. Never to be lost again!
</div>
