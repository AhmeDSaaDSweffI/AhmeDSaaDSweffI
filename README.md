<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=26&duration=3500&pause=1000&color=00E0C6&center=true&vCenter=true&width=760&lines=Ahmed+Saad+Sweffi;Digital+IC+Design+%26+Verification+Engineer;A+finite+state+machine+that+runs+on+coffee." alt="Ahmed Saad Sweffi" />

<a href="https://www.linkedin.com/in/ahmed-saad-sweffi-09b2751a9"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<a href="mailto:a.s.sweffi@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
<a href="https://scholar.google.com/citations?user=sv31Gr0AAAAJ&hl=en"><img src="https://img.shields.io/badge/Scholar-4285F4?style=for-the-badge&logo=googlescholar&logoColor=white" alt="Google Scholar"/></a>
<a href="https://ieeexplore.ieee.org/author/756976241738184"><img src="https://img.shields.io/badge/IEEE-00629B?style=for-the-badge&logo=ieee&logoColor=white" alt="IEEE"/></a>

</div>

---

## 🔁 `module ahmed_sweffi` — state diagram

> Reset is optional. Coffee is not.

```mermaid
stateDiagram-v2
    direction LR
    [*] --> IDLE
    IDLE        --> COFFEE      : alarm @ 07:00
    COFFEE      --> RTL_DESIGN  : caffeine_ready
    RTL_DESIGN  --> LINT        : Verilog / SystemVerilog
    LINT        --> SIMULATE    : 0 lint violations
    SIMULATE    --> DEBUG       : sim_failed
    DEBUG       --> RTL_DESIGN  : root_cause_found
    SIMULATE    --> UVM_VERIFY  : sim_passed
    UVM_VERIFY  --> COVERAGE    : SVA + RAL + CRT
    COVERAGE    --> UVM_VERIFY  : coverage not closed
    COVERAGE    --> SIGNOFF     : coverage == 100%
    SIGNOFF     --> [*]         : tape-out 🎉
```

---

## 🗺️ Transition Legend — *(the skills firing on each edge)*

| State / Edge | Tools & skills in play |
|:--|:--|
| **RTL_DESIGN** | `Verilog` · `SystemVerilog` · HW/SW co-design |
| **LINT** | `Questa Lint` · `CDC/RDC` · STA · metastability |
| **SIMULATE** | `QuestaSim` · `ModelSim` · `Vivado` · `Quartus` |
| **UVM_VERIFY** | `UVM` · `SVA` · `RAL` · `Cocotb` · constrained-random |
| **COVERAGE** | functional + code coverage · GLS · signoff |
| **Protocols handled** | `AXI` · `AHB` · `APB` · `I2C` · `SPI` · `UART` · SerDes |
| **Also runs** | `Python` · `C/C++` · `MATLAB` · `TCL` · ML-for-HW |

```
UVM_INFO: state == SIGNOFF  →  coverage 100%,  0 bugs escaped to silicon.
```

<div align="center">

<sub>🎓 B.Sc. Electronics & Communications @ E-JUST · 🇹🇼 Incoming exchange @ NKUST · 📍 Cairo, Egypt</sub>

⭐ *Star the repo if the state machine reached SIGNOFF.*

</div>
