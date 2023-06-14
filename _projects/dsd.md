---
layout: page
title: Digital Hardware Design - FPGA
description: Cosine Accelerator on an FPGA in Verilog
img: assets/img/12.jpg #FPGA IMAGE
importance: 1
category: work
---

This project involved taking subsequent steps to accerlate an arbitrary vector function:
$$ f(x) = \sum_{i=1}^{N} 0.5 \times x_i + x_i^2 \cos(\frac{x_i - 128}{128})$$
On a DE1-SoC FPGA board.

The start of this project involved relatively small hardware/software additionas and optimisation. The final steps resulted in major latency reduction by adding a custom instruction to the NIOSII softcore processor via a bespoke digital block, including a CORDIC function in hardware. 


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/de1.jpg" title="example image" class="img-fluid rounded z-depth-1" %} 
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/cordic.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left is the DE1-SoC FPGA board. On the right is bespoke digtal block, implementing the arbitrary vector function mentioned above. 
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal its glory in the next row of images.
