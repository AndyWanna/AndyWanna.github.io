---
layout: page
title: Technical Experience
permalink: /experience/
description: Growing collection of Industry Experiences
nav: true
nav_order: 2
---

## AMD - 3-Month Summer Internship - 2025

During my summer research-oriented internship at AMD, following my first PhD year, I worked within the Numerical Architecture Hardware Group. This team, similar to the group I worked with at Intel the previous year, focused on the design and automation of high-performance arithmetic components for GPUs and NPUs. Our objective was to develop datapath generation tools that produce designs optimized for highly specific domain data properties, such as input arrival times, toggle rates, and specialized formats. My primary project centered on advanced multiplier generation.

To establish the foundation for a high-performance multiplier generator, we first needed to rigorously define the existing design space of optimal multiplier architectures. This investigation led directly to the invention of novel integer and constant multiplier architectures, achieving significant gains in both minimum delay and area efficiency over baseline designs. Utilizing these foundational components, I developed a sophisticated E-Graph multiplier framework that systematically modeled the entire design space for array creation and reduction. This innovation allowed for the automated exploration and synthesis of arbitrarily hybrid, high-performance multiplier architectures.

Finally, I integrated domain-specific input data properties (such as arrival time and toggle rates) into the framework. This capability enabled the system to automatically generate optimized designs that account for the specific use-case domain features, thereby ensuring optimal power and performance profiles for target applications.

## Intel - 2-Month Summer Internship - 2024

The summer between graduating from Imperial and starting my Ph.D. at Georgia Tech I completed a fast-paced internship as part of the numerical hardware team in the GPU group at Intel. The group applies to modern arithemtic and hardware research to compute units withing Intel's advanced GPUs and NPUs, blending hardware and mathematics research and practical engineering.

My primary project focused on automating the optimization of mixed-precision floating point multipliers using E-Graphs, implemented in Rust. This work aimed to enhance the efficiency of multiplier designs, a critical component in Intel's GPU and NPU architectures. In parallel, I investigated strategies for minimizing glitch power in hardware designs, employing Integer Linear Programming techniques. This research is crucial for reducing energy consumption and improving the reliability of digital circuits. Additionally, I explored optimization methods for dot-product hardware units, laying the groundwork for future developments in Intel's computational hardware.

Despite the limited time, we developed promising ideas that should continue influencing future dot product and multiplier units within Intel GPUs and NPUs. The insights and skills gained from the internship were significant, sparking several hardware automation questions that will undoubtedly influence my PhD research. This experience provided invaluable exposure to industrial practices and challenges, offering a unique perspective that will shape my future work in the field.

## Quantum Motion Technologies - 6-Month Industrial Placement (CO-OP) - 2023

Quantum Motion Technologies (QMT) is a quantum computing startup looking to create qubits using electron spin, using classical silicon transistors. I am working on the Integrated Circuits (IC) team where we aim to integrate classical analogue and digital electronics onto silicon chips with quantum elements.

The primary project over these 6 months involves investigating the viability of using FPGA's and a custom digital hardware/software stack to replace the current methods of measuring and controlling Quantum Test Chips. The goal of this project is too utilize the FPGA as a signal generator that can quickly respond and control the Test Chip upon feedback from reflected signals, with high precision and quick response time. I also have a secondary project that involves porting the current software environment used to program the chips onto an RP2040, in order to optimize the current lab setup and test flow by making certain components more compact and automatic.

The primary goals achieved over these 6 months are:

- Building on the Quantum Instrumentation Control Kit (QICK) in both hardware and software
  - Expanding on provided FPGA custom hardware to add new exclusive functionality necessary at QMT
    - Peak-Tracking hardware control loop
    - Improved precision/range/functionality of signal generators
  - Developing software library for end users to interface with FPGA
- Improving tool-flow by porting systems to low-level C on an RP2040
  - Enable end users to interface with the RP2040 via a serial or Ethernet connection
  - Convert all communication between the RP2040 and target chip to utilize hardware communication protocols

<!-- <style>
.row {
  background-color: white;
}
</style> -->