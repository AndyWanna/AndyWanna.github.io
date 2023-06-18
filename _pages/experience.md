---
layout: page
title: Experience
permalink: /experience/
description: Growing resume of techincal experiences
nav: true
nav_order: 1
---

## Quantum Motion Technologies

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Logos/QMT.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Quantum Motion Technologies (QMT) is a quantum computing startup looking to create qubits using electron spin, using classical silicon transistors. I am working on the Integrated Circuits (IC) team where we aim to integrate classical analogue and digital electronics onto silicon chips with quantum elements.

### 6-Month Industrial Placement - 2023

The primary project over these 6 months involves investigating the viability of using FPGA's and a custom digital hardware/software stack to replace the current methods of measuring and controlling Quantum Test Chips. I also have a secondary project that involves porting the current software environment used to program the chips onto a RP2040.

The primary goals and task I will complete/have completed over these 6 months are:
* Building on the Quantum Instrumentation Control Kit (QICK) in both hardware and software
  - Expandidng on provided FPGA custom hardware to add new exclusive functionality necessary at QMT
    * Peak-Tracking hardware control loop
    * Improved precision/range/functtionality of  signal generators
  - Developing software library for an end-user to interface with FPGA
* Improving tool-flow by porting systems to low-level C on an RP2040
  - Add ability for end user to interface with RP2040 via a serial or ethernert connection
  - Convert all communication between the RP2040 and target chip to utilise hardware communcication protocols

### 3-Month Internship at Quantum Motion Technologies - 2022

During these 3 months my prject revolved more around analogue and digital validaiton. The 1st project was designing a current sensor with specifc requirements to replace the existing one being used. The second was to investigate a correlation between on chip ring oscillators and transistor properties.

The key completed tasks during this intership include:
- Characterised silicon transitor properties at both room temperature and cryogenic temperatures
   * Automated data preporcessing and analysis using Python
   * Verified operation of ring oscillators
- Designed low-noise, wide range (1na-10ma), wideband (100MHz) current sensor schematic and PCB


## Research into Hardware Optimization at Imperial College London 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Logos/icl.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Throught my 3rd year at university I have been researching with the Circuits and Systems (CAS) gorup at Imperial College London. We are investigating the usgae of Equivalency Graphs (E-Graphs) in datapath optimization for multiplier circuits. 

Multiplier circuits account for significant resource usage in datapath-dominated circuit designs and RTL designers continue to build bespoke hand-crafted multiplication arrays for their particular application. The construction of an optimized multiplier presents trade-offs between pre-processing to generate a smaller array and array reduction. E-Graphs are cruically able to epxlore these various tradeoffs effeciently.

The following are some of the early developments that have been made:
* Created rewrite framework in Rust using EGG to express alternative multiplier representations via E-Graph rewrites.
* Demonstreated the proposed tool can reduce the latency of a squaring circuit by up to 69%

