---
layout: post
title: Baofeng Radio Programming
date: 2025-01-05 19:11:00-0800
description: BC Channel programming for Baofeng UV-82 radio.
tags: radio outdoors
categories: small-projects sports
thumbnail: assets/img/posts/2025-01-05-post-radio-channels/listing-sticker.jpg
giscus_comments: true
related_posts: false
related_publications:
---

Inexpensive radios like the Baofeng UV-5R are super handy and popular in the outdoors. I compiled a list of channels from a bunch of sources to program these radios that is especially useful for recreation and travel in British Columbia.

## Requirements

- Baofeng radio, I use the UV-82HP
- USB to headphone/mic jack programming cable, these are easily available online
- [CHIRP](https://chirpmyradio.com/projects/chirp/wiki/Download) program

## Instructions

1. Download the CHIRP program and my config file [here]({{ 'assets\files\posts\2025-01-05-post-radio-channels\Baofeng_UV-82HP_20210114.img' | relative_url }}).
2. Plug in your radio with the programming cable and power it on.
3. Download the current configuration from the radio. In CHIRP, select Radio ⯈ Download from radio... and follow the steps. In my case, the Port is "Prolific USB-to-Serial Comm Port", the vendor is "Baofeng", and the model is "UV-82HP". For some programming cables under Windows 11, the steps [here](https://www.miklor.com/COM/UV_Drivers.php#install) must be followed to revert to the older Prolific driver.
4. At this point, make a backup of your current configuration using File ⯈ Save As...
5. Load my config file into CHIRP with File ⯈ Open..., which should result in the table of channel parameters shown below.
6. Make any modification to the channels and settings by using the respective tabs in CHIRP.
7. When finished, upload to the radio with Radio ⯈ Upload to radio...

<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/posts/2025-01-05-post-radio-channels/chirp-channels.png" class="img-fluid rounded z-depth-1" zoomable="true" %}
    </div>
    <div class="col-sm-3 mt-5 mt-md-0">
        {% include figure.html path="assets/img/posts/2025-01-05-post-radio-channels/listing-sticker.jpg" class="img-fluid rounded z-depth-1" zoomable="true" %}
    </div>
</div>
<div class="caption">
    Left: CHIRP with the config file loaded. Right: Channel reference label stuck on battery.
</div>

## Channel Listing

The config file currently contains the following channels. I have not tested all of them. Many of these channels require an amateur radio licence to transmit on, please use responsibly! This is available as a [spreadsheet]({{ 'assets\files\posts\2025-01-05-post-radio-channels\channel-listing.xlsx' | relative_url }}) also containing a helpful label you can place on the radio as shown above. Happy adventures!

|--------------|------|----------|------------|
|Channel index | Name | Category | Details    |
|--------------|------|----------|------------|
| 1-14         | FRS  | General purpose | General purpose family radio service channels used to communicate with other radios (e.g. BCA link, Rocky Talkie). |
| 15-22        | GMRS | General purpose | The additional 8 higher-power GMRS channels. |
| 23-28        | BC Link | General purpose | Duplicates of several FRS and GMRS channels that correspond to channels 'A' through 'F' of the BCA Link radios. |
| 29-30        | LP | Travel | LP channels generally used for logging operations. |
| 31-35        | MURS | General purpose | USA multi-use radio service public channels (<span style="color:red">currently not approved in Canada</span>). |
| 36-40        | LADD | Industry | Commonly used trucking channels in BC. |
| 41-75        | RR | Travel | Resource road callout channels for BC forest service road travel. |
| 76-80        | LD | Travel | Resource road loading channels. |
| <span style="color:red">81-82</span> | <span style="color:red">SAR</span> | <span style="color:red">Emergency</span> | <span style="color:red">Search and rescue for BC and Canada.</span> |
| 83-87        | WX | Weather | RX-only weather channels for Canada. |
| 88-97        | Various | Industry | Logging channels used in the Kootenays. |
| 98-113       | REP | Repeater | Commonly used BC repeater channels. |
| 114-123      | MAR | Marine | Backup of common marine VHF channels (<span style="color:red">Ch. 114, 116, and 121 are emergency!</span>). |
| 124          | 4WDABC | General purpose | 4 Wheel Drive association of BC |
| 125-127      | WBSP | Industry | RX-only Whistler Blackcomb Ski Patrol |
