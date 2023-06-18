---
layout: page
title: Mars Rover
description: a project that redirects to another website
img: assets/img/RangeRover/rover.jpeg
importance: 1
category: Software
---
This was our 2nd year End-Of-Year project. The goal was to design a fully functioning autonomous rover in a group of 7. I was in charge of the command module. This comprised of muliple components:
- AWS and Node.JS Back End for the rover to recieve commands and communicate data back to the user
- HTML/CSS/JS Front End for the user to interact with the rover
- MySQL Data Base to store and rover data such as postion and detected objects.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/RangeRover/RR-Home.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/RangeRover/RR-cntrl.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The 2 frontend of the WebApp. Left: Home and About page. Right: Rover Command Page.
</div>

The Command page includes:
- Buttons to toggle the rover's movement: 
    - Switching between autonomous and manual drive commands
    - Determining speed and controls
- Live Map:
    - Tracks rover's live position
    - Displays "aliens" and obstacles the rover detects
    - Can be used to select a co-oridnate for the rover to move to in manual mode
- Live Battery Information

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/RangeRover/rover.jpeg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <!-- <video> -->
        <iframe src="https://youtube.com/shorts/aE_GtGLtH0A?feature=share" title="YouTube video player" frameborder="0" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
        <!-- </video> -->
    </div>
</div>
<div class="caption">
    Image and video of the Rover in action
</div>