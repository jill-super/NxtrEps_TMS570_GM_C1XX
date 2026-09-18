---
title: "FrqDepDmpnInrtCmp"
description: "FrqDepDmpnInrtCmp: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_FrqDepDmpnInrtCmp).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> title: "FrqDepDmpnInrtCmp — Frequency_Dependant_Damping_And_Inertia_Compenstation_MDD"

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_FrqDepDmpnInrtCmp.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_FrqDepDmpnInrtCmp.arxml` |
| Generation templates | `Ap_FrqDepDmpnInrtCmp_Cfg.arxml.tt`, `Ap_FrqDepDmpnInrtCmp_Cfg.h.tt`, `Ap_FrqDepDmpnInrtCmp_Generate.bat`, `Ap_FrqDepDmpnInrtCmp_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (13 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_IRead_FrqDepDmpnInrtCmp_Per1_BaseAssistCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_FrqDepDmpnInrtCmp_Per1_CRFMotorVel_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_FrqDepDmpnInrtCmp_Per1_FreqDepDmpSrlComSvcDft_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_FrqDepDmpnInrtCmp_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_FrqDepDmpnInrtCmp_Per1_VehicleLonAccel_KphpS_f32` | RTE-generated symbol |
| `Rte_IRead_FrqDepDmpnInrtCmp_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IRead_FrqDepDmpnInrtCmp_Per1_WIRCmdAmpBlnd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_FrqDepDmpnInrtCmp_Per1_FrqDepDmpnInrtCmp_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_FrqDepDmpnInrtCmp_Per1_FrqDepDmpnInrtCmp_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_FltInjection_SCom_FltInjection` | RTE-generated symbol |
| `Rte_Call_FrqDepDmpnInrtCmp_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_FrqDepDmpnInrtCmp_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_FrqDepDmpnInrtCmp_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_FrqDepDmpnInrtCmp.h` `filters.h` `fixmath.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_FrqDepDmpnInrtCmp` `Ap_FrqDepDmpnInrtCmp_Cfg.h` `Rte.h` `Rte_Ap_FrqDepDmpnInrtCmp.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [FrqDepDmpnInrtCmp — Frequency_Dependant_Damping_And_Inertia_Compenstation_MDD](./FrqDepDmpnInrtCmp-Frequency_Dependant_Damping_And_Inertia_Compenstation_MDD/) | `FrqDepDmpnInrtCmp/doc/Frequency_Dependant_Damping_And_Inertia_Compenstation_MDD.docx` |
| [FrqDepDmpnInrtCmp — FrqDepDmpnInrtCmp Integration Manual](./FrqDepDmpnInrtCmp-FrqDepDmpnInrtCmp-Integration-Manual/) | `FrqDepDmpnInrtCmp/doc/FrqDepDmpnInrtCmp Integration Manual.doc` |

*Repository path: `FrqDepDmpnInrtCmp/`* 
