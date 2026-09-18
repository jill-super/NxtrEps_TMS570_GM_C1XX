---
title: "BatteryVoltage"
description: "BatteryVoltage: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_BatteryVoltage).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> description: "Converted .docx document from BatteryVoltage/doc."

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_BatteryVoltage.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_BatteryVoltage.arxml` |
| Generation templates | `Ap_BatteryVoltage_Cfg.arxml.tt`, `Ap_BatteryVoltage_Cfg.h.tt`, `Ap_BatteryVoltage_Generate.bat`, `Ap_BatteryVoltage_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (20 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Pim_OvervoltageData` | RTE-generated symbol |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_IRead_BatteryVoltage_Per1_BattSwitched_Volt_f32` | RTE-generated symbol |
| `Rte_IRead_BatteryVoltage_Per1_Batt_Volt_f32` | RTE-generated symbol |
| `Rte_IWrite_BatteryVoltage_Per1_SysC_Vecu_Volt_f32` | RTE-generated symbol |
| `Rte_IWriteRef_BatteryVoltage_Per1_SysC_Vecu_Volt_f32` | RTE-generated symbol |
| `Rte_IWrite_BatteryVoltage_Per1_Vecu_Volt_f32` | RTE-generated symbol |
| `Rte_IWriteRef_BatteryVoltage_Per1_Vecu_Volt_f32` | RTE-generated symbol |
| `Rte_IWrite_BatteryVoltage_Per1_VswitchClosed_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_BatteryVoltage_Per1_VswitchClosed_Cnt_lgc` | RTE-generated symbol |
| `Rte_Call_FltInjection_SCom_FltInjection` | RTE-generated symbol |
| `Rte_Call_BatteryVoltage_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_BatteryVoltage_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IRead_BatteryVoltage_Per2_BattSwitched_Volt_f32` | RTE-generated symbol |
| `Rte_IRead_BatteryVoltage_Per2_SysCVSwitch_Volt_f32` | RTE-generated symbol |
| `Rte_Call_BatteryVoltage_Per2_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_BatteryVoltage_Per2_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_OvervoltageData_SetRamBlockStatus` | RTE-generated symbol |
| `Rte_Call_OvervoltageData_WriteBlock` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_BatteryVoltage_Cfg.h` `BatteryVoltage_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Os.h` `Rte_Ap_BatteryVoltage.h` `adc_regs.h` `fixmath.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_BatteryVoltage` `Ap_BatteryVoltage_Cfg.h` `Rte.h` `Rte_Ap_BatteryVoltage.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [BatteryVoltage — BatteryVoltage_Integration_Manual](./BatteryVoltage-BatteryVoltage_Integration_Manual/) | `BatteryVoltage/doc/BatteryVoltage_Integration_Manual.docx` |
| [BatteryVoltage — Battery_Voltage_MDD](./BatteryVoltage-Battery_Voltage_MDD/) | `BatteryVoltage/doc/Battery_Voltage_MDD.doc` |

*Repository path: `BatteryVoltage/`* 
