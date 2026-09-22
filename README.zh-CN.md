<div align="center">

由 **[OPENSAT](https://github.com/Satellite-OSS)** 开源卫星社区维护的一份开源卫星仿真软件清单。

[![Total views](https://raw.githubusercontent.com/Satellite-OSS/.github/main/traffic/SatelliteSimulationSoftware.svg)](https://github.com/Satellite-OSS/.github/blob/main/traffic/SatelliteSimulationSoftware.csv "Cumulative recorded repository views; updated hourly")
[![Discussions](https://img.shields.io/badge/Discussions-Join%20the%20Community-2ea44f?style=flat-square&logo=github)](https://github.com/orgs/Satellite-OSS-BUPT/discussions)
[![README](https://img.shields.io/badge/README-English-blue?style=flat-square)](README.md)

[English](README.md) | **中文**

</div>

---

## 📋 关于这份清单

卫星科研与工程中的通信网络、星座运行、轨道动力学以及射频、电磁建模等场景，需要使用不同的仿真工具。本仓库汇集**三个仿真方向的 26 个开源项目**，其中 4 个面向 SDR 的项目交叉收录，共有 30 个分类位置，帮助研究人员和开发者在查阅各项目一手文档前快速发现适用工具。

这里收录的均为**第三方链接**：项目由其原始团队或组织维护。本仓库是导航式资源汇总，并不分发软件；来源范围和链接核验记录见[范围与来源](#范围与来源)。

---

## 🎯 入选标准

1. 与卫星通信、轨道分析、射频、SDR、电磁或航天器仿真工作流直接相关
2. 具有开源项目、一手代码仓库、官方项目页或持续维护的文档
3. 至少支持一类实际工作流：仿真、建模、协议评估、任务分析、信号生成或工程验证

---

## 第三方仿真软件

以下项目按主要仿真工作流组织为卫星通信网络与协议、轨道分析与任务动力学、射频/SDR/电磁仿真三类。部分 SDR 工具会在适用时交叉收录。

<details>
<summary><strong>目录</strong></summary>

- [关于这份清单](#关于这份清单)
- [入选标准](#入选标准)
- [快速索引](#快速索引)
- [卫星通信网络与协议仿真](#卫星通信网络与协议仿真) · 16
- [轨道分析与任务动力学](#轨道分析与任务动力学) · 6
- [射频、SDR 与电磁仿真](#射频sdr-与电磁仿真) · 8 个分类位置，其中 4 个交叉收录
- [如何选择](#如何选择)
- [范围与来源](#范围与来源)
- [参与贡献](#参与贡献)
- [许可](#许可)

</details>

## 快速索引

#### [卫星通信网络与协议仿真](#卫星通信网络与协议仿真) <sup>16 个工具</sup>

- [**OpenSAND**](#opensand) — 端到端卫星通信系统仿真
- [**CosmicBeats-Simulator**](#cosmicbeats-simulator) — 多领域空间系统仿真
- [**icarus-ndnsim**](#icarus-ndnsim) — 基于 ns-3 的 LEO 星座 NDN 仿真
- [**LSNS**](#lsns) — 大规模卫星网络仿真
- [**SatSIM**](#satsim) — 多卫星仿真与可视化
- [**SNK**](#snk) — 星座网络性能仿真

#### [轨道分析与任务动力学](#轨道分析与任务动力学) <sup>6 个工具</sup>

- [**Celestia**](#celestia) — 三维天体与卫星可视化
- [**Skyfield**](#skyfield) — 高精度天文与卫星位置计算
- [**GMAT**](#gmat) — 任务分析
- [**Orekit**](#orekit) — 空间飞行动力学库

#### [射频、SDR 与电磁仿真](#射频sdr-与电磁仿真) <sup>8 个分类位置，其中 4 个来自网络仿真分类的交叉收录</sup>

- [**GNU Radio**](#gnu-radio) — SDR 开发与仿真
- [**gr-dvbs2rx**](#gr-dvbs2rx) — SDR DVB-S2 接收机实现
- [**MEEP**](#meep) — 电磁传播仿真
- [**openEMS**](#openems) — 电磁与天线仿真

## 卫星通信网络与协议仿真

| 项目 | 来源中的分类或用途 | 一手项目链接 |
| --- | --- | --- |
| **OpenSAND** | 端到端卫星通信系统仿真；来源特别提及 DVB-RCS2 与 DVB-S2。 | [GitHub](https://github.com/CNES/opensand) · [官网](https://www.opensand.org/) |
| **CosmicBeats-Simulator** | 覆盖轨道动力学、无线通信、物联网、计算与成像场景的空间系统仿真。 | [GitHub](https://github.com/vismay2303/CosmicBeats-Simulator) |
| **icarus-ndnsim** | 基于 ns-3 的 NDN 仿真，用于大规模 LEO 星座。 | [GitHub](https://github.com/ICARUS-ICN/icarus-ndnsim) |
| **LSNS** | 支持拓扑、路由、缓存与轨道计算的大规模卫星网络仿真。 | [GitHub](https://github.com/infonetlijian/Large-Scale-Satellite-Network-Simulator-LSNS) |
| **SatSIM** | 面向编队飞行测试与验证的实时多卫星仿真。 | [GitHub](https://github.com/ssc-ai/satsim) |
| **SNK** | 用于星座路由与网络性能评估的空间网络仿真。 | [GitHub](https://github.com/xdr940/snk) |
| **SNS-3（SNS3）** | 面向 ns-3 的卫星网络扩展模块。 | [GitHub](https://github.com/sns3/sns3-satellite) |
| **gr-opssat** | ESA OPS-SAT UHF 信号接收、解调与解码工具，不是仿真器。 | [GitHub](https://github.com/esa/gr-opssat) |
| **Leandvb** | 轻量级 DVB-S/DVB-S2 实现。 | [项目页](http://www.pabr.org/radio/leandvb/leandvb.en.html) |
| **gr-dvbs2rx** | 面向 SDR 工作流的 GNU Radio DVB-S2 接收机实现。 | [GitHub](https://github.com/igorauad/gr-dvbs2rx) |
| **OpenLTE** | LTE FDD SDR 实现与测试工具，属于通用 3GPP LTE 工具，而非卫星专用仿真器。 | [SourceForge](https://sourceforge.net/projects/openlte/) · [GitHub 源码](https://github.com/osh/openlte) |
| **OAI-RAN / OAI-CN** | 对齐 3GPP 的无线接入网与核心网实现、仿真环境。 | [OpenAirInterface](https://openairinterface.org/) |
| **free5GC** | 来源列为用于仿真工作的 3GPP 核心网实现。 | [GitHub](https://github.com/free5gc/free5gc) |
| **FLoRaSat** | 基于 OMNeT++ 的端到端卫星物联网离散事件仿真，采用 LoRa/LoRaWAN 空天适配。 | [GitHub](https://github.com/viveris/FLoRaSat) |
| **ChirpStack** | 卫星物联网仿真支撑。 | [官网](https://www.chirpstack.io/) |
| **GPS-SDR-SIM** | GPS 信号仿真。 | [GitHub](https://github.com/osqzss/gps-sdr-sim) |

### OpenSAND

来源将 OpenSAND 描述为端到端卫星通信模拟器，支持网状与星型拓扑、多点和多网关，并可接入透明或再生卫星。选型前应以项目一手文档核验当前版本的协议支持范围。

### CosmicBeats-Simulator

来源将 CosmicBeats-Simulator 描述为服务于网络、人工智能和计算等多类研究的空间模拟平台，列举了直连卫星物联网、分布式地面站和成像卫星运行等场景。

### icarus-ndnsim

来源指出 icarus-ndnsim 基于 ns-3，面向使用 NDN 作为通信后端的大规模 LEO 星座，可使用点到点、CSMA 和无线等链路层模型。

### LSNS

来源指出 LSNS 支持卫星网络拓扑、路由、协同缓存和实时轨道计算，并采用双体卫星轨道计算模型。

### SatSIM

来源将 SatSIM 描述为基于 TensorFlow 与 CUDA 的高保真多卫星模拟器，可覆盖传感器、执行器、航天器动力学、星间通信协议和环境干扰，用于编队飞行测试与验证。

### SNK

来源将 SNK 描述为面向互联网服务星座网络性能评估的空间网络仿真框架，涉及路由以及时延、拉伸、容量和吞吐量等指标。

### SNS-3

SNS-3 在来源列表中写作 `SNS3`，是面向 ns-3 的卫星网络扩展模块。一手 README 指出其由 `satellite`、`traffic` 与 `magister-stats` 三个模块构成，并建议按支持的 ns-3 版本匹配同一发布标签。

### FLoRaSat

FLoRaSat 是面向 LoRa/LoRaWAN 卫星物联网的 OMNeT++ 离散事件仿真框架。一手文档描述了空天地物联网模型，包括卫星网关、轨道传播、星间链路、路由和地面段。

## 轨道分析与任务动力学

| 项目 | 来源中的分类或用途 | 一手项目链接 |
| --- | --- | --- |
| **Celestia** | 卫星与天体三维显示、互动与模拟。 | [发布页](https://github.com/CelestiaProject/Celestia/releases) |
| **Skyfield** | 高精度天文与地球卫星位置计算。 | [GitHub](https://github.com/skyfielders/python-skyfield) · [官网](https://rhodesmill.org/skyfield/) |
| **GMAT** | 任务分析软件。 | [GitHub](https://github.com/nasa/GMAT) |
| **CelestLab** | 空间动力学计算。 | [Scilab 工具箱](https://atoms.scilab.org/toolboxes/celestlab) |
| **Orekit** | 空间动力学计算。 | [GitHub](https://github.com/Orekit/orekit) |
| **poliastro** | 空间动力学计算。 | [GitHub](https://github.com/poliastro/poliastro) |

### Celestia

来源将 Celestia 描述为可探索行星、卫星、恒星和星系的免费三维空间模拟软件，并可计算太阳系天体的位置和运动。

### Skyfield

来源将 Skyfield 描述为纯 Python 天文计算库，可产生行星与地球卫星的高精度位置数据。

### GMAT

来源列出 GMAT 用于任务分析。具体的动力学模型、摄动配置和接口能力应以 NASA GMAT 文档为准。

### Orekit

来源列出 Orekit 用于空间动力学计算。工程实现应以其一手文档确定数值模型与版本。

## 射频、SDR 与电磁仿真

来源将 4 个面向 SDR 的项目放在卫星通信网络与协议仿真类别中。鉴于这些项目也服务于射频与 SDR 工作流，本目录在此交叉收录；它们不会在仓库总数中重复计数。

| 项目 | 来源中的分类或用途 | 一手项目链接 |
| --- | --- | --- |
| **GNU Radio** | SDR 仿真与开发。 | [GitHub](https://github.com/gnuradio/gnuradio) |
| **gr-opssat** | OPS-SAT UHF 信号接收、解调与解码工具，不是仿真器。 | [GitHub](https://github.com/esa/gr-opssat) |
| **Leandvb** | DVB-S/DVB-S2 实现。 | [项目页](http://www.pabr.org/radio/leandvb/leandvb.en.html) |
| **gr-dvbs2rx** | 面向 SDR 的 DVB-S2 接收机实现。 | [GitHub](https://github.com/igorauad/gr-dvbs2rx) |
| **GPS-SDR-SIM** | GPS 信号仿真。 | [GitHub](https://github.com/osqzss/gps-sdr-sim) |
| **MEEP** | 电磁传播仿真。 | [GitHub](https://github.com/NanoComp/meep) |
| **openEMS** | 电磁与天线仿真。 | [GitHub](https://github.com/thliebig/openEMS) |
| **xnec2c** | 电磁与天线仿真。 | [项目页](https://www.xnec2c.org/) |

### GNU Radio

来源将 GNU Radio 列为 SDR 仿真工具。它是通用信号处理框架，因此任何卫星实验都应同时记录波形、信道、模型和测试场景。

### gr-dvbs2rx

来源将 gr-dvbs2rx 描述为面向 SDR 的 DVB-S2 发射与接收实现，包含物理层同步、前向纠错和 BBFRAME 处理相关模块。

### gr-opssat 与 OpenLTE

来源将两个项目列在仿真工具附近；一手文档则分别将 `gr-opssat` 定义为 ESA OPS-SAT UHF 信号的接收、解调与解码工具，将 OpenLTE 定义为带测试工具的 LTE FDD SDR 实现。二者都可作为通信工作流的支撑工具，但本目录按维护文档而非原始列表中的简写重新标注。

### MEEP、openEMS 与 xnec2c

来源将这三个项目归为电磁传播或天线仿真工具。它们采用的数值方法与工作流不同；共享结果时应记录求解器配置、几何、材料、边界和网格设置。

---

## 🤔 如何选择

- 做**卫星通信网络与星座协议**：OpenSAND、icarus-ndnsim、LSNS、SNK、SNS-3
- 做**卫星物联网与 LoRa/LoRaWAN 仿真**：FLoRaSat、ChirpStack
- 做**轨道分析、任务设计与空间飞行动力学**：GMAT、Orekit、Skyfield、CelestLab、poliastro
- 做**射频、SDR、信号生成与电磁建模**：GNU Radio、GPS-SDR-SIM、MEEP、openEMS、xnec2c

---

## 范围与来源

本仓库是发现与选型索引，并不分发所列项目。项目链接优先采用文章可见的一手链接，或为同名项目补充的项目维护页面；使用具体版本前请自行核验链接。

## 🤝 参与贡献

研究人员、开发者、学生和卫星爱好者都欢迎加入。如果你知道有项目应该出现在这份清单里，欢迎提交 pull request，或在 Discussions 里发起讨论。
👉 **[Join the Discussions](https://github.com/orgs/Satellite-OSS-BUPT/discussions)**

---

## 📄 许可

本文档是一份导航式的资源汇总。各项目的许可证与版权仍归其原始仓库所有。
