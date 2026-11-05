# Anish Dey
### **RTL Design & Verification Engineer | Microarchitecture & Digital ASIC/FPGA**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/AnishDey27)
[![Email](https://img.shields.io/badge/Email-anish.dey.ju%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:anish.dey.ju@gmail.com)
[![Location](https://img.shields.io/badge/Location-Kolkata%2C%20India-lightgrey?style=flat-square)](#)

---

### 📌 Summary

Undergraduate in Electronics & Telecommunication Engineering at **Jadavpur University ('27)** and former **Digital Design Intern at Texas Instruments (SITARA MPU DFT Team)**. Specializing in **RTL microarchitecture**, **Out-of-Order bus interconnects**, **Clock Domain Crossing (CDC)**, and **Assertion-Based Verification (SVA/UVM)**. Focused on designing synthesizable digital systems with deterministic latencies and self-checking verification harnesses.

---

### 🛠️ Technical Competencies

| Domain | Competencies & Technologies |
| :--- | :--- |
| **Microarchitecture & RTL** | Out-of-Order Execution, Skid Buffers, Decoupled AW/W Channels, Hazard Scoreboards, CDC (2-FF Sync, Gray Counters), Pipelining, FSMs |
| **Verification & Quality** | Constrained-Random Verification, SystemVerilog Assertions (SVA), Scoreboards, Coverage closure, Synchronous Sampling |
| **Protocols & Standards** | AMBA AXI4 / AXI4-Lite, MESI Cache Coherency, UART (16x oversampling), I²C, JTAG, DFT (ATPG, TSV analysis) |
| **Languages & Scripting** | SystemVerilog, Verilog, Python (OOP / Automation), C, TCL, Bash |
| **EDA & Verification Tools** | Synopsys (VCS, Verdi, Design Compiler), Xilinx Vivado, Verilator, Yosys, Icarus Verilog |

---

### 💼 Experience

#### **Texas Instruments** — *Digital Design Intern (SITARA MPU DFT Team)* `[May 2026 – Jul 2026]`
- **ATPG Collateral Automation:** Automated generation of 90+ ATPG collateral files (`assign`, `modeinit`, `editmodel`) from device specs using Agentic AI workflows, slashing engineering turnaround time from **3–4 weeks to ~1 hour**.
- **TSV Diagnostics at Scale:** Built an automated analysis pipeline parsing **10,000+ Test Structure Violations (TSVs)** across sub-chip and top-level designs, reducing manual review overhead by **~85%** with automated waiver justification and logic pinpointing.

---

### 🚀 Highlighted Microarchitecture & Verification Projects

#### 1. [AXI4 High-Performance Memory Slave (Microarchitecture)](https://github.com/AnishDey27)
*Synthesizable SystemVerilog IP supporting Out-of-Order Execution & Asymmetric Latencies*
- Microarchitected decoupled address (AW) and data (W) channels synchronized via **Token FIFOs** to prevent write stalling and sustain INCR burst throughput.
- Designed per-ID pending FIFOs with an integrated **Cross-Group Hazard Scoreboard** utilizing tracking counters to eliminate structural hazards and enforce in-order response dispatch.
- Implemented **pipelined skid buffers** on primary interfaces and round-robin arbitration across interleaved dual memory banks with 2-cycle and 4-cycle access latencies.

#### 2. [AXI4-Lite Slave & Verification Framework](https://github.com/AnishDey27/axi4-lite-slave-verification)
*Production-Grade Bus Slave with Multi-Threaded Directed-Random Testbench*
- Microarchitected a **"Snoop & Serialize" Hazard-Stalled FSM** enforcing strict Read-After-Write (RAW) consistency across simultaneous read/write collisions.
- Built a multi-threaded verification environment with parallel backpressure engines and a semaphore-locked scoreboard to ensure race-free transaction checking.
- Embedded protocol-checking **SystemVerilog Assertions (SVA)** and achieved 100% DUT reliability over **2,000,512 randomized cycles**.

#### 3. [MESI Cache Coherence & Performance Simulator](https://github.com/AnishDey27/mesi-cache-simulator)
*Cycle-Accurate Multi-Core Memory Subsystem Performance Engine*
- Developed a cycle-accurate, trace-driven 4-core SMP cache simulator with an integrated shared snooping bus and **Tree-PLRU** replacement algorithm.
- Validated across 8 architectural stress benchmarks, modeling **18-cycle peer-to-peer cache transfers** versus **103-cycle memory fetches**, BusRdX invalidations, and dirty-line writebacks.

#### 4. [RTL UART Transceiver with CDC Protection](https://github.com/AnishDey27)
*Robust Parameterizable Serial Interface in Verilog*
- Engineered parameterized TX/RX engines featuring **VALID/READY handshakes** and deterministic FSM data paths.
- Built a multi-stage **2-FF CDC synchronizer** paired with 16x oversampling clock recovery and hardware framing-error detection.

#### 5. [Silicon Studio IDE](https://github.com/AnishDey27/silicon-studio-ide)
*Full-Stack EDA Workspace for Automated RTL Simulation & Synthesis*
- Integrated execution pipelines for **Yosys**, **Verilator**, and **iverilog** with SkyWater 130nm / ASAP7 cell library metrics.
- Automated static rule checks for Clock Domain Crossing (CDC), FSM deadlocks, and timing constraint linting.

---

### 📊 GitHub Activity

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=AnishDey27&show_icons=true&theme=dark&count_private=true&hide_border=true" width="48%" alt="Anish's GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=AnishDey27&layout=compact&theme=dark&hide_border=true" width="48%" alt="Top Languages" />
</div>
