# Anish Dey
### Digital IC Design & Verification Engineer | Microarchitecture & RTL

<p align="left">
  <a href="https://linkedin.com/in/deyanish"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:anish.dey.ju@gmail.com"><img src="https://img.shields.io/badge/Email-anish.dey.ju%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://github.com/AnishDey27"><img src="https://img.shields.io/badge/GitHub-AnishDey27-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub" /></a>
  <img src="https://img.shields.io/badge/Location-Kolkata%2C%20India-lightgrey?style=flat-square" alt="Location" />
</p>

---

### 📌 Profile
Undergraduate in Electronics & Telecommunication Engineering at **Jadavpur University ('27)** and former **Digital Design Intern at Texas Instruments (SITARA MPU DFT Team)**. Specializing in synthesizable RTL microarchitecture, Out-of-Order bus interconnects, Clock Domain Crossing (CDC), and Assertion-Based Verification (SVA).

---

### 🛠️ Technical Skills

* **Core Domains:** ASIC/FPGA Digital Design, Microarchitecture, Out-of-Order Execution, Pipelining, Clock Domain Crossing (CDC), Static Timing Analysis (STA), CMOS Design, Design for Testability (DFT)
* **Verification:** Functional Verification, Directed-Random Testing, Assertion-Based Verification (SVA), Constrained-Random Regressions, Scoreboards & Coverage Closure
* **Protocols & Standards:** AMBA AXI4 / AXI4-Lite, MESI Cache Coherence, UART, I²C, JTAG
* **Languages & Scripting:** SystemVerilog, Verilog, C, Python (OOP), TCL, Bash
* **EDA Tools & Platforms:** Synopsys (VCS, Verdi, Design Compiler), Xilinx Vivado, Verilator, Yosys, Icarus Verilog, Linux

---

### 💼 Industry Experience

#### **Texas Instruments** — *Digital Design Intern (SITARA MPU DFT Team)* `[May 2026 – Jul 2026]`
* **ATPG Collateral Automation:** Automated generation of 90+ ATPG collateral files (`assign`, `modeinit`, `editmodel`) from device specs using Agentic AI, cutting engineering turnaround time from **3–4 weeks to ~1 hour**.
* **Large-Scale TSV Analysis:** Built an automated analysis pipeline parsing **10,000+ Test Structure Violations (TSVs)** across sub-chip and top-level designs, slashing manual review overhead by **~85%** via automated waiver justification.

---

### 🚀 Key Microarchitecture & Verification Projects

#### 1. [Silicon Studio IDE](https://github.com/AnishDey27/silicon-studio-ide) `Python | Yosys | Verilator | Sky130`
* Full-stack EDA workspace integrating **Yosys**, **Verilator**, and **iverilog** with SkyWater 130nm and ASAP7 PDK libraries.
* Automated rule checking for Clock Domain Crossing (CDC) synchronization, FSM deadlocks, and synthesis timing constraints.

#### 2. [AXI4 High-Performance Memory Slave](https://github.com/AnishDey27) `SystemVerilog`
* Architected a synthesizable AXI4 slave IP supporting **Out-of-Order execution** and non-blocking INCR bursts.
* Decoupled AW and W channels synchronized via **Token FIFOs**; integrated **pipelined skid buffers** on primary interfaces.
* Engineered per-ID pending FIFOs with a **Cross-Group Hazard Scoreboard** to prevent structural hazards and guarantee in-order completion across interleaved memory groups with asymmetric (2/4-cycle) access latencies.

#### 3. [AXI4-Lite Slave & Verification Framework](https://github.com/AnishDey27/axi4-lite-slave-verification) `SystemVerilog | Python | Vivado`
* Microarchitected a **"Snoop & Serialize" Hazard-Stalled FSM** enforcing strict Read-After-Write (RAW) consistency across simultaneous read/write collisions.
* Built a multi-threaded verification testbench with parallel backpressure engines and a semaphore-locked scoreboard.
* Validated protocol compliance with embedded **SystemVerilog Assertions (SVA)**, achieving **100% DUT reliability over 2,000,512 randomized cycles**.

#### 4. [MESI Cache Protocol & Systems Simulator](https://github.com/AnishDey27/mesi-cache-simulator) `Python`
* Developed a cycle-accurate, trace-driven 4-core SMP cache simulator with a shared snooping bus and **Tree-PLRU** eviction policy.
* Modeled latency penalties across 8 stress scenarios, contrasting **18-cycle peer-to-peer transfers** against **103-cycle memory fetches**, BusRdX invalidations, and dirty writebacks.

#### 5. [RTL UART Transceiver (Tx & Rx)](https://github.com/AnishDey27/uart_tx_rtl) `Verilog | Vivado`
* Parameterized UART transceiver core with deterministic FSM datapaths and standard VALID/READY handshakes.
* Implemented a **2-stage CDC synchronizer**, **16x oversampling** clock recovery, and hardware framing-error detection.
