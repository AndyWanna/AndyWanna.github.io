---
layout: page
title: MIPS 32-bit CPU
description: Simple 32-Bit MIPS CPU in Verilog
img: assets/img/12.jpg #FPGA IMAGE
importance: 1
category: work
---

This was a group project with 6 colleagues. It comprised of designing the fundmanetal digital blocks to make a 5-stage MIPS 32-bit CPU and creating testbenches to verify the operation of the CPU.

I persoanlly was responsible for designing the Instruction Decode, Register File, Memory Access and Control blocks. I also took on the duty fo validating the overall exectution of the CPU, seperate to unit tests, which involved debugging and redising the CPU multiple times. Furthemore I created the test-bench template in SystemVerilog to unify and optimize the overall process of creating unit tests.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/mips.jpeg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    MIPS Block Diagram. 
</div>

Check github repo