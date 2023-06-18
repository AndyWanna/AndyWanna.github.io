---
layout: page
title: MIPS 32-bit CPU
description: Simple 32-Bit MIPS CPU in Verilog
img: assets/img/MIPS/MIPS.png #FPGA IMAGE
importance: 3
category: Hardware
---

This was a group project with 6 colleagues. It comprised of designing the fundamental digital blocks to make a 5-stage MIPS 32-bit CPU and creating test-benches to verify the operation of any equivalent MIPS 32-bit CPU.

I personally was responsible for designing the instruction decode, register file, memory access and control blocks. I also took on the duty fo validating the overall execution of the CPU, separate to unit tests, which involved debugging and redesigning the CPU multiple times. Furthermore I created the test-bench template in SystemVerilog to unify and optimize the overall process of creating unit tests.

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
