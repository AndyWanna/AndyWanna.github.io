---
layout: page
title: Research
permalink: /research/
description: E-graphs for hardware design automation, from arithmetic expressions to HLS programs to netlists.
nav: true
nav_order: 1
---

## Georgia Institute of Technology

### EGGROLL: Reinforcement Learning for E-Graph Exploration {#eggroll}

*Jan 2026 – present · Georgia Tech and AMD · first author, in preparation · invited demo at ARITH 2026*

Equality saturation is powerful but scales badly: on large designs the e-graph grows faster than it can be explored. EGGROLL treats e-graph exploration as a decision problem. The e-graph is the state, applying a rewrite is an action, and the reward comes from the cost of the expression extracted at the end.

- Built as a generic framework: it applies to any e-graph setup given a language, rewrite set, analyses, cost function and extraction method.
- In early experiments it matches or improves on the expressions found by exhaustive equality saturation while building far smaller e-graphs.
- It currently drives a netlist rewriting flow, guiding exploration away from e-graph blow-up on large designs.

### Lemonade: Automated HLS Design Modularization using E-Graphs {#lemonade}

*Mar 2025 – present · first author, under review*

HLS tools synthesize every program into independent hardware, so any sharing across workloads has to be engineered by hand. That is costly in ML, where models keep reusing the same kernels. Lemonade automatically discovers reusable hardware modules across structurally distinct HLS programs.

- An MLIR-based framework combining e-graphs, anti-unification, and polyhedral analysis.
- Polyhedral loop-mapping analysis derives the minimal set of sound loop transformations that expose shared modules, pruning an 8,716M-candidate space to 4,096 designs.
- Decoupled hardware-oriented cost functions: a hardware impact cost for module extraction and a performance cost for implementation.
- Reuses 38.1% of synthesized hardware across Polybench, GNN layers and transformer encoder blocks. Composed with ScaleHLS, it gives a geo-mean 47.8% lower area at iso-delay and 53.8% fewer cycles at iso-area.

An early version was presented at the [EGRAPHS workshop at PLDI 2025](https://www.youtube.com/live/AEbvKbHPRhM?si=D3sPKH6MXOo_Q5H0&t=11214) (recording).

### ForgeBench: An HLS Design Generator of ML Test Suites for Next-Generation HLS Tools {#forgebench}

*Apr 2025 – present · co-first author, under review at ACM TRETS · extends our FCCM 2026 poster*

No fixed benchmark suite stays representative as ML workloads change. ForgeBench is a generator instead: it composes synthesizable HLS C/C++ on demand from a JSON specification over an extensible ML kernel library.

- Full model-level designs for the ResNet family and LLaMA-3.1-8B, including a complete 32-layer LLM project covering prefill and decode, KV-cache and attention, validated against a NumPy golden reference.
- A 12,912-design suite across GEMM, DNN and LLM workloads spanning the area–latency space, with 2,711 designs placed and routed on a ZCU102, all meeting timing.
- A modularization suite with hand-built shared-module baselines, used to evaluate tools like Lemonade.

Using ForgeBench, we tested how well current HLS frameworks (ScaleHLS, HIDA, AutoSA, StreamHLS and Allo) handle modern ML designs. Support falls off as designs grow. On LLM designs, every tool except Allo stops at parsing.

[arXiv](https://arxiv.org/abs/2504.15185) · [code](https://github.com/hchen799/ForgeBench)

### SpecScore: Quantifying Readability of HLS-Generated RTL Using LLMs {#specscore}

*May 2026 – present · co-first author, in preparation*

HLS tools generate RTL that engineers still have to read, debug and verify, but there is no automatic way to measure how readable it is. SpecScore measures how closely tool-generated RTL follows its HLS C++ specification, using cosine similarity in a joint LLM embedding space, with no human annotation.

- Four strategies for embedding RTL that exceeds model context windows, including hierarchical module summarization.
- Validated at 0.95 mean reciprocal rank on PolyBench, MachSuite and CHStone.

### Formal Verification of Hardware Arithmetic in Lean {#lean}

*Aug 2025 – Dec 2025*

- A Rust-to-Lean 4 flow that verifies RTL arithmetic datapaths against a bitvector DSL specification. Verilog is translated through Yosys and AIGER, and equivalence is discharged with `bv_decide` and CaDiCaL.
- A type-explicit arithmetic DSL that forces a bitwidth on every wire, 3.64× more concise than equivalent RTL.
- Canonical bitwidth reconciliation, mapping hardware's n, m → k operators onto Lean's `BitVec`.

## Imperial College London

### OptiMult: Multiplier Optimization via E-Graph Rewriting {#optimult}

*Nov 2022 – Jun 2023 · with Intel and UCLA · first author, ASILOMAR 2023*

With Sam Coward, Theo Drane, Prof. George Constantinides and Prof. Miloš Ercegovac, I built OptiMult, an e-graph rewriting tool in Rust on `egg`. It explores equivalent multiplier architectures as local, equivalence-preserving rewrites and emits synthesizable Verilog.

- A dual row and column representation of AND arrays, with a two-phase optimization that uses separate rewrite sets and delay cost models in each phase to keep gate-level search tractable.
- Found non-standard compressor structures during search.
- Cut latency by up to 46% on squarers and 9% on multipliers against a commercial synthesis tool at TSMC 5nm, with every design formally verified by equivalence checking.

[Paper (IEEE Xplore)](https://ieeexplore.ieee.org/document/10476812) · [arXiv](https://arxiv.org/abs/2312.06004)

### OptINN: Breaking the Interpretability–Efficiency Trade-off for DNNs on GPUs {#optinn}

*Oct 2023 – Jun 2024 · M.Eng. thesis, supervised by Prof. Wayne Luk and Dr. Ce Guo*

Interpretable neural networks are usually too slow to deploy where interpretability matters most. OptINN makes prototype-based interpretable networks run efficiently on GPUs.

- A prototype-based architecture that recasts prototype distance as GPU-optimized convolutions with hard-sigmoid activations, giving full cuDNN and TensorRT support.
- A toolchain that compiles pretrained CNNs into optimized interpretable TensorRT engines, with principled quantize/dequantize node placement and quantization-aware training for INT8.
- Prototype interpretability holds up under quantization: the interpretability score moves by less than 0.03 from FP32 to INT8 while latency falls by up to 84.4%. MobileNet-V3 runs interpretably in 2.10 ms, against 8.35 ms for the original CNN.
