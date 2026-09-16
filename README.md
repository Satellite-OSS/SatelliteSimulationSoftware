<h1 align="center">Open Satellite Simulation Software</h1>

<p align="center">
A curated and continuously maintained collection of open-source software for satellite communication, orbital analysis, RF, and simulation workflows.
</p>

<p align="center">
  <a href="https://github.com/Satellite-OSS/.github/blob/main/traffic/SatelliteSimulationSoftware.csv" title="Cumulative recorded repository views; updated hourly"><img src="https://raw.githubusercontent.com/Satellite-OSS/.github/main/traffic/SatelliteSimulationSoftware.svg" alt="Total views"></a>
  <a href="https://github.com/orgs/Satellite-OSS-BUPT/discussions"><img src="https://img.shields.io/badge/Discussions-Join%20the%20Community-2ea44f?style=flat-square&logo=github" alt="Join the community discussion"></a>
  <a href="./README_CN.md"><img src="https://img.shields.io/badge/README-简体中文-0969da?style=flat-square&labelColor=555555" alt="Read in Simplified Chinese"></a>
</p>

<p align="center"><strong>English</strong> | <a href="./README_CN.md">中文</a></p>

<p align="center"><strong>30 source-listed tools</strong> &nbsp;·&nbsp; <strong>3 simulation domains</strong></p>

<details>
<summary><strong>Contents</strong></summary>

