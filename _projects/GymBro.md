---
layout: page
title: Gymbro - Embedded System
description: Embedded Sytem integrating Raspberry Pi and AWS server
img: assets/img/GymBro/Device.jpg
importance: 2
category: Software
---

This project focused on using embedded systems to create a commericial product. Our product, Gymbri, is an integrated product and webapp that acts your personal gym assistant. It keeps track of your overall workouts and progress over time but further track your reps and rest time for each excersise while at the gym. 

 The main local processor was a Raspberry Pi Pico running python. The device was communicating with an AWS Server running Node JS to handle the information provided by the deivces and users. I focused on creating the server backend and integrating the full system with the Raspberry Pi. My goal was ot create a server that could easily handle multiple users and devices interacting wiht the webapp. The technologies used to achieve this were Passport.JS and a seperate MySQL database. The functionality of the server includes:

- AWS servre handles multiple concurrent users and devices.
- User accounts and secure authentication
- Accelerometer to automatically count repetitions in real time
- Keep track of workout and excersise history and progress

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/GymBro/Device.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Gymbro Model Device
</div>

Screenshots from the Webapp can be seen below

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/GymBro/history.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/GymBro/Wrkt1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/GymBro/Wrkt2.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>    
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/GymBro/Start.webp" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Various webpages from the Gymbro webapp
</div>

<div class="row">
    <div>
        <iframe width="560" height="315" src="https://www.youtube.com/embed/rFBxXwwBgMg" title="YouTube video player" frameborder="0" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
    </div>
</div>
<div class="caption">
    Gymbro advertisement video
</div>
