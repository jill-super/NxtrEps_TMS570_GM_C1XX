---
title: "DiagMgr"
description: "DiagMgr: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house diagnostics manager (Ap_DiagMgr).*
## Purpose and responsibility
Software area `DiagMgr` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_DiagMgr_Core.c`, `Ap_DiagMgr_DemIf.c`, `Ap_DiagMgr_FailAction.c` |
| `include/` | `Ap_DiagMgr.h`, `Ap_DiagMgr_Types.h` |
| Generation templates | `DiagMgr_Cfg.c.tt`, `DiagMgr_Cfg.h.tt`, `DiagMgr_Generate.bat`, `DiagMgr_Proxy.c.tt`, `DiagMgr_bswmd.arxml`, `DiagMgr_swc.arxml.tt` |
## Public API
Top RTE/component symbols referenced in the sources (26 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Read_MEC_Cnt_enum` | RTE-generated symbol |
| `Rte_Read_MfgDiagInhibit_Cnt_lgc` | RTE-generated symbol |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_Call_DemIf_RestartDem` | RTE-generated symbol |
| `Rte_Call_DemIf_SetOperationCycleState` | RTE-generated symbol |
| `Rte_Call_DemIf_DemShutdown` | RTE-generated symbol |
| `Rte_Call_DiagMgr_Per2_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_DemIf_SetEventStatus` | RTE-generated symbol |
| `Rte_Call_DiagMgr_Per2_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_Read_IgnCnt_Cnt_u16` | RTE-generated symbol |
| `Rte_Read_MtrTrq_MtrNm_f32` | RTE-generated symbol |
| `Rte_Read_VehSpd_Kph_f32` | RTE-generated symbol |
| `Rte_Read_HwTrq_HwNm_f32` | RTE-generated symbol |
| `Rte_Write_DiagStsNonRecRmpToZeroFltPres_Cnt_lgc` | RTE-generated symbol |
| `Rte_Write_DiagStsCtrldDisRmpPres_Cnt_lgc` | RTE-generated symbol |
| `Rte_Write_DiagStsRecRmpToZeroFltPres_Cnt_lgc` | RTE-generated symbol |
| `Rte_Write_DiagStsHWASbSystmFltPres_Cnt_lgc` | RTE-generated symbol |
| `Rte_Write_DiagStsDefVehSpd_Cnt_lgc` | RTE-generated symbol |
| `Rte_Write_DiagStsDefTemp_Cnt_lgc` | RTE-generated symbol |
| `Rte_Write_DiagStsScomHWANotValid_Cnt_lgc` | RTE-generated symbol |
| `Rte_Write_DiagStsWIRDisable_Cnt_lgc` | RTE-generated symbol |
| `Rte_Write_DiagRampRate_XpmS_f32` | RTE-generated symbol |
| `Rte_Write_DiagRampValue_Uls_f32` | RTE-generated symbol |
| `Rte_Write_DiagRmpToZeroActive_Cnt_lgc` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_DiagMgr.h` `Ap_DiagMgr_Types.h` `CalConstants.h` `Det.h` `DiagMgr_Cfg.h` `GlobalMacro.h` `MemMap.h` `NvM.h` `Os.h` `Rte_Type.h` `Std_Types.h` `fixmath.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`CalConstants.h` `Compiler_Cfg.h` `Det.h` `DiagMgr_Cfg.h` `MemMap.h` `NvM.h` `Os.h` `Rte.h` `Rte_Ap_DiagMgr.h` `Rte_Compiler_Cfg.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [DiagMgr — Diagnostics_Manager_MDD](./DiagMgr-Diagnostics_Manager_MDD/) | `DiagMgr/doc/Diagnostics_Manager_MDD.docx` |

*Repository path: `DiagMgr/`* 
