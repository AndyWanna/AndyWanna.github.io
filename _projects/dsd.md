---
layout: page
title: Digital Hardware Design - FPGA
description: Cosine Accelerator on an FPGA in Verilog
img: assets/img/DSD/de1.jpg #FPGA IMAGE
importance: 1
category: Hardware
---

This project involved taking subsequent steps to accelerate an arbitrary vector function:
$$ f(x) = \sum_{i=1}^{N} 0.5 \times x_i + x_i^2 \cos(\frac{x_i - 128}{128})$$ \\
On a DE1-SoC FPGA board.

The start of this project involved relatively small hardware/software additions and optimization. The final steps resulted in major latency reduction by adding a custom instruction to the NIOS-II soft-core processor via a bespoke digital block, including a CORDIC function in hardware. 

Here are some of the optimization that resulted in the largest speed gains:
- Custom CORDIC hardware block with optimized iterations/word-length
- Specialized Floating-Point power of 2 divider
- Optimum instruction and data cache sizes


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/DSD/de1.jpg" title="example image" class="img-fluid rounded z-depth-1" %} 
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/DSD/cordic.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: The DE1-SoC FPGA board. Right: Bespoke digital block, implementing the arbitrary vector function mentioned above. 
</div>

