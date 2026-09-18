---
title: "DigColPs"
description: "DigColPs: purpose, files, API and documents (Sensor / Actuator Abstraction)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-Cs (Sa_DigColPs/Int).*
## Purpose and responsibility
Software area `DigColPs` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Sa_DigColPs.c`, `Sa_DigColPsInt.c` |
| `include/` | `Sa_DigColPsInt.h` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Sa_DigColPs.arxml` |
| Generation templates | `Sa_DigColPs_Cfg.arxml.tt`, `Sa_DigColPs_Cfg.h.tt`, `Sa_DigColPs_Generate.bat`, `Sa_DigColPs_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (13 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Pim_DigColPsEOL` | RTE-generated symbol |
| `Rte_Call_EOLDigColPosCals_WriteBlock` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_SystemTime_GetSystemTime_mS_u32` | RTE-generated symbol |
| `Rte_Call_SystemTime_DtrmnElapsedTime_mS_u16` | RTE-generated symbol |
| `Rte_IRead_DigColPs_Per2_MecState_Cnt_enum` | RTE-generated symbol |
| `Rte_IWrite_DigColPs_Per2_I2CHwAbsPosValid_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_DigColPs_Per2_I2CHwAbsPosValid_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_DigColPs_Per2_I2CHwAbsPos_HwDeg_f32` | RTE-generated symbol |
| `Rte_IWriteRef_DigColPs_Per2_I2CHwAbsPos_HwDeg_f32` | RTE-generated symbol |
| `Rte_IWrite_DigColPs_Per2_TrimComp_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_DigColPs_Per2_TrimComp_Cnt_lgc` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_GetNTCActive` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`CalConstants.h` `GlobalMacro.h` `I2cNxtr.h` `I2cNxtr_Cfg.h` `MemMap.h` `Os.h` `Rte_Sa_DigColPs.h` `Sa_DigColPsInt.h` `SystemTime.h` `filters.h` `fixmath.h` `interrupts.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [DigColPs — DigColPsInt_MDD](./DigColPs-DigColPsInt_MDD/) | `DigColPs/doc/DigColPsInt_MDD.docx` |
| [DigColPs — DigColPs_Integration_Manual](./DigColPs-DigColPs_Integration_Manual/) | `DigColPs/doc/DigColPs_Integration_Manual.docx` |
| [DigColPs — DigColPs_MDD](./DigColPs-DigColPs_MDD/) | `DigColPs/doc/DigColPs_MDD.docx` |

*Repository path: `DigColPs/`* 
