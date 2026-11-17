# 飞行器控制系统设计与仿真 MATLAB/Simulink 工具箱

<div align="left">
  <img src="https://img.shields.io/badge/MATLAB-R2023a%2B-blue?style=flat-square&logo=mathworks" alt="MATLAB">
  <img src="https://img.shields.io/badge/License-MIT-lightgrey?style=flat-square" alt="License">
  <img src="https://img.shields.io/badge/Platform-Windows%20%7C%20Ubuntu%20%7C%20Kylin%20%7C%20UOS-2ea44f?style=flat-square" alt="Platform">
  <img src="https://img.shields.io/badge/Status-Open%20Source-orange?style=flat-square" alt="Status">
</div>

**一套面向无人机飞控系统基于模型设计（MBD）的全流程开源 MATLAB/Simulink 工具箱，由 AFCToolBox（飞控快速开发）+ ASEToolBox（实时仿真）两大子工具箱组成，覆盖算法建模、自动代码生成、工程编译、硬件烧录、实时仿真、半实物仿真与飞行验证全链路。**

---

> 📚 **本仓库为总入口（导航页）**
>
> 两个子工具箱已拆分为**独立仓库**分别维护，各自拥有独立的版本号、更新节奏与使用文档。
> 本仓库**不存放代码与模型文件**，请从下方索引前往对应仓库获取。

## 一、工具箱索引


| 子工具箱 | 定位 | 当前版本 | 代码仓库 | 中文文档 | English |
| --- | --- | --- | --- | --- | --- |
| **AFCToolBox** | 无人机飞控快速开发工具箱 | `v6.01.251215P` | [zqhkd/AFCToolBox](https://github.com/zqhkd/AFCToolBox) | [中文文档](https://github.com/zqhkd/AFCToolBox/blob/main/README.md) | [English](https://github.com/zqhkd/AFCToolBox/blob/main/README_EN.md) |
| **ASEToolBox** | 实时仿真工具箱 | `v2.01.260417` | [zqhkd/ASEToolBox](https://github.com/zqhkd/ASEToolBox) | [中文文档](https://github.com/zqhkd/ASEToolBox/blob/main/README.md) | [English](https://github.com/zqhkd/ASEToolBox/blob/main/README_EN.md) |

> 两个工具箱相互配合，可支撑从飞控算法建模、自动代码生成、工程编译、硬件一键烧录、实时仿真、半实物仿真、台架试验到试飞验证的**全流程快速原型开发**。


## 二、能力一览

| 能力             | AFCToolBox（飞控快速开发）       | ASEToolBox（实时仿真）                    |
| -------------- | ------------------------ | ----------------------------------- |
| Simulink 可视化建模 | 开源模块库，图形化开发              | 用户模型一键部署                            |
| 自动代码生成         | 嵌入式 C 代码自动生成             | 模型编译 / 部署自动化                        |
| 工程编译           | Keil 工程一键编译、Hex 固件生成     | —                                   |
| 硬件烧录           | STLink / JLink 一键自动烧录    | —                                   |
| 实时监测           | AFCDTCom 上位机实时监测         | 运行状态实时查询（Query）                     |
| 硬实时运行环境        | —                        | Ubuntu 22.04 LTS + PREEMPT-RT 实时内核  |
| 多硬件平台          | AFC 全系飞控                 | 凌华工控机、EMB3118 / EMB3942 / EMB4940 等 |
| 仿真与测试          | SIL / HIL / 3D 视景 / 飞行试验 | 数学仿真 / 半实物仿真 / 双机仿真                 |

## 三、如何取用

1. 按需在**上方索引**中选择工具箱，进入对应仓库；
2. 在该仓库的 **Releases** 中下载对应版本发布包，或直接 `git clone` 仓库；
3. 按该仓库 `README_CN.md` 中的"部署配置 → 使用教程"章节完成环境搭建与上手；
4. **AFC 与 ASE 需同时使用时，请分别克隆两个仓库**，两者互不包含。

**环境要求**：MATLAB R2023a 或更高版本。上位机支持 Windows 10/11、银河麒麟 Kylin V10（桌面版）、统信 UOS V20（桌面版）；ASEToolBox 下位机为 Ubuntu 22.04 LTS（含 PREEMPT-RT 实时内核）或银河麒麟 Kylin V10 SP1（含实时内核）。

## 四、版本说明

- 版本号格式为 `主版本.次版本.日期编码`，如 `6.01.251215P` 表示 6.01 系列、2025-12-15 发布的 P 版；
- 各工具箱的具体版本请以对应仓库的 **Releases** 与发布目录名为准，本页版本号仅作索引；
- 本页版本号会随子仓库发布同步更新，如需历史版本请前往子仓库查看。

## 五、开源许可

本项目基于 **MIT License** 开源，所有用户可免费下载、使用、修改、二次开发，支持学生学习、个人开发等全场景使用。

- **版权**：中山大学 航空航天学院
- **环境要求**：MATLAB R2023a 或更高版本

## 六、联系与贡献

本项目由**中山大学航空航天学院 ACG 团队**基于 MATLAB/Simulink 自主研制并完全开源。代码疑问、Bug 反馈与学术合作意向，请通过以下方式联系：

- 个人邮箱（永久）：zqhkd@qq.com

> 问题反馈请在**对应子仓库**提交 Issue（AFCToolBox → AFCToolBox 仓库；ASEToolBox → ASEToolBox 仓库），便于问题归类与版本追溯。

---

*本仓库仅提供入口指引，不存放代码与模型文件。*