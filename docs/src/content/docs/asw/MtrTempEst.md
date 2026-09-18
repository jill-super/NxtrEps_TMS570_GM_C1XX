---
title: "MtrTempEst"
description: "MtrTempEst: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_MtrTempEst).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> title: "MtrTempEst — Motor_Temperature_Estimation_Integration_Manual"

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_MtrTempEst.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_MtrTempEst.arxml` |
| Generation templates | `Ap_MtrTempEst_Cfg.arxml.tt`, `Ap_MtrTempEst_Cfg.h.tt`, `Ap_MtrTempEst_Generate.bat`, `Ap_MtrTempEst_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (28 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_MtrTempEst_Init1_AmbTemp_DegC_f32` | RTE-generated symbol |
| `Rte_IRead_MtrTempEst_Init1_CtrlTempFinal_DegC_f32` | RTE-generated symbol |
| `Rte_IRead_MtrTempEst_Init1_EngTemp_DegC_f32` | RTE-generated symbol |
| `Rte_IWrite_MtrTempEst_Init1_AssistMechTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IWriteRef_MtrTempEst_Init1_AssistMechTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IWrite_MtrTempEst_Init1_CuTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IWriteRef_MtrTempEst_Init1_CuTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IWrite_MtrTempEst_Init1_MagTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IWriteRef_MtrTempEst_Init1_MagTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IWrite_MtrTempEst_Init1_SiTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IWriteRef_MtrTempEst_Init1_SiTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IRead_MtrTempEst_Per1_AMTempEstDisable_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_MtrTempEst_Per1_AmbTemp_DegC_f32` | RTE-generated symbol |
| `Rte_IRead_MtrTempEst_Per1_CtrlTempFinal_DegC_f32` | RTE-generated symbol |
| `Rte_IRead_MtrTempEst_Per1_EngTemp_DegC_f32` | RTE-generated symbol |
| `Rte_IRead_MtrTempEst_Per1_EstPkCurr_AmpSq_f32` | RTE-generated symbol |
| `Rte_IRead_MtrTempEst_Per1_HwVel_HwRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_MtrTempEst_Per1_ScomTempDataRcvd_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_MtrTempEst_Per1_AssistMechTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IWriteRef_MtrTempEst_Per1_AssistMechTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IWrite_MtrTempEst_Per1_CuTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IWriteRef_MtrTempEst_Per1_CuTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IWrite_MtrTempEst_Per1_MagTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IWriteRef_MtrTempEst_Per1_MagTempEst_DegC_f32` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_MtrTempEst_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_MtrTempEst.h` `filters.h` `fixmath.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_MtrTempEst` `Ap_MtrTempEst_Cfg.h` `Rte.h` `Rte_Ap_MtrTempEst.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [MtrTempEst — Motor_Temperature_Estimation_Integration_Manual](./MtrTempEst-Motor_Temperature_Estimation_Integration_Manual/) | `MtrTempEst/doc/Motor_Temperature_Estimation_Integration_Manual.docx` |
| [MtrTempEst — Motor_Temperature_Estimation_MDD](./MtrTempEst-Motor_Temperature_Estimation_MDD/) | `MtrTempEst/doc/Motor_Temperature_Estimation_MDD.docx` |

*Repository path: `MtrTempEst/`* 
