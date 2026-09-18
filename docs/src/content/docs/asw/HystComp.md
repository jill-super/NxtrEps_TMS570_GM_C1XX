---
title: "HystComp"
description: "HystComp: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_HystComp).*
## Purpose and responsibility
Software area `HystComp` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_HystComp.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_HystComp.arxml` |
| Generation templates | `Ap_HystComp_Cfg.arxml.tt`, `Ap_HystComp_Cfg.h.tt`, `Ap_HystComp_Generate.bat`, `Ap_HystComp_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (12 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_HystComp_Per1_AssistMechTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IRead_HystComp_Per1_BaseAssistCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_HystComp_Per1_DefeatHystService_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_HystComp_Per1_FricOffset_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_HystComp_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_HystComp_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IRead_HystComp_Per1_WIRCmdAmpBlnd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_HystComp_Per1_HysteresisComp_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_HystComp_Per1_HysteresisComp_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_FltInjection_SCom_FltInjection` | RTE-generated symbol |
| `Rte_Call_HystComp_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_HystComp_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_HystComp_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_HystComp.h` `filters.h` `fixmath.h` `float.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_HystComp` `Ap_HystComp_Cfg.h` `Rte.h` `Rte_Ap_HystComp.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [HystComp — HystComp_Integration_Manual](./HystComp-HystComp_Integration_Manual/) | `HystComp/doc/HystComp_Integration_Manual.docx` |
| [HystComp — Hysteresis_Compensation_MDD](./HystComp-Hysteresis_Compensation_MDD/) | `HystComp/doc/Hysteresis_Compensation_MDD.doc` |

*Repository path: `HystComp/`* 
