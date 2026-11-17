# Aircraft Flight Control System Design and Simulation MATLAB/Simulink Toolbox

<div align="left">
  <img src="https://img.shields.io/badge/MATLAB-R2023a%2B-blue?style=flat-square&logo=mathworks" alt="MATLAB">
  <img src="https://img.shields.io/badge/License-MIT-lightgrey?style=flat-square" alt="License">
  <img src="https://img.shields.io/badge/Platform-Windows%20%7C%20Ubuntu%20%7C%20Kylin%20%7C%20UOS-2ea44f?style=flat-square" alt="Platform">
  <img src="https://img.shields.io/badge/Status-Open%20Source-orange?style=flat-square" alt="Status">
</div>

**An end-to-end open-source MATLAB/Simulink toolbox for UAV flight-control systems based on Model-Based Design (MBD). It is composed of two sub-toolboxes — AFCToolBox for rapid flight-controller development and ASEToolBox for real-time simulation — covering the complete chain: algorithm modelling, automatic code generation, project build, hardware flashing, real-time simulation, hardware-in-the-loop simulation and flight validation.**

---

> 📚 **This repository is the entry page (navigation hub)**
>
> Both sub-toolboxes are maintained in **separate repositories**, each with its own versioning, release cadence and documentation.
> This repository **holds no code or model files** — use the index below to reach the relevant repository.

## 1. Toolbox Index


| Sub-toolbox | Scope | Current version | Repository | Chinese docs | English |
| --- | --- | --- | --- | --- | --- |
| **AFCToolBox** | Rapid UAV flight-controller development toolbox | `v6.01.251215P` | [zqhkd/AFCToolBox](https://github.com/zqhkd/AFCToolBox) | [中文文档](https://github.com/zqhkd/AFCToolBox/blob/main/AFCToolBox-README_CN.md) | [English](https://github.com/zqhkd/AFCToolBox/blob/main/AFCToolBox-README_EN.md) |
| **ASEToolBox** | Real-time simulation toolbox | `v2.01.260417` | [zqhkd/ASEToolBox](https://github.com/zqhkd/ASEToolBox) | [中文文档](https://github.com/zqhkd/ASEToolBox/blob/main/ASEToolBox-README_CN.md) | [English](https://github.com/zqhkd/ASEToolBox/blob/main/ASEToolBox-README_EN.md) |

> Together, the two toolboxes support **full-chain rapid prototyping**: flight-control algorithm modelling, automatic code generation, project build, one-click hardware flashing, real-time simulation, hardware-in-the-loop simulation, bench testing and flight validation.

## 2. Capabilities at a Glance

| Capability | AFCToolBox (rapid flight-controller development) | ASEToolBox (real-time simulation) |
| --- | --- | --- |
| Simulink visual modelling | Open-source block libraries, graphical development | One-click deployment of the user model |
| Automatic code generation | Automatic embedded C code generation | Automated model compilation / deployment |
| Project build | One-click Keil project build, Hex firmware generation | — |
| Hardware flashing | One-click automatic flashing via STLink / JLink | — |
| Real-time monitoring | Real-time monitoring with the AFCDTCom ground software | Real-time run-status query (Query) |
| Hard real-time runtime | — | Ubuntu 22.04 LTS + PREEMPT-RT real-time kernel |
| Multi-hardware support | The whole AFC flight-controller family | ADLINK industrial PCs, EMB3118 / EMB3942 / EMB4940, etc. |
| Simulation and testing | SIL / HIL / 3D visualisation / flight test | Numerical simulation / HIL simulation / dual-unit simulation |

## 3. How to Use

1. Pick the toolbox you need from the **index above** and open its repository;
2. Download the matching release from that repository's **Releases**, or `git clone` it directly;
3. Follow the "deployment → tutorial" chapters in that repository's `README_EN.md` to set up and get started;
4. **To use AFC and ASE together, clone both repositories separately** — neither bundles the other.

**Requirements**: MATLAB R2023a or later. The host machine supports Windows 10/11, Kylin V10 (Desktop) and UOS V20 (Desktop); the ASEToolBox target machine runs Ubuntu 22.04 LTS (with the PREEMPT-RT real-time kernel) or Kylin V10 SP1 (with the real-time kernel).

## 4. Versioning

- Version numbers follow `major.minor.date-code`, e.g. `6.01.251215P` means the P release of the 6.01 series published on 2025-12-15;
- Always treat the **Releases** page and the release folder name of each sub-repository as authoritative; the versions on this page are an index only;
- This page is updated whenever the sub-repositories publish a new release; for historical versions, refer to the sub-repository.

## 5. License

This project is released under the **MIT License**. Anyone may download, use, modify and extend it free of charge — suitable for student learning, personal projects and many other scenarios.

- **Copyright:** School of Aeronautics and Astronautics, Sun Yat-sen University
- **Requirements:** MATLAB R2023a or later

## 6. Contact and Contribution

This project was developed in-house by the **ACG team, School of Aeronautics and Astronautics, Sun Yat-sen University**, on top of MATLAB/Simulink, and is fully open-source. For implementation questions, bug reports or academic collaboration, please get in touch:

- **Email:** zqhkd@qq.com

> Please open Issues in the **relevant sub-repository** (AFCToolBox issues → AFCToolBox repository; ASEToolBox issues → ASEToolBox repository) so they can be triaged and traced per version.

---

*This repository only provides entry guidance and holds no code or model files.*