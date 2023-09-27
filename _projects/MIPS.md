---
layout: page
title: MIPS 32-bit CPU
description: Simple 32-Bit MIPS CPU in Verilog
img: assets/img/MIPS/MIPS.png #FPGA IMAGE
importance: 3
category: Hardware
---

This was a group project with 6 colleagues. It comprised of designing the fundamental digital blocks to make a 5-stage MIPS 32-bit CPU and creating test-benches to verify the operation of any equivalent MIPS 32-bit CPU.

I personally was responsible for designing the instruction decode, register file, memory access and control blocks. I also took on the duty of validating the overall execution of the CPU, separate to unit tests. Instructions were provided to the CPU via an avalon memory bus, to ensure a faithful test of the real world operation of the CPU I created a test-bench template in SystemVerilog to simulate the endianess clock delay of the memory interface bus. This unified the overall process enabling anyone in the team could quickly create unit tests and test-benches .

<div class="row justify-content-sm-center">
    <div class="col-sm-7 mt-3 mt-md-0">
        {% include figure.html path="assets/img/MIPS/MIPS.png" title="example image" class="img-fluid rounded z-depth-1" %} 
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/MIPS/flow.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    Left: Designed MIPS Block Diagram. Right: Test-bench Methodology.
</div>
