---
title: "GMStrtStop"
description: "GMStrtStop: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_GMStrtStop).*
## Purpose and responsibility
Software area `GMStrtStop` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_GMStrtStop.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_GMStrtStop.arxml` |
| Generation templates | `Ap_GMStrtStop_Cfg.arxml.tt`, `Ap_GMStrtStop_Cfg.h.tt`, `Ap_GMStrtStop_Generate.bat`, `Ap_GMStrtStop_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (13 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_IRead_StrtStop_Per1_APAState_State_enum` | RTE-generated symbol |
| `Rte_IRead_StrtStop_Per1_EngSpd_Rpm_f32` | RTE-generated symbol |
| `Rte_IRead_StrtStop_Per1_HandwheelVelocity_HwRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_StrtStop_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_StrtStop_Per1_SS12VFault_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_StrtStop_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_StrtStop_Per1_SSScale_Uls_f32` | RTE-generated symbol |
| `Rte_IWriteRef_StrtStop_Per1_SSScale_Uls_f32` | RTE-generated symbol |
| `Rte_IWrite_StrtStop_Per1_SSSlew_UlspS_f32` | RTE-generated symbol |
| `Rte_IWriteRef_StrtStop_Per1_SSSlew_UlspS_f32` | RTE-generated symbol |
| `Rte_IWrite_StrtStop_Per1_SSState_State_enum` | RTE-generated symbol |
| `Rte_IWriteRef_StrtStop_Per1_SSState_State_enum` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_GMStrtStop.h` `SystemTime.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [GMStrtStop — GMStrtStop_Integration_Manual](./GMStrtStop-GMStrtStop_Integration_Manual/) | `GMStrtStop/doc/GMStrtStop_Integration_Manual.doc` |
| [GMStrtStop — GMStrtStop_MDD](./GMStrtStop-GMStrtStop_MDD/) | `GMStrtStop/doc/GMStrtStop_MDD.docx` |

*Repository path: `GMStrtStop/`* 
