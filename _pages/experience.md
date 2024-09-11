---
layout: page
title: Experience
permalink: /experience/
description: Growing resume of technical experiences
nav: true
nav_order: 1
---

## Research Expreiences

Below are my primary completed research projects, hopefully will add research projects from my Ph.D. at Geeorgia Tech soon!

### Georgia Insititute of Technology

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Logos/GTExtended.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

#### COMING SOON!

### Imperial College London

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Logos/IMPERIAL.png" title="Imperial Logo" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

#### Final Year Project -- Optimizing Interpretable Deep Learning

I completed my Final Year Masters Thesis under the supervision of Professors Wayne Luk and Ce Guo. I focused on quantifying and automating Interpretability for Deep Learning.  

Deep learning, particularly in the form of convolutional neural networks (CNNs), has achieved significant success in applications such as medical imaging and autonomous driving. However, the lack of interpretability in these models has limited their adoption in critical fields where transparency and trust are paramount. This research introduces **OptINN**, an optimized interpretable neural network (INN) architecture, designed to address these challenges by leveraging GPU acceleration and quantization techniques.

The key contributions are:

- **Quantifying Interpretability**: Introduced a novel metric to quantitatively assess interpretability in deep learning models, enabling an analysis of trade-offs between interpretability, accuracy, and performance.
- **Automated INN Conversion from CNNs**: Developed a generalized method to automatically convert standard CNNs into INNs with minimal performance overhead, using automated acceleration techniques to optimize for GPU execution.
- **Performance Optimization**: Demonstrated significant improvements in inference latency and accuracy. The FP16 MobileNet-V3-based OptINN achieved an 88.83% reduction in latency compared to the ResNet-50 IAIA-BL model while maintaining high interpretability. The Int-8 QAT EfficientNet-V2 OptINN exhibited a 2.17 percentage point increase in top-1 accuracy and an 80.49% latency improvement over comparable models.
The work has been written as conference paper and has been submitted to *AAAI 2025*

#### Undergraduate Research -- OptiMult

Throughout my third year at university I have been researching with the Circuits and Systems (CAS) group at Imperial College London, specifically with Ph.D. student Sam Coward, Professor George Constantinids and Professor Emeritus Miloš Ercegovac at UCLA. We investigated the usage of Equivalency Graphs (E-Graphs) in data-path optimization for multiplier circuits.  

Multiplier circuits account for significant resource usage in data-path-dominated circuit designs and RTL designers continue to build bespoke hand-crafted multiplication arrays for their particular application. The construction of an optimized multiplier presents trade-offs between pre-processing to generate a smaller array and array reduction. E-Graphs are crucially able to explore these various tradeoffs efficiently. The goal of this research project is to explore the feasibility of incorporating an E-Graph framework into a HDL compiler/synthesizer that could optimize specific multiplier expressions for either area or latency. The initial proposed e-graph tool developed in Rust - **OptiMult** - has demonstrated latency improvements against standard logic synthesis tools for multiplier expressions.

The following are some of the main results:

- Created Rewrite framework in Rust using EGG to express alternative multiplier representations via E-Graph rewrites
- Demonstrated latency reduction in arithmetic circuits against industry standard logic synthesis tools
  - 46% latency reduction in squarer circuits.
  - 9% latency reduction in general multiplier circuits.

The paper has now been presented at *ASILOMAR 2023* - available [**HERE**](https://ieeexplore.ieee.org/document/10476812)!

## Industry Expreiences

### Intel 2-Month Summer Internship - 2024

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Logos/intel_logo.png" title="Intel Logo" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The summer between graduating from Imperial and starting my Ph.D. at Georgia Tech I completed a fast-paced internship as part of the numerical hardware team in the GPU group at Intel. The group applies to modern arithemtic and hardware research to compute units withing Intel's advanced GPUs and NPUs, blending hardware and mathematics research and practical engineering.

My primary project focused on automating the optimization of mixed-precision floating point multipliers using E-Graphs, implemented in Rust. This work aimed to enhance the efficiency of multiplier designs, a critical component in Intel's GPU and NPU architectures. In parallel, I investigated strategies for minimizing glitch power in hardware designs, employing Integer Linear Programming techniques. This research is crucial for reducing energy consumption and improving the reliability of digital circuits. Additionally, I explored optimization methods for dot-product hardware units, laying the groundwork for future developments in Intel's computational hardware.

Despite the limited time, we developed promising ideas that should continue influencing future dot product and multiplier units within Intel GPUs and NPUs. The insights and skills gained from the internship were significant, sparking several hardware automation questions that will undoubtedly influence my PhD research. This experience provided invaluable exposure to industrial practices and challenges, offering a unique perspective that will shape my future work in the field.

### 6-Month Industrial Placement (CO-OP) at Quantum Motion Technologies

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Logos/QMT.png" title="QMT Logo" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

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