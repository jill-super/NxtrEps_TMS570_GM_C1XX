---
title: "StaMd"
description: "StaMd: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house state machine (Ap_StaMd).*
## Purpose and responsibility
Software area `StaMd` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_StaMd.c` |
| Generation templates | `Ap_StaMd_Cfg.c.tt`, `Ap_StaMd_Cfg.h.tt`, `Ap_StaMd_Generate.bat`, `Ap_StaMd_Proxy.c.tt`, `Ap_StaMd_bswmd.arxml`, `Ap_StaMd_swc.arxml.tt` |
## Public API
Top RTE/component symbols referenced in the sources (18 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_CloseCheckData_WriteBlock` | RTE-generated symbol |
| `Rte_Call_StaMd_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_IRead_StaMd_Per1_FTerm_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_StaMd_Per1_CTerm_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_StaMd_Per1_ATerm_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_StaMd_Per1_RampStatusComplete_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_StaMd_Per1_ControlledDampStatusComplete_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_StaMd_Per1_TMFTestComplete_Cnt_lgc` | RTE-generated symbol |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_Call_TOD_OP_SET` | RTE-generated symbol |
| `Rte_Switch_SystemState_Mode` | RTE-generated symbol |
| `Rte_Call_StaMd_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_DiagMgr_StaCtrl_Shutdown` | RTE-generated symbol |
| `Rte_Enter_StaMds_MilestoneRqst_WARMINIT_ExclArea` | RTE-generated symbol |
| `Rte_Exit_StaMds_MilestoneRqst_WARMINIT_ExclArea` | RTE-generated symbol |
| `Rte_Call_CloseCheckData_GetErrorStatus` | RTE-generated symbol |
| `Rte_Call_TypeHData_WriteBlock` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_StaMd_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Os.h` `Rte_Ap_StaMd.h` `Std_Types.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_StaMd_Cfg.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h` `Os.h` `Rte.h` `Rte_Ap_StaMd.h` `Rte_Compiler_Cfg.h` `Rte_Hook.h` `Rte_Type.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [StaMd — States_And_Modes_GeneratedConfiguration_MDD](./StaMd-States_And_Modes_GeneratedConfiguration_MDD/) | `StaMd/doc/States_And_Modes_GeneratedConfiguration_MDD.docx` |
| [StaMd — States_And_Modes_MDD](./StaMd-States_And_Modes_MDD/) | `StaMd/doc/States_And_Modes_MDD.docx` |

*Repository path: `StaMd/`* 
