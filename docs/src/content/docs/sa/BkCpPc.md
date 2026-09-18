---
title: "BkCpPc"
description: "BkCpPc: purpose, files, API and documents (Sensor / Actuator Abstraction)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Sa_BkCpPc).*
## Purpose and responsibility
Software area `BkCpPc` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Sa_BkCpPc.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Sa_BkCpPc.arxml` |
| Generation templates | `Sa_BkCpPc_Cfg.arxml.tt`, `Sa_BkCpPc_Cfg.h.tt`, `Sa_BkCpPc_Generate.bat`, `Sa_BkCpPc_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (31 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_BkCpPc_Per1_BattSwitched_Volt_f32` | RTE-generated symbol |
| `Rte_IRead_BkCpPc_Per1_Batt_Volt_f32` | RTE-generated symbol |
| `Rte_IRead_BkCpPc_Per1_MotorVelocityMRFUnfiltered_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_BkCpPc_Per1_OVERRIDESIGDIAGADC_Volt_f32` | RTE-generated symbol |
| `Rte_IRead_BkCpPc_Per1_PMOSDIAGADC_Volt_f32` | RTE-generated symbol |
| `Rte_IRead_BkCpPc_Per1_PwrDiscATestStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_BkCpPc_Per1_PwrDiscBTestStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_BkCpPc_Per1_PwrDiscATestComplete_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_BkCpPc_Per1_PwrDiscATestComplete_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_BkCpPc_Per1_PwrDiscBTestComplete_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_BkCpPc_Per1_PwrDiscBTestComplete_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_BkCpPc_Per1_PwrDiscClosed_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_BkCpPc_Per1_PwrDiscClosed_Cnt_lgc` | RTE-generated symbol |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_PhyCapDischarge_OP_SET` | RTE-generated symbol |
| `Rte_Call_PhyCapPrecharge_OP_SET` | RTE-generated symbol |
| `Rte_Call_SystemTime_DtrmnElapsedTime_mS_u16` | RTE-generated symbol |
| `Rte_Call_SystemTime_GetSystemTime_mS_u32` | RTE-generated symbol |
| `Rte_Call_BkCpPc_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_BkCpPc_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IWrite_BkCpPc_Trns1_PwrDiscATestComplete_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_BkCpPc_Trns1_PwrDiscATestComplete_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_BkCpPc_Trns1_PwrDiscBTestComplete_Cnt_lgc` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Sa_BkCpPc.h` `Sa_BkCpPc_Cfg.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`CalConstants.h` `Compiler_Cfg.h` `MemMap.h` `Sa_BkCpPc` `Rte.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Sa_BkCpPc.h` `Rte_Type.h` `Sa_BkCpPc_Cfg.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [BkCpPc — Bulk_Cap_Precharge_MDD](./BkCpPc-Bulk_Cap_Precharge_MDD/) | `BkCpPc/doc/Bulk_Cap_Precharge_MDD.docx` |

*Repository path: `BkCpPc/`* 
