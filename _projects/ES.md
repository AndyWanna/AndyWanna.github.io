---
layout: page
title: Digital Synth
description: Digital Synth using Arm M4
img: assets/img/Synth/synth.png
importance: 4
category: Software
---

This project mainly focused on low-level multithreaded programming in Embedded C to create a digital synthesizer. In our group of 4 people, I focused mainly on creating concurrent threads and ISR functions to enable increasing capabilities of the digital synthesizer. Some of the key functionalities I implemented include:

- Polyphony across multiple keyboards (compounding multiple key frequencies)
- Modular keyboards with Auto Detect (enable connection/disconnection of modules in any order or time)
- Stereo Sound (Sound is played across all available speakers) 

A key part of this project was ensuring thread safety and that each thread meets it's required deadlines. To verify this I implemented a configurable test suite using C directives.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Synth/synth.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Synth/threads.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Single synth module. Right: Thread and ISR functions.
</div>

