---
title: "GM C1XX EPS — TMS570 AUTOSAR documentation"
description: "AUTOSAR-based Electric Power Steering firmware for GM C1XX (TI TMS570): layers, modules, APIs and converted design documents."
template: splash
hero:
  tagline: AUTOSAR-based Electric Power Steering firmware for GM C1XX (TI TMS570) — layers, modules, APIs and design documents.
  actions:
    - text: Browse the layers
      link: ./asw/
      icon: right-arrow
    - text: Vector vs. custom
      link: ./general/vector-vs-custom/
      icon: open-book
      variant: secondary
---

## Project overview

Complete Electric Power Steering (EPS) firmware for the **GM C1XX** platform on the
**Texas Instruments TMS570** (ARM Cortex-R4), developed to **AUTOSAR** and **ISO 26262 ASIL D**.
It implements torque sensing, power-assisted steering control, motor control, diagnostics
(UDS/CAN) and manufacturing services.

## AUTOSAR layers

- [Application Software (ASW)](./asw/) — AUTOSAR application software components (Ap_*), diagnostics and state management. (49 areas)
- [Sensor / Actuator Abstraction](./sa/) — Sensor/actuator abstraction software components (Sa_*) and associated diagnostics. (11 areas)
- [Complex Device Drivers (CDD)](./cdd/) — Complex device drivers (Cd_*) and motor-control / power-stage drivers. (4 areas)
- [Basic Software (BSW)](./bsw/) — Vector MICROSAR basic software, memory stack (Fee/NvM), XCP and ECU services. (3 areas)
- [MCAL & MCU Drivers](./mcal/) — Microcontroller abstraction: on-chip peripheral drivers, startup code and platform types. (8 areas)
- [RTE & System Integration](./rte/) — RTE, OS configuration, generated data, interface projects and build/tooling integration. (1 areas)
- [Libraries & Common](./libs/) — Shared libraries, common diagnostics services, metrics and quality tooling. (5 areas)

- [General](./general/build-system/) — build system, safety, test reports, glossary.

## Vector vs. custom

- **Custom (Nexteer in-house):** all `Ap_*`/`Sa_*`/`Cd_*` application modules, drivers and libraries.
- **Vector-provided:** the MICROSAR BSW stack, generated RTE/OS data and DaVinci artefacts
  (see [BSW](./bsw/) and [RTE & System Integration](./rte/)).
- **Third-party:** TI Flash/FEE drivers (`Fee`, `Fls`), Gliwa T1 (`GliwaT1`), PRQA QAC config.

Full matrix: [Vector vs. custom code](./general/vector-vs-custom/).

## Repository structure

```text
<repo root>/            # ECU firmware (this snapshot) — untouched by the docs project
  <Module>/             # one folder per SW-C/driver: autosar/ generate/ src/ tools/ utp/ doc/
  GM_C1XX_EPS_TMS570/   # ECU integration: SwProject/ (BSW, RTE, SW-Cs) + Tools/ + HLDD/
  docs/                 # this documentation site (Astro 7 + Starlight project root)
  .github/workflows/    # Pages deploy + Dependabot auto-merge
```
