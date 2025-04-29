---
title: Rapid Prototype
layout: page
nav_order: 5
---

## BikeGuider Rapid Prototype Display 

BikeGuider consists of two core elements: a handlebar-mounted haptic module and a companion mobile app. 

The haptic module, powered by an ESP32 microcontroller, delivers programmable vibration intensity and patterns via 3D-printed mounts.

<div style="display: flex; justify-content: center; gap: 1rem; flex-wrap: wrap;">
  <figure style="margin: 0;">
    <img src="Images/handlebar_fixed_compon_1.png"
         alt="Front view of handlebar motor mount"
         width="400">
    <figcaption>Front view of the 3D-printed motor mount</figcaption>
  </figure>
  <figure style="margin: 0;">
    <img src="Images/handlebar_fixed_compon_2.png"
         alt="Side view of handlebar motor mount"
         width="400">
    <figcaption>Side view showing attachment points</figcaption>
  </figure>
</div>

<div style="text-align: center;">
  <img src="Images/rapid_prototype_sketch.jpg" alt="rapid_proto_sketch" width="400">
  <figcaption>Overall system sketch</figcaption>
</div>

<video width="600" controls>
  <source 
    src="{{ '/Video/vibrating_motor_demo.mp4' | relative_url }}" 
    type="video/mp4">
</video>



