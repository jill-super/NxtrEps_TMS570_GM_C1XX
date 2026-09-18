---
title: "EtDmpFw"
description: "EtDmpFw: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_EtDmpFw).*
## Purpose and responsibility
Software area `EtDmpFw` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_EtDmpFw.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_EtDmpFw.arxml` |
| Generation templates | `Ap_EtDmpFw_Cfg.arxml.tt`, `Ap_EtDmpFw_Cfg.h.tt`, `Ap_EtDmpFw_Generate.bat`, `Ap_EtDmpFw_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (12 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_EtDmpFw_Per1_AssistEOTDamping_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_EtDmpFw_Per1_CRFMtrVel_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_EtDmpFw_Per1_EOTDisable_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_EtDmpFw_Per1_HandwheelAuthority_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_EtDmpFw_Per1_HandwheelPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_EtDmpFw_Per1_MEC_Counter_Cnt_enum` | RTE-generated symbol |
| `Rte_IRead_EtDmpFw_Per1_Vehicle_Speed_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_EtDmpFw_Per1_EOTDampingLtd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_EtDmpFw_Per1_EOTDampingLtd_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_FaultInjection_SCom_FltInjection` | RTE-generated symbol |
| `Rte_Call_EtDmpFw_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_EtDmpFw_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_EtDmpFw_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_EtDmpFw.h` `fixmath.h` `fpmtype.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_EtDmpFw` `Ap_EtDmpFw_Cfg.h` `Rte.h` `Rte_Ap_EtDmpFw.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [EtDmpFw — EOTDampingFirewall_MDD](./EtDmpFw-EOTDampingFirewall_MDD/) | `EtDmpFw/doc/EOTDampingFirewall_MDD.doc` |

*Repository path: `EtDmpFw/`* 
