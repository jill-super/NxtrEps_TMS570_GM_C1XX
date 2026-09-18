---
title: "HwPwUp"
description: "HwPwUp: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_HwPwUp).*
## Purpose and responsibility
Software area `HwPwUp` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_HwPwUp.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_HwPwUp.arxml` |
| Generation templates | `Ap_HwPwUp_Cfg.arxml.tt`, `Ap_HwPwUp_Cfg.h.tt`, `Ap_HwPwUp_Generate.bat`, `Ap_HwPwUp_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (25 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_HwPwUp_Per1_MtrDrvrInitComplete_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_HwPwUp_Per1_PwrDiscATestComplete_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_HwPwUp_Per1_PwrDiscBTestComplete_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_HwPwUp_Per1_TMFTestComplete_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_HwPwUp_Per1_MtrDrvrInitStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_HwPwUp_Per1_MtrDrvrInitStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_HwPwUp_Per1_PwrDiscATestStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_HwPwUp_Per1_PwrDiscATestStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_HwPwUp_Per1_PwrDiscBTestStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_HwPwUp_Per1_PwrDiscBTestStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_HwPwUp_Per1_TMFTestStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_HwPwUp_Per1_TMFTestStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_Call_MilestoneRqst_WarmInitMilestoneComplete` | RTE-generated symbol |
| `Rte_Call_HwPwUp_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_HwPwUp_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IWrite_HwPwUp_Trns1_MtrDrvrInitStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_HwPwUp_Trns1_MtrDrvrInitStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_HwPwUp_Trns1_PwrDiscATestStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_HwPwUp_Trns1_PwrDiscATestStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_HwPwUp_Trns1_PwrDiscBTestStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_HwPwUp_Trns1_PwrDiscBTestStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_HwPwUp_Trns1_TMFTestStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_HwPwUp_Trns1_TMFTestStart_Cnt_lgc` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_HwPwUp_Cfg.h` `CalConstants.h` `MemMap.h` `Rte_Ap_HwPwUp.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_HwPwUp` `Ap_HwPwUp_Cfg.h` `Rte.h` `Rte_Ap_HwPwUp.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [HwPwUp — Hardware_Power_Up_MDD](./HwPwUp-Hardware_Power_Up_MDD/) | `HwPwUp/doc/Hardware_Power_Up_MDD.docx` |

*Repository path: `HwPwUp/`* 
