---
layout: page
title: Research
permalink: /research/
description: Growing resume of research experience
nav: true
nav_order: 1
---

## Georgia Insititute of Technology

<!-- <div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Logos/GTExtended.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div> -->

### Lemonade -- Automated High-Level Synthesis Design Modularization using E-Graphs

High-Level Synthesis (HLS) tools have revolutionized hardware development for specialized accelerators, but they fundamentally lack support for designing *reusable architectures*. Every HLS program is currently synthesized into independent hardware, forcing designers to manually engineer any potential sharing across different workloads. This limitation is particularly restrictive in fast-evolving fields like machine learning, where core computational kernels are often shared but require separate, redundant hardware implementations. To bridge this gap, we introduced **Lemonade**, a framework that automatically identifies and modularizes common hardware components across a set of HLS programs, enabling true architectural design directly within the HLS workflow.

The key contributions are:

- **Automated Modularization**:  We combine hardware-oriented E-Graph exploration with Anti-Unification to automatically identify and extract synthesizable hardware modules from multiple HLS designs.
- **Scalable Loop Transformation**: We integrate polyhedral loop analysis to determine the soundness and optimal reuse opportunities within nested loop structures, making the exploration tractable.
- **Hardware-Aware Extraction**: We propose a decoupled extraction flow using customizable cost functions that prioritize the usefulness (area/delay span) and synthesizability of learned modules over simple code compression.

This work was initially presented at the *EGRAPH* workshop at *PLDI 2025* - available [**HERE**](https://www.youtube.com/live/AEbvKbHPRhM?si=D3sPKH6MXOo_Q5H0&t=11214)!

## Imperial College London

<!-- <div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Logos/IMPERIAL.png" title="Imperial Logo" class="img-fluid rounded z-depth-1" %}
    </div>
</div> -->

### Final Year Project -- Optimizing Interpretable Deep Learning

I completed my Final Year Masters Thesis under the supervision of Professors Wayne Luk and Ce Guo. I focused on quantifying and automating Interpretability for Deep Learning.  

Deep learning, particularly in the form of convolutional neural networks (CNNs), has achieved significant success in applications such as medical imaging and autonomous driving. However, the lack of interpretability in these models has limited their adoption in critical fields where transparency and trust are paramount. This research introduces **OptINN**, an optimized interpretable neural network (INN) architecture, designed to address these challenges by leveraging GPU acceleration and quantization techniques.

The key contributions are:

- **Quantifying Interpretability**: Introduced a novel metric to quantitatively assess interpretability in deep learning models, enabling an analysis of trade-offs between interpretability, accuracy, and performance.
- **Automated INN Conversion from CNNs**: Developed a generalized method to automatically convert standard CNNs into INNs with minimal performance overhead, using automated acceleration techniques to optimize for GPU execution.
- **Performance Optimization**: Demonstrated significant improvements in inference latency and accuracy. The FP16 MobileNet-V3-based OptINN achieved an 88.83% reduction in latency compared to the ResNet-50 IAIA-BL model while maintaining high interpretability. The Int-8 QAT EfficientNet-V2 OptINN exhibited a 2.17 percentage point increase in top-1 accuracy and an 80.49% latency improvement over comparable models.

### Undergraduate Research -- OptiMult

Throughout my third year at university I have been researching with the Circuits and Systems (CAS) group at Imperial College London, specifically with Ph.D. student Sam Coward, Professor George Constantinids and Professor Emeritus Miloš Ercegovac at UCLA. We investigated the usage of Equivalency Graphs (E-Graphs) in data-path optimization for multiplier circuits.  

Multiplier circuits account for significant resource usage in data-path-dominated circuit designs and RTL designers continue to build bespoke hand-crafted multiplication arrays for their particular application. The construction of an optimized multiplier presents trade-offs between pre-processing to generate a smaller array and array reduction. E-Graphs are crucially able to explore these various tradeoffs efficiently. The goal of this research project is to explore the feasibility of incorporating an E-Graph framework into a HDL compiler/synthesizer that could optimize specific multiplier expressions for either area or latency. The initial proposed e-graph tool developed in Rust - **OptiMult** - has demonstrated latency improvements against standard logic synthesis tools for multiplier expressions.

The following are some of the main results:

- Created Rewrite framework in Rust using EGG to express alternative multiplier representations via E-Graph rewrites
- Demonstrated latency reduction in arithmetic circuits against industry standard logic synthesis tools
  - 46% latency reduction in squarer circuits.
  - 9% latency reduction in general multiplier circuits.

The paper has now been presented at *ASILOMAR 2023* - available [**HERE**](https://ieeexplore.ieee.org/document/10476812)!
