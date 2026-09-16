<h1 align="center">开源卫星仿真软件</h1>

<p align="center">
持续整理卫星通信、轨道分析、射频与仿真工作流相关的开源软件，并保留条目的来源与一手项目链接。
</p>

<p align="center">
  <a href="https://github.com/Satellite-OSS/.github/blob/main/traffic/SatelliteSimulationSoftware.csv" title="累计仓库访问量，每小时更新"><img src="https://raw.githubusercontent.com/Satellite-OSS/.github/main/traffic/SatelliteSimulationSoftware.svg" alt="总访问量"></a>
  <a href="https://github.com/orgs/Satellite-OSS-BUPT/discussions"><img src="https://img.shields.io/badge/Discussions-Join%20the%20Community-2ea44f?style=flat-square&logo=github" alt="加入社区讨论"></a>
  <a href="./README.md"><img src="https://img.shields.io/badge/README-English-0969da?style=flat-square&labelColor=555555" alt="Read in English"></a>
</p>

<p align="center"><a href="./README.md">English</a> | <strong>中文</strong></p>

<p align="center"><strong>26 个软件项目</strong> &nbsp;·&nbsp; <strong>3 个仿真方向</strong></p>

<details>
<summary><strong>目录</strong></summary>

- [快速索引](#快速索引)
- [卫星通信网络与协议仿真](#卫星通信网络与协议仿真) · 16
- [轨道分析与任务动力学](#轨道分析与任务动力学) · 6
- [射频、SDR 与电磁仿真](#射频sdr-与电磁仿真) · 8 个分类位置，其中 4 个交叉收录
- [范围与来源](#范围与来源)
- [参与贡献](#参与贡献)

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
| **SNS3** | 基于 ns-3 的卫星通信网络模拟器。 | 待核验来源链接 |
| **gr-opssat** | 小卫星调制解调器仿真。 | 待核验来源链接 |
| **Leandvb** | 轻量级 DVB-S/DVB-S2 实现。 | [项目页](http://www.pabr.org/radio/leandvb/leandvb.en.html) |
| **gr-dvbs2rx** | 面向 SDR 工作流的 GNU Radio DVB-S2 接收机实现。 | [GitHub](https://github.com/igorauad/gr-dvbs2rx) |
| **OpenLTE** | 3GPP 仿真。 | 待核验来源链接 |
| **OAI-RAN / OAI-CN** | 对齐 3GPP 的无线接入网与核心网实现、仿真环境。 | [OpenAirInterface](https://openairinterface.org/) |
| **free5GC** | 来源列为用于仿真工作的 3GPP 核心网实现。 | [GitHub](https://github.com/free5gc/free5gc) |
| **FLoRaSat** | 卫星物联网仿真。 | 待核验来源链接 |
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
| **gr-opssat** | 小卫星调制解调器仿真。 | 待核验来源链接 |
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

### MEEP、openEMS 与 xnec2c

来源将这三个项目归为电磁传播或天线仿真工具。它们采用的数值方法与工作流不同；共享结果时应记录求解器配置、几何、材料、边界和网格设置。

## 范围与来源

本仓库是发现与选型索引，并不分发所列项目。上表项目名及来源分类，来自所给知乎文章的公开可见部分；条目说明均为压缩转述。项目链接优先采用文章可见的一手链接，或为同名项目补充的项目维护页面；使用具体版本前请自行核验链接。

原文详情列表的其余部分受付费订阅限制。本仓库不会尝试解锁、抓取或收录该受限内容。可见范围、引用方式及维护规则见[来源注记](./docs/sources/zhihu-1948060672953917707.md)。

## 参与贡献

欢迎研究人员、开发者、学生和卫星爱好者参与。提交前请阅读[贡献指南](./CONTRIBUTING.md)；发现新条目或分类问题，可在 [OPENSAT Discussions](https://github.com/orgs/Satellite-OSS-BUPT/discussions) 中讨论。
