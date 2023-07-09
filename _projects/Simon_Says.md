---
layout: page
title: Simon Says Battle Royale - FPGA Video Game
description: Multiplayer Video Game using FPGA and input controller
img: assets/img/SSays/ss-screen.jfif
importance: 4
category: Hardware
---

This project was a simple multiplayer "Battle Royale" style video game intended to make physiotherapy and physical recovery entertaining for young children. The video-game was developed in a group of 6 and I mainly contributed to developing the FPGA as the input device.

Input/Output peripherals on the FPGA were used to interact with the video game. The FPGA acts as a dedicated component of the game constantly providing the user with the information, making use of its compute power not treating simply as an accelerometer for i/o.  Multiplayer is implemented via a centralized server, hosted on AWS. This keeps tracks of each player connected in the game and handles the game flow. The FPGA and a python program running on the host laptop act as the client connected to the server, providing the user input and data and receiving instructions for the server to progress the game and update the host's results.

The FPGA Controller has the following functionality:
- Real-Time transmitting and receiving of data between FPGA and Client PC
- Accelerometer to detect x/y/z translational motion
- Low Pass FIR filtering of accelerometer data
- Buttons, Switches, LEDs and 7-Segment display as i/o peripherals 

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
