---
title: "CtrldDisShtdn"
description: "CtrldDisShtdn: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_CtrldDisShtdn).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> description: "Converted .docx document from CtrldDisShtdn/doc."

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_CtrldDisShtdn.c` |
| AUTOSAR model | 5 `.arxml` file(s), e.g. `Ap_CtrldDisShtdn.arxml` |
| Generation templates | `Ap_CtrldDisShtdn_Cfg.arxml.tt`, `Ap_CtrldDisShtdn_Cfg.h.tt`, `Ap_CtrldDisShtdn_Generate.bat`, `Ap_CtrldDisShtdn_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (19 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_CtrldDisShtdn_Per1_AssistAssyPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IRead_CtrldDisShtdn_Per1_CRFMtrVel_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_CtrldDisShtdn_Per1_DiagStsF2Active_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_CtrldDisShtdn_Per1_SumLimTrqCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_CtrldDisShtdn_Per1_CntDisMtrTrqCmdCRF_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_CtrldDisShtdn_Per1_CntDisMtrTrqCmdCRF_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_CtrldDisShtdn_Per1_CntDisMtrTrqCmdMRF_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_CtrldDisShtdn_Per1_CntDisMtrTrqCmdMRF_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_CtrldDisShtdn_Per1_CtrldDmpStsCmp_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_CtrldDisShtdn_Per1_CtrldDmpStsCmp_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_CtrldDisShtdn_Per1_SysC_CRFMtrTrqCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_CtrldDisShtdn_Per1_SysC_CRFMtrTrqCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_CtrldDisShtdn_Per1_SysC_MRFMtrTrqCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_CtrldDisShtdn_Per1_SysC_MRFMtrTrqCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_Call_SystemTime_DtrmnElapsedTime_mS_u16` | RTE-generated symbol |
| `Rte_Call_SystemTime_GetSystemTime_mS_u32` | RTE-generated symbol |
| `Rte_Call_CtrldDisShtdn_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_CtrldDisShtdn_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_CtrldDisShtdn_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_CtrldDisShtdn.h` `filters.h` `fixmath.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_CtrldDisShtdn` `Ap_CtrldDisShtdn_Cfg.h` `Rte.h` `Rte_Ap_CtrldDisShtdn.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [CtrldDisShtdn — Controller_Disable_MDD](./CtrldDisShtdn-Controller_Disable_MDD/) | `CtrldDisShtdn/doc/Controller_Disable_MDD.docx` |

*Repository path: `CtrldDisShtdn/`* 
