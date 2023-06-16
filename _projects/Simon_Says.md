---
layout: page
title: Simon Says Battle Royale - FPGA Video Game
description: Multiplayer Video Game using FPGA and input controller
img: assets/img/SSays/ss-screen.jfif
importance: 1
category: Hardware
---

This project was a simple multiplayer "Battle Royale" style video game intended to make physiotherapy and recovery entertaining for young children. The video-game was developed in a group of 6 and I mainly contributed to developing the FPGA as the input device.
Input/Output peripherlas on the FPGA are used to interact with the video game. Multiplayer is impemented via a centralised server with FPGA interfacing with a local python client connected to the server. 

The FPGA Controller has the following functionality:
- Real-Time transmitting an recieving of data between FPGA and Client PC
- Accelerometer to detect x/y/z translation
- Low Pass FIR filtering of accelerometer data
- Buttons, Switches and 7-Segment display as i/o peripherals 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/SSays/ss-screen.jfif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/SSays/de10.webp" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Example screen from Video Game. Right: FPGA Controller
</div>
