# A Curated List of PIM Simulators, Frameworks, and Benchmarks

This repository contains a curated and categorized list of academic and industrial tools for simulating, modeling, and benchmarking Processing-in-Memory (PIM) systems. The list is organized to help researchers, students, and engineers navigate the PIM research landscape.

---

## 🏛️ 1. Architectural PIM Simulators

Detailed, often cycle-accurate simulators for modeling digital PIM architectures integrated with host processors. They are essential for system-level research and hardware/software co-design.

| Name | Description | Resources |
|---|---|---|
| **ASTRA-sim** | A comprehensive simulator for large-scale systems with distributed accelerators, modeling both computation and network-on-chip (NoC) communication. | [Paper](https://arxiv.org/pdf/2303.14006) \| [Code](https://github.com/astra-sim/astra-sim) \| [Website](https://astra-sim.github.io/) |
| **CLAPPS** | A cross-layer simulation approach for PIM-enabled systems, modeling interactions from the application down to the hardware. | [Paper](https://web.inf.ufpr.br/mazalves/wp-content/uploads/sites/13/2019/10/samos2017.pdf) |
| **PIMCoSim** | A system-level co-simulation platform based on RISC-V for evaluating PIM systems. | [Paper](https://www.mdpi.com/2079-9292/13/23/4795) |
| **PIMSim** | A gem5-based simulator for a PIM architecture featuring PIM-enabled instructions and a specialized memory controller. | [Paper](https://ieeexplore.ieee.org/document/8567968) \| [Code](https://github.com/vineodd/PIMSim) |
| **PimSimNN** | A comprehensive simulator for evaluating both digital PIM and analog CIM-based neural network accelerators. | [Paper](https://arxiv.org/pdf/2402.18089) \| [Code](https://github.com/wangxy-2000/pimsim-nn) |
| **gem5-ndp** | A gem5-based simulator extension to model and evaluate near-data processing architectures. | [Paper](https://hpcas.inesc-id.pt/~handle/papers/Conf_SBAC-PAD_2022.pdf) |
| **NDPmulator** | A gem5-based framework for evaluating NDP architectures, with a focus on operating system and coherence support. | [Paper](https://hpcas.inesc-id.pt/~unify/papers/journal_access24a.pdf) \| [Code](https://github.com/hpc-ulisboa/NDPmulator) |
| **Sim2pim** | A gem5 extension designed to evaluate PIM architectures by modeling PIM-enabled instructions and memory controllers. | [Paper](https://web.inf.ufpr.br/mazalves/wp-content/uploads/sites/13/2022/06/JSA2022.pdf) \| [Paper2](https://past.date-conference.com/proceedings-archive/2021/pdf/1725.pdf) |
| **M2NDP** | A gem5-based framework for exploring data movement and management in Multi-Module Near-Data Processing systems. | [Paper](https://arxiv.org/pdf/2404.19381) \| [Code](https://github.com/PSAL-POSTECH/M2NDP-public) |
| **Extended gem5** | A version of gem5 extended with timing-accurate models for HBM2-based PIM like Samsung's Aquabolt. | [Paper](https://www.degruyterbrill.com/document/doi/10.1515/itit-2023-0019/html?lang=en) |
| **Pimsimulator** | A simulator for Samsung's HBM2-PIM (FUNK) architecture, providing a performance and functional model. | [Code](https://github.com/SAITPublic/PIMSimulator) |
| **PiMsimulation** | A functional simulator developed in C++ for exploring basic Processing-in-Memory operations. | [Code](https://github.com/RohSiHyun/PiMsimulation) |
| **uPIMulator** | A cycle-accurate simulator specifically for the UPMEM PIM architecture, modeling its DPU (DRAM Processing Unit) cores. | [Paper](https://arxiv.org/pdf/2308.00846) \| [Code](https://github.com/VIA-Research/uPIMulator) |
| **MPU-Sim** | A simulator for a "Memory Processing Unit" (MPU), an architecture that adds compute capabilities to the memory controller. | [Paper](https://jyhuang91.github.io/papers/cal2021-mpusim.pdf) \| [Code](https://github.com/GD06/mpu-sim_distribution) |
| **MultiPIM** | A framework designed to simulate and evaluate systems that integrate multiple heterogeneous PIM architectures. | [Paper](https://www.sihangliu.com/docs/MultiPIM_CAL.pdf) \| [Code](https://github.com/Systems-ShiftLab/MultiPIM) |
| **Proteus** | A fast and accurate simulator for heterogeneous PIM architectures, including support for modern ReRAM-based designs. | [Paper](https://hpcrl.github.io/ICS2025-webpage/program/Proceedings_ICS25/ics25-60.pdf) \| [Code](https://github.com/CMU-SAFARI/Proteus) |
| **MIMDRAM** | A simulator for a novel PIM architecture enabling MIMD (Multiple Instruction, Multiple Data) execution inside DRAM. | [Paper](https://arxiv.org/pdf/2402.19080) \| [Code](https://github.com/CMU-SAFARI/MIMDRAM) |
| **SMCSim** | A detailed, cycle-accurate simulator for systems using Smart Memory Cubes for near-memory processing. | [Paper1](https://kluedo.ub.rptu.de/frontdoor/deliver/index/docId/4324/file/_FINAL_W07.11.4.pdf) \| [Paper2](https://cs.brown.edu/people/acrotty/pubs/3490148.3538591.pdf) \| [Code](https://github.com/salilkapur/SMCSim) |
| **NATSA** | A simulator for a near-data accelerator specifically designed for time-series analysis workloads. | [Paper](https://people.inf.ethz.ch/omutlu/pub/NATSA_time-series-analysis-near-data_iccd20.pdf) \| [Code](https://github.com/CMU-SAFARI/NATSA) |
| **PIMSys** | A PIM simulation platform focused on system-level integration, including OS and runtime aspects. | [Paper](https://dl.acm.org/doi/full/10.1145/3695794.3695797) |
| **HMC-Sim-2.0** | A simulator for the Hybrid Memory Cube (HMC), an early 3D-stacked memory architecture that enabled near-memory computation. | [Paper](https://ieeexplore.ieee.org/document/7529923) |
| **LLMServingSim** | A system-level simulator for evaluating LLM serving infrastructures, with the capability to model PIM-based hardware. | [Paper](https://arxiv.org/pdf/2408.05499) \| [Code](https://github.com/casys-kaist/llmservingsim) |
| **Wave-PIM** | A simulator for a novel PIM architecture that uses analog waveform processing for scientific computing applications. | [Paper](https://lca.ece.utexas.edu/pubs/ICPP_21_Wave_PIM.pdf) |

---

## 🧠 2. Analog, Neuromorphic & In-Memory Compute (CIM/AIMC) Simulators

Simulators for PIM based on emerging non-volatile memories (ReRAM, MRAM) and analog computing, primarily used for accelerating AI/ML workloads.

| Name | Description | Resources |
|---|---|---|
| **IBM Analog Kit** | A Python toolkit for simulating analog AI accelerators, allowing exploration of device non-idealities and training algorithms. | [Docs](https://aihwkit.readthedocs.io/en/latest/) \| [Code](https://github.com/IBM/aihwkit) |
| **NeuroSim for PIM** | An extension of the popular NeuroSim framework to model and evaluate PIM systems for AI applications. | [Paper](https://www.frontiersin.org/journals/artificial-intelligence/articles/10.3389/frai.2021.659060/full) \| [Code](https://github.com/neurosim/DNN_NeuroSim_V2.1) |
| **MemTorch** | A PyTorch-based library for simulating the behavior of memristive crossbar arrays, designed for deep learning research. | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0925231222002053) \| [Code](https://github.com/coreylammie/MemTorch) |
| **3D CiM LLM Sim** | A simulator from IBM for evaluating Mixture-of-Experts (MoE) models on an abstract 3D analog-in-memory compute (AIMC) system. | [Paper](https://www.nature.com/articles/s43588-024-00753-x) \| [Code](https://github.com/IBM/3D-CiM-LLM-Inference-Simulator) |
| **PUMA** | A framework for evaluating PIM accelerators that use memristor crossbars, considering microarchitectural effects. | [Paper](https://arxiv.org/pdf/1901.10351) |
| **CIM-SIM** | A simulator designed for Compute-in-Memory architectures, focused on modeling the performance of CIM macros. | [Paper](https://dl.acm.org/doi/10.1145/3323439.3323989) |
| **PipeLayer** | A simulator for resistive cross-point array accelerators, modeling pipelined execution for neural networks. | [Paper](https://ieeexplore.ieee.org/abstract/document/7920854) |
| **RAPIDNN** | A framework for high-throughput DNN inference using analog memory devices, modeling system-level performance. | [Paper](https://arxiv.org/pdf/1806.05794) |
| **DL-RSIM** | A simulation framework for exploring deep learning accelerators based on Resistive RAM (ReRAM) technology. | [Paper](https://ieeexplore.ieee.org/document/8587661) |

---

## 🏭 3. Commercial & Product-Specific Simulators

Simulators and software frameworks released by companies to enable development on their specific PIM hardware.

| Name | Description | Resources |
|---|---|---|
| **UPMEM SDK Func Sim**| A functional simulator in the UPMEM SDK for developing and debugging applications for UPMEM DPUs without hardware. | [Explanation](https://events.safari.ethz.ch/heart24-memorycentric-tutorial/lib/exe/fetch.php?media=heart_2024_pim_tutorial_handout.pdf) |
| **UPMEM LLM Framework** | A software framework (not a simulator) demonstrating how to run large language models on UPMEM's PIM hardware. | [Code1](https://github.com/upmem/dpu_demo) \| [Code2](https://github.com/upmem/upmem_llm_framework) |
| **SK hynix AiM Sim** | A simulator for the SK hynix Accelerator-in-Memory (AiM) architecture based on GDDR6-AiM memory. | [Paper](https://arxiv.org/pdf/2402.07578) \| [Code](https://github.com/arkhadem/aim_simulator) |

---

## 📈 4. Performance, Power, & Area Modeling Frameworks

Tools that use analytical or ML-based models to quickly estimate PIM system metrics without detailed simulation.

| Name | Description | Resources |
|---|---|---|
| **NAPEL** | A machine learning-based framework to rapidly predict the performance and energy of near-memory processing systems. | [Paper](https://people.inf.ethz.ch/omutlu/pub/NAPEL-near-memory-computing-performance-prediction-via-ML_dac19.pdf) |
| **MNSIM 2.0** | A framework for benchmarking and modeling various neuromorphic computing architectures, including PIM-based ones. | [Paper](https://ieeexplore.ieee.org/document/10058114) \| [Code](https://github.com/thu-nics/MNSIM-2.0) |
| **Statistical DRAM Model** | A methodology for building statistical models of DRAM behavior for faster and more scalable system simulation. | [Paper](https://dl.acm.org/doi/pdf/10.1145/3357526.3357576) |

---

## 🧱 5. Foundational Memory Simulators (Essential Context)

Crucial memory simulators that model standard DRAM and NVM, often used as a base for PIM simulators.

| Name | Description | Resources |
|---|---|---|
| **Ramulator** | A fast and extensible DRAM simulator supporting a wide variety of standards (DDR3/4, LPDDR3/4, HBM, etc.). | [Paper](https://people.inf.ethz.ch/omutlu/pub/ramulator_dram_simulator-ieee-cal15.pdf) \| [Code](https://github.com/CMU-SAFARI/ramulator) |
| **Ramulator 2.0** | The next-generation Ramulator with improved flexibility for modern memory standards and PIM substrates. | [Paper](https://arxiv.org/pdf/2308.11030) \| [Code](https://github.com/CMU-SAFARI/ramulator2) |
| **DRAMsim3** | A cycle-accurate DRAM simulator that models timing, power, and thermal behavior. | [Paper](https://ieeexplore.ieee.org/document/8999595) \| [Code](https://github.com/umd-memsys/DRAMsim3) |
| **NVMain** | A detailed architectural simulator for emerging non-volatile memories like Phase-Change Memory (PCM) and ReRAM. | [Paper](https://ieeexplore.ieee.org/document/6296505) \| [Code](https://github.com/SEAL-UCSB/NVmain) |

---

## 🔬 6. PIM Benchmark Suites

Collections of workloads and applications designed to evaluate the performance and efficiency of PIM systems.

| Name | Description | Resources |
|---|---|---|
| **PIMeval / PIMbench** | A comprehensive benchmark suite (PIMbench) and evaluation framework (PIMeval) for assessing PIM architectures. | [Paper](https://www.cs.virginia.edu/venkat/papers/iiswc2024.pdf) \| [Code](https://github.com/UVA-LavaLab/PIMeval-PIMbench) |
| **PrIM** | A suite of 16 PIM-friendly applications, designed to highlight the benefits and characteristics of PIM computation. | [Paper](https://arxiv.org/pdf/2404.08810) \| [Code](https://github.com/amair-lab/PriM) |
| **InSituBench** | A benchmark suite focused on in-situ processing, a key concept in PIM where computation happens where data resides. | N/A |
| **IRAM** | An early benchmark concept related to "Intelligent RAM," a precursor to modern PIM. | N/A |

---

## 📜 7. Theoretical Models & Abstractions

Works that define theoretical foundations, programming models, or high-level architectural concepts for PIM.

| Name | Description | Resources |
|---|---|---|
| **The PIM Model**| A theoretical paper that formally defines the PIM model of computation and analyzes algorithm complexity. | [Paper](https://www.cs.ucr.edu/~ygu/papers/SPAA21/PIM.pdf) |
| **V-PIM** | A high-level model proposing a PIM-based accelerator design for video analytics. | [Paper](https://ceca.pku.edu.cn/docs/20181223162256557204.pdf) |
| **GNN-PIM** | A high-level model proposing a PIM-based accelerator design for Graph Neural Networks. | [Paper](https://ceca.pku.edu.cn/docs/20200915165942122459.pdf) |

---

## ⚙️ 8. Synthesis & Design Automation Tools

Tools that automate the process of creating PIM hardware designs from high-level descriptions.

| Name | Description | Resources |
|---|---|---|
| **PIMSYN** | A synthesis framework that automatically generates Verilog code for PIM accelerators. | [Paper](https://arxiv.org/pdf/2402.18114) |

---

## How to Contribute

Found a tool that's missing? Notice an error in a link? Please open an issue or submit a pull request! We welcome contributions to keep this list accurate and up-to-date.