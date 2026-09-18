---
title: "Damping"
description: "Damping: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_Damping).*
## Purpose and responsibility
Software area `Damping` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_Damping.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_Damping.arxml` |
| Generation templates | `Ap_Damping_Cfg.arxml.tt`, `Ap_Damping_Cfg.h.tt`, `Ap_Damping_Generate.bat`, `Ap_Damping_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (13 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_Damping_Per1_AssistCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_Damping_Per1_AssistMechTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IRead_Damping_Per1_CustomDamp_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_Damping_Per1_DampingDDFactor_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_Damping_Per1_DefeatDampingSvc_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_Damping_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_Damping_Per1_MotorVelCRF_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_Damping_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_Damping_Per1_DampingCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_Damping_Per1_DampingCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_FltInjection_SCom_FltInjection` | RTE-generated symbol |
| `Rte_Call_Damping_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_Damping_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_Damping_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_Damping.h` `filters.h` `fixmath.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_Damping` `Ap_Damping_Cfg.h` `Rte.h` `Rte_Ap_Damping.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [Damping — Damping_Integration_Manual](./Damping-Damping_Integration_Manual/) | `Damping/doc/Damping_Integration_Manual.docx` |
| [Damping — Damping_MDD](./Damping-Damping_MDD/) | `Damping/doc/Damping_MDD.docx` |

*Repository path: `Damping/`* 