- [Quick index](#quick-index)
- [Satellite communication networks and protocols](#satellite-communication-networks-and-protocols) · 16
- [Orbital analysis and mission dynamics](#orbital-analysis-and-mission-dynamics) · 6
- [RF, SDR, and electromagnetic simulation](#rf-sdr-and-electromagnetic-simulation) · 8
- [Scope and provenance](#scope-and-provenance)
- [Contributing](#contributing)

</details>

## Quick index

#### [Satellite communication networks and protocols](#satellite-communication-networks-and-protocols) <sup>16 tools</sup>

- [**OpenSAND**](#opensand) — End-to-end satellite communication simulation
- [**CosmicBeats-Simulator**](#cosmicbeats-simulator) — Multi-domain space-system simulation
- [**icarus-ndnsim**](#icarus-ndnsim) — LEO constellation NDN simulation on ns-3
- [**LSNS**](#lsns) — Large-scale satellite network simulation
- [**SatSIM**](#satsim) — Multi-satellite simulation and visualisation
- [**SNK**](#snk) — Satellite constellation network-performance simulation

#### [Orbital analysis and mission dynamics](#orbital-analysis-and-mission-dynamics) <sup>6 tools</sup>

- [**Celestia**](#celestia) — Interactive 3D celestial visualisation
- [**Skyfield**](#skyfield) — Precision astronomical and satellite-position computation
- [**GMAT**](#gmat) — Mission analysis
- [**Orekit**](#orekit) — Space-flight dynamics library

#### [RF, SDR, and electromagnetic simulation](#rf-sdr-and-electromagnetic-simulation) <sup>8 tools</sup>

- [**GNU Radio**](#gnu-radio) — SDR development and simulation
- [**gr-dvbs2rx**](#gr-dvbs2rx) — SDR DVB-S2 receiver implementation
- [**MEEP**](#meep) — Electromagnetic propagation simulation
- [**openEMS**](#openems) — Electromagnetic and antenna simulation

## Satellite communication networks and protocols

| Project | Source classification | Primary project link |
| --- | --- | --- |
| **OpenSAND** | End-to-end satellite communication simulation; the source highlights DVB-RCS2 and DVB-S2 use cases. | [GitHub](https://github.com/CNES/opensand) · [Website](https://www.opensand.org/) |
| **CosmicBeats-Simulator** | Space-system simulation spanning orbital dynamics, wireless communications, IoT, computing, and imaging scenarios. | [GitHub](https://github.com/vismay2303/CosmicBeats-Simulator) |
| **icarus-ndnsim** | ns-3-based NDN simulation for large LEO constellations. | [GitHub](https://github.com/ICARUS-ICN/icarus-ndnsim) |
| **LSNS** | Large-scale satellite-network simulation with topology, routing, caching, and orbit-calculation support. | [GitHub](https://github.com/infonetlijian/Large-Scale-Satellite-Network-Simulator-LSNS) |
| **SatSIM** | Real-time multi-satellite simulation for formation-flight testing and validation. | [GitHub](https://github.com/ssc-ai/satsim) |
| **SNK** | Space-network simulation for evaluating constellation routing and performance indicators. | [GitHub](https://github.com/xdr940/snk) |
| **SNS3** | Satellite communication network simulator based on ns-3. | Source link pending verification |
| **gr-opssat** | Small-satellite modem simulation. | Source link pending verification |
| **Leandvb** | Lightweight DVB-S/DVB-S2 implementation. | [Project page](http://www.pabr.org/radio/leandvb/leandvb.en.html) |
| **gr-dvbs2rx** | GNU Radio-based DVB-S2 receiver implementation for SDR workflows. | [GitHub](https://github.com/igorauad/gr-dvbs2rx) |
| **OpenLTE** | 3GPP simulation. | Source link pending verification |
| **OAI-RAN / OAI-CN** | 3GPP-aligned radio access and core-network implementation and simulation environment. | [OpenAirInterface](https://openairinterface.org/) |
| **free5GC** | 3GPP core-network implementation referenced for simulation work. | [GitHub](https://github.com/free5gc/free5gc) |
| **FLoRaSat** | Satellite IoT simulation. | Source link pending verification |
| **ChirpStack** | Satellite IoT simulation support. | [Website](https://www.chirpstack.io/) |
| **GPS-SDR-SIM** | GPS signal simulation. | [GitHub](https://github.com/osqzss/gps-sdr-sim) |

### OpenSAND

The source describes OpenSAND as an end-to-end satellite communication simulator with mesh and star topologies, multiple gateways, and transparent or regenerative satellite access. Use its primary documentation to validate current protocol support before selecting a release.

### CosmicBeats-Simulator

The source presents CosmicBeats-Simulator as a platform for cross-domain space-system research. Its listed scenarios include direct-to-satellite IoT, distributed ground stations, and imaging-satellite operation.

### icarus-ndnsim

The source identifies icarus-ndnsim as an ns-3-based simulator for deploying NDN as the communication backend of large LEO constellations. It can work with point-to-point, CSMA, and wireless link-layer models.

### LSNS

The source identifies LSNS as a large-scale satellite-network simulator for network topology, routing, collaborative caching, and a real-time orbit-calculation module based on a two-body orbit model.

### SatSIM

The source describes SatSIM as a TensorFlow and CUDA-based high-fidelity multi-satellite simulator for sensors, actuators, spacecraft dynamics, inter-satellite communication protocols, and environmental effects.

### SNK

The source describes SNK as a constellation-network framework for routing and network-performance studies, including latency, stretch, capacity, and throughput.

## Orbital analysis and mission dynamics

| Project | Source classification | Primary project link |
| --- | --- | --- |
| **Celestia** | Interactive 3D display and exploration of satellites and celestial bodies. | [Releases](https://github.com/CelestiaProject/Celestia/releases) |
| **Skyfield** | Precision astronomical computation, including Earth-satellite positions. | [GitHub](https://github.com/skyfielders/python-skyfield) · [Website](https://rhodesmill.org/skyfield/) |
| **GMAT** | Mission analysis software. | [GitHub](https://github.com/nasa/GMAT) |
| **CelestLab** | Space-dynamics computation. | [Scilab toolbox](https://atoms.scilab.org/toolboxes/celestlab) |
| **Orekit** | Space-dynamics computation. | [GitHub](https://github.com/Orekit/orekit) |
| **poliastro** | Space-dynamics computation. | [GitHub](https://github.com/poliastro/poliastro) |

### Celestia

The source characterises Celestia as a free 3D space simulator for exploring celestial objects and their positions and motion.

### Skyfield

The source characterises Skyfield as a pure-Python astronomy library that produces high-precision positions for planets and Earth satellites.

### GMAT

The source lists GMAT as mission-analysis software. Consult the project documentation for current models, force configurations, and supported interfaces.

### Orekit

The source lists Orekit as a space-dynamics computation library. Its primary documentation should be the basis for implementation decisions and numerical-model selection.

## RF, SDR, and electromagnetic simulation

| Project | Source classification | Primary project link |
| --- | --- | --- |
| **GNU Radio** | SDR simulation and development. | [GitHub](https://github.com/gnuradio/gnuradio) |
| **gr-opssat** | Small-satellite modem simulation. | Source link pending verification |
| **Leandvb** | DVB-S/DVB-S2 implementation. | [Project page](http://www.pabr.org/radio/leandvb/leandvb.en.html) |
| **gr-dvbs2rx** | SDR-oriented DVB-S2 receiver implementation. | [GitHub](https://github.com/igorauad/gr-dvbs2rx) |
| **GPS-SDR-SIM** | GPS signal simulation. | [GitHub](https://github.com/osqzss/gps-sdr-sim) |
| **MEEP** | Electromagnetic propagation simulation. | [GitHub](https://github.com/NanoComp/meep) |
| **openEMS** | Electromagnetic and antenna simulation. | [GitHub](https://github.com/thliebig/openEMS) |
| **xnec2c** | Electromagnetic and antenna simulation. | [Project page](https://www.xnec2c.org/) |

### GNU Radio

The source lists GNU Radio under SDR simulation. It is a general-purpose signal-processing framework, so a satellite-specific model, waveform, and test scenario should be documented alongside every experiment.

### gr-dvbs2rx

The source describes gr-dvbs2rx as an SDR-oriented DVB-S2 transmitter and receiver implementation with processing blocks for physical-layer synchronisation, forward error correction, and BBFRAME handling.

### MEEP, openEMS, and xnec2c

The source groups these projects as electromagnetic-propagation or antenna-simulation tools. They support different numerical methods and workflows; record solver configuration, geometry, materials, boundaries, and mesh settings with any result shared in this repository.

## Scope and provenance

This directory is a discovery index, not a distribution of the listed projects. Project names and the source classifications above are extracted and condensed from the publicly visible part of the referenced Zhihu article. Project links point to primary project pages where they were visible in the article or where a project-maintained page was identified from the named project; contributors should check the link before relying on a release.

The article exposes only part of its detailed list without a paid subscription. This repository deliberately excludes the locked portion. See the [source note](./docs/sources/zhihu-1948060672953917707.md) for the extraction boundary, citation, and maintenance rules.

## Contributing

Researchers, developers, students, and satellite enthusiasts are welcome. Please read [the contribution guide](./CONTRIBUTING.md) before opening a pull request, and use [OPENSAT Discussions](https://github.com/orgs/Satellite-OSS-BUPT/discussions) for discovery or categorisation questions.
