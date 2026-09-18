---
title: "OvrVoltMon"
description: "OvrVoltMon: purpose, files, API and documents (Sensor / Actuator Abstraction)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Sa_OvrVoltMon).*
## Purpose and responsibility
Software area `OvrVoltMon` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Sa_OvrVoltMon.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Sa_OvrVoltMon.arxml` |
| Generation templates | `Sa_OvrVoltMon_Cfg.arxml.tt`, `Sa_OvrVoltMon_Cfg.h.tt`, `Sa_OvrVoltMon_Generate.bat`, `Sa_OvrVoltMon_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (6 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_OvrVoltMon_Per1_PwrDiscBTestStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_phyOvrVoltFdbk_OP_GET` | RTE-generated symbol |
| `Rte_Call_OvrVoltMon_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_OvrVoltMon_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Sa_OvrVoltMon.h` `Sa_OvrVoltMon_Cfg.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`CalConstants.h` `Compiler_Cfg.h` `MemMap.h` `Sa_OvrVoltMon` `Rte.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Sa_OvrVoltMon.h` `Rte_Type.h` `Sa_OvrVoltMon_Cfg.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [OvrVoltMon — OverVoltageMonitor_MDD](./OvrVoltMon-OverVoltageMonitor_MDD/) | `OvrVoltMon/doc/OverVoltageMonitor_MDD.docx` |
| [OvrVoltMon — OvrVoltMon_Integration_Manual](./OvrVoltMon-OvrVoltMon_Integration_Manual/) | `OvrVoltMon/doc/OvrVoltMon_Integration_Manual.docx` |

*Repository path: `OvrVoltMon/`* 
