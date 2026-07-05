<div align="center">

<!-- Typing banner -->
<a href="https://github.com/AhmeDSaaDSweffI">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=24&duration=3200&pause=900&color=00E0C6&center=true&vCenter=true&width=720&lines=module+ahmed_sweffi+%2F*+Digital+IC+Design+%26+Verification+*%2F;100%25+functional+coverage.+0+bugs+escaped+to+silicon.;always+%40(posedge+coffee)+begin+clean_rtl+%3C%3D+1;+end" alt="typing banner" />
</a>

# `ahmed_sweffi.sv` — the human under test 🧪

**Digital IC Designer • Digital Verification Engineer**
📍 Cairo, Egypt &nbsp;|&nbsp; 🎓 E-JUST '27 &nbsp;|&nbsp; 🇯🇵→🇹🇼 Incoming Exchange @ NKUST

<a href="https://www.linkedin.com/in/ahmed-saad-sweffi-09b2751a9"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<a href="mailto:a.s.sweffi@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
<a href="https://scholar.google.com/citations?user=sv31Gr0AAAAJ&hl=en"><img src="https://img.shields.io/badge/Scholar-4285F4?style=for-the-badge&logo=googlescholar&logoColor=white" alt="Google Scholar"/></a>
<a href="https://orcid.org/0009-0006-4340-9756"><img src="https://img.shields.io/badge/ORCID-A6CE39?style=for-the-badge&logo=orcid&logoColor=white" alt="ORCID"/></a>
<a href="https://ieeexplore.ieee.org/author/756976241738184"><img src="https://img.shields.io/badge/IEEE-00629B?style=for-the-badge&logo=ieee&logoColor=white" alt="IEEE"/></a>

</div>

---

## 🔩 The DUT (Device Under Test)

> Instantiate carefully. Requires an external caffeine PLL for stable operation.

```systemverilog
`timescale 1ns / 1_lifetime

module ahmed_sweffi #(
    parameter        LOCATION   = "Cairo, Egypt",
    parameter        ROLE       = "Digital IC Design & Verification",
    parameter int    COVERAGE   = 100          // %, non-negotiable
)(
    input  logic        clk,                    // sourced from a caffeine PLL
    input  logic        coffee_in,              // active-high, mandatory
    input  logic        deadline_near,          // async assert, unfortunately
    input  logic [7:0]  spec_ambiguity,         // there is always some
    output logic        clean_rtl,              // 0 lint violations
    output logic [31:0] bugs_found,             // monotonically increasing
    output logic        bugs_escaped            // tied to 1'b0 by contract
);

    // synthesizable charisma — passes DRC & LVS
    always_ff @(posedge clk or posedge deadline_near) begin
        if (coffee_in) begin
            clean_rtl  <= 1'b1;
            bugs_found <= bugs_found + 1'b1;
        end else begin
            clean_rtl  <= 1'bx;                  // do NOT drive without coffee
        end
    end

    assign bugs_escaped = 1'b0;                  // we simply don't do that here

endmodule
```

---

## 🔁 Daily FSM (state diagram)

```mermaid
stateDiagram-v2
    [*] --> IDLE
    IDLE            --> COFFEE          : alarm @ 07:00
    COFFEE          --> RTL             : caffeine_ready
    RTL             --> SIMULATE        : compile_pass
    SIMULATE        --> DEBUG           : sim_failed
    DEBUG           --> WAVEFORM_STARE  : still_failing
    WAVEFORM_STARE  --> AHA             : signal@0x1F glitched
    AHA             --> COMMIT          : fix_applied
    COMMIT          --> DEBUG           : new_bug_found
    COMMIT          --> SLEEP           : coverage == 100%
    SLEEP           --> IDLE            : alarm
```

```text
       __    __    __    __    __    __
clk  _|  |__|  |__|  |__|  |__|  |__|  |__     // ~running on caffeine
             _______
coffee_in __|       |___________________       // rising edge REQUIRED
                    ___________
clean_rtl _________|           |__________       // asserts shortly after coffee
```

---

## ✅ UVM Scoreboard Report

```text
============================================================================
  UVM_INFO scoreboard.sv(42) @ 27yrs: comparing expected vs ahmed_actual ...
----------------------------------------------------------------------------
  COVERGROUP                         COVERAGE   GOAL   STATUS
----------------------------------------------------------------------------
  verification_skills                 100.0%    100%   [ PASS ]
  rtl_design                           98.7%    100%   [ WARN ]  // always learning
  coffee_dependency                   100.0%    100%   [ PASS ]
  bugs_escaped_to_silicon               0.0%      0%   [ PASS ]
  imposter_syndrome                    42.0%      0%   [ FAIL ]  // known, WONTFIX
----------------------------------------------------------------------------
  UVM_INFO: ** TEST PASSED **   0 UVM_ERROR   0 UVM_FATAL
