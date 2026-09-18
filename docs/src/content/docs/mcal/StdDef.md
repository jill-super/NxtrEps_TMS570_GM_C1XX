---
title: "StdDef"
description: "StdDef: purpose, files, API and documents (MCAL & MCU Drivers)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer platform-type headers plus TMS570 register-definition includes.*
## Purpose and responsibility
Software area `StdDef` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `include/` | `Compiler.h`, `Platform_Types.h`, `Std_Types.h` |
| AUTOSAR model | 3 `.arxml` file(s), e.g. `Constants.arxml` |
## Public API
No C sources in this area (configuration, generated data or tooling only).
## Usage and dependencies
Selected project headers included by this module:
`Compiler_Cfg.h`
## Documents
No `doc/` documents for this module.

*Repository path: `StdDef/`* 
