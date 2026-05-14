---
layout: page
title: "iPod Variations Help Guide"
permalink: "/ipod-variations-help/"
header:
    image_fullwidth_staff: ravaei_header.png
---

See the tutorial video below for setup and usage instructions, or scroll down for troubleshooting information. For additional support, please <a href="{{ site.url }}{{ site.baseurl }}/contact/">contact Kian</a>.

<div class="center flex-video widescreen vimeo">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/meHX0E88xjg" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

## Setup Diagram

<div class="row">
  <div class="twelve columns">
    <img src="{{ site.urlimg }}ipod-variations-setup.svg"
         alt="iPod variations setup"
         class="scale-with-grid">
  </div>
</div>

## Downloads

* [Max](https://cycling74.com/downloads) (Download the free version, it is not necessary to have a trial of the paid version)
* <a href="{{ site.url }}{{ site.baseurl }}/downloads/ipod-variations.html">iPod Variations Max Project</a>

## Troubleshooting

### _Audio is not working_

Make sure the downloaded ZIP folder for iPod Variations is unzipped. Open the folder and ensure that the enclosed "media" subfolder contains all 61 WAV files.

Open the project file and go to Audio > Open Audio Settings. Ensure that the correct audio output device is selected. Also, try toggling the "Audio On" button off and on again.

### _Foot pedal is not working_

If using a USB foot pedal, ensure that the pedal is set to spacebar. This is usually done with a software that can be downloaded from the foot pedal manufacturer's website.

If using a bluetooth foot pedal, check the computer's bluetooth settings to ensure that the pedal is connected. The computer must also be within range of the pedal's bluetooth signal. Ensure that the left pedal is set to PageDown (STOP), and the right pedal is set to PageUp (GO). This is usually done with a software program that can be downloaded from the foot pedal manufacturer's website.

### _Mirroring is not working_

First, ensure both devices are connected to the same WiFi network or mobile hotspot. Press the "refresh" button everytime your device connects to a new network to generate a unique connection URL.

The most common reason for this issue is that the WiFi network has a firewall blocking the Miraweb connection. The best solution is to connect both devices to a mobile hotspot. The mobile hotspot can be from the phone you're using to mirror, or a different device.

In rare instances, there is an issue with the latest issue of Miraweb. Open the iPod Variations Project File and go to Mirror > Install Miraweb. If Miraweb is already installed, press "uninstall" and download a previous version.

### _Something else is not working_

Try downloading version 9.1.2 from the [Max](https://cycling74.com/downloads) website, and reopening the iPod Variations project file. Turning your computer off and on again is always worth a try. If the issue persists, please <a href="{{ site.url }}{{ site.baseurl }}/contact/">contact Kian</a>.

_Updated 2026-05-14_