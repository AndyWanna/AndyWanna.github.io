---
layout: page
title: Experience
permalink: /experience/
description: Industry internships in numerical hardware, design automation and FPGA engineering.
nav: true
nav_order: 3
---

## AMD — Graduate Applied Researcher {#amd-gar}

*Oct 2025 – May 2028*

AMD funds my Ph.D. research directly, first through a research gift and then a sponsored research agreement. Results from the collaboration transfer into AMD's design flows.

## AMD — Numerical Hardware Engineer Intern, Summer 2026 {#amd-2026}

*May 2026 – Aug 2026 · Numerical hardware team*

My second summer with AMD's numerical hardware team took e-graph rewriting from arithmetic expressions down to fully mapped standard-cell netlists.

- Built an e-graph rewriting tool that operates on mapped netlists, reducing cell count and area.
- Scaled the flow to production netlists of over 4 million cells. The tool is now being evaluated by AMD's IP synthesis team.
- Extended ILP-based extraction so it stays tractable at netlist scale, with delay constrained, left free, or optimized.

## AMD — Numerical Hardware Engineer Intern, Summer 2025 {#amd-2025}

*May 2025 – Aug 2025 · Numerical hardware team*

The team designs and automates high-performance arithmetic units for GPUs and NPUs. My project was multiplier generation tailored to the data a multiplier will actually see.

- Designed integer and constant multiplier architectures that improve both minimum delay and area over baseline designs.
- Built an e-graph multiplier framework covering the design space of array generation and reduction, enabling hybrid multiplier architectures.
- Developed methods to generate multipliers optimized for input properties such as arrival times and toggle rates.

## Intel — Numerical Hardware Engineer Intern, Summer 2024 {#intel-2024}

*Jun 2024 – Aug 2024 · Numerical hardware team, GPU group*

Between Imperial and Georgia Tech I joined Intel's numerical hardware team, which brings arithmetic research into the compute units of Intel GPUs and NPUs.

- Automated mixed-precision floating-point multiplier optimization in Rust using e-graphs, improving PPA by up to 10%.
- Investigated glitch power minimization in hardware designs using integer linear programming.

## Quantum Motion — FPGA Engineering Co-op {#qmt-2023}

*Apr 2023 – Sep 2023 · Integrated Circuits team, London*

Quantum Motion builds qubits on standard silicon transistors. I worked on replacing the lab's equipment for measuring and controlling quantum test chips with an FPGA-based stack.

- Designed a bespoke FPGA signal generator for high-speed qubit feedback, extending the Quantum Instrumentation Control Kit (QICK) with a peak-tracking control loop and better signal-generator precision and range.
- Built a Python library on PYNQ and QICK for users to drive the FPGA.
- Ported parts of the chip-programming environment to an RP2040 microcontroller in C, communicating over TCP/IP on Ethernet.

## Quantum Motion — Analog and Digital IC Validation Intern {#qmt-2022}

*Jul 2022 – Sep 2022 · London*

- Validated ring oscillators on silicon test chips, analyzing transistor properties at room temperature and at cryogenic temperatures (2 K).