============================================================================
```

---

## 🧰 Tech Stack (`import ahmed_pkg::*;`)

**HDL & Methodologies**
![SystemVerilog](https://img.shields.io/badge/SystemVerilog-DA3E52?style=for-the-badge&logo=verilog&logoColor=white)
![Verilog](https://img.shields.io/badge/Verilog-8B0000?style=for-the-badge)
![UVM](https://img.shields.io/badge/UVM-1E90FF?style=for-the-badge)
![SVA](https://img.shields.io/badge/SVA-6A5ACD?style=for-the-badge)
![Cocotb](https://img.shields.io/badge/Cocotb-3776AB?style=for-the-badge&logo=python&logoColor=white)

**Protocols & Architecture**
![AXI](https://img.shields.io/badge/AXI-005571?style=for-the-badge)
![AHB](https://img.shields.io/badge/AHB-005571?style=for-the-badge)
![APB](https://img.shields.io/badge/APB-005571?style=for-the-badge)
![I2C](https://img.shields.io/badge/I2C-005571?style=for-the-badge)
![SPI](https://img.shields.io/badge/SPI-005571?style=for-the-badge)
![UART](https://img.shields.io/badge/UART-005571?style=for-the-badge)
![SerDes](https://img.shields.io/badge/SerDes-005571?style=for-the-badge)

**Programming & Tools**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C%2FC%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=for-the-badge&logo=mathworks&logoColor=white)
![TCL](https://img.shields.io/badge/TCL-FFA500?style=for-the-badge)
![Vivado](https://img.shields.io/badge/Vivado-C7202E?style=for-the-badge&logo=xilinx&logoColor=white)
![QuestaSim](https://img.shields.io/badge/QuestaSim-005CA9?style=for-the-badge)
![Quartus](https://img.shields.io/badge/Quartus-0071C5?style=for-the-badge&logo=intel&logoColor=white)

---

## 🏗️ Featured `synthesis` (projects that actually taped out of my brain)

| Block | What it does | Coverage |
|---|---|---|
| 🧠 **NPU for Hybrid CNN-Transformer** (Grad Project, mentored by **Analog Devices**) | FPGA accelerator on Zynq-7020: 32×16 systolic PE array @ 76.8 GOPS, patch-reshape engine, SIMD post-processor, UVM block-level verification | in progress |
| 🔢 **Systolic Array** | Parameterizable weight-stationary array in SystemVerilog for CNN matmul | directed TB |
| 🔌 **I2C Design & Verify** | Master/Slave, all 4 modes, full UVM env | **100%** |
| 📡 **UART Transmitter** | FSM-based, configurable parity/baud, self-checking scoreboard | **100%** |
| 🧷 **SPI Slave + RAM** | Coverage-driven UVM, all SPI modes + memory ops | **100%** |
| 🚌 **AXI4-Lite Slave** | Layered UVM + SVA: handshaking, back-pressure, error responses | ✔ |
| 🧭 **Packet Router** | Constrained-random UVM: FIFO limits, port contention, bad headers | **100%** |
| 🗂️ **APB RAL** | UVM Register Abstraction Layer, mirroring checks | bit-field |
| ➕ **4-bit ALU** | Low-latency arith/logic + dynamic flags, transaction-level UVM | ✔ |
| 🚦 **Traffic Light FSM** | 4-way intersection on Altera Cyclone III, 7-seg driver | sim ✔ |
| ⚙️ **DSP48A1 Slice** | Configurable slice on Spartan-6, 100 MHz closure, 0 lint | **100%** |

---

## 📄 Publications

- **Sweffi, A. S.**, et al. *Spider IoT-Based Wearable Remote Health Monitoring System Using Machine Learning*, **JAC-ECC 2025**, Alexandria, Egypt. [`DOI: 10.1109/JAC-ECC67970.2025.11417567`](https://doi.org/10.1109/JAC-ECC67970.2025.11417567)
- 🕸️ *On progress* — **Spider IoT V2**: multi-modal sensing + optimized on-device ML.
- 🍅 *On progress* — **Tomato Plant Disease Detection**: real-time edge inference (YOLOv10 + MobileNetV2).

---

<div align="center">

## 📊 Post-Synthesis Reports

<img height="165" src="https://github-readme-stats.vercel.app/api?username=AhmeDSaaDSweffI&show_icons=true&hide_border=true&title_color=00E0C6&icon_color=00E0C6&theme=tokyonight" alt="stats"/>
<img height="165" src="https://github-readme-streak-stats.herokuapp.com/?user=AhmeDSaaDSweffI&hide_border=true&stroke=00E0C6&ring=00E0C6&fire=00E0C6&currStreakLabel=00E0C6&background=1A1B27" alt="streak"/>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=AhmeDSaaDSweffI&layout=compact&hide_border=true&title_color=00E0C6&theme=tokyonight" alt="top langs" height="150"/>

</div>

---

<div align="center">

```systemverilog
initial begin
    $display("Thanks for reading the testbench of my life.");
    $display("If bugs_escaped != 0, it was a feature.");
    $finish;
end
```

⭐ *Star a repo if the waveform made sense.*

</div>
