---
title: "VehDyn"
description: "VehDyn: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_VehDyn).*
## Purpose and responsibility
Software area `VehDyn` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_VehDyn.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_VehDyn.arxml` |
| Generation templates | `Ap_VehDyn_Cfg.arxml.tt`, `Ap_VehDyn_Cfg.h.tt`, `Ap_VehDyn_Generate.bat`, `Ap_VehDyn_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (26 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Pim_MotPosReset` | RTE-generated symbol |
| `Rte_IRead_VehDyn_Init1_RelHwPos_HwDeg_f32` | RTE-generated symbol |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_GetNTCActive` | RTE-generated symbol |
| `Rte_Call_NVM_VehDynReset_Srv_ReadBlock` | RTE-generated symbol |
| `Rte_Call_SystemTime_GetSystemTime_mS_u32` | RTE-generated symbol |
| `Rte_IRead_VehDyn_Per1_CcwEOT_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_VehDyn_Per1_CwEOT_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_VehDyn_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_VehDyn_Per1_MotorVelCRF_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_VehDyn_Per1_RelHwPos_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_VehDyn_Per1_TorqueCmdCRF_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_VehDyn_Per1_VehicleSpeedValid_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_VehDyn_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_VehDyn_Per1_SensorlessAuthority_Uls_f32` | RTE-generated symbol |
| `Rte_IWriteRef_VehDyn_Per1_SensorlessAuthority_Uls_f32` | RTE-generated symbol |
| `Rte_IWrite_VehDyn_Per1_SensorlessHwPos_HwDeg_f32` | RTE-generated symbol |
| `Rte_IWriteRef_VehDyn_Per1_SensorlessHwPos_HwDeg_f32` | RTE-generated symbol |
| `Rte_Call_SystemTime_DtrmnElapsedTime_mS_u32` | RTE-generated symbol |
| `Rte_Call_VehDyn_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_VehDyn_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_Read_RelHwPos_HwDeg_f32` | RTE-generated symbol |
| `Rte_Call_NVM_VehDynReset_Srv_WriteBlock` | RTE-generated symbol |
| `Rte_IRead_VehDyn_Trns1_HandwheelPosition_HwDeg_f32` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_VehDyn_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_VehDyn.h` `SystemTime.h` `filters.h` `fixmath.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_VehDyn` `Ap_VehDyn_Cfg.h` `Rte.h` `Rte_Ap_VehDyn.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [VehDyn — VehDyn_Integration_Manual](./VehDyn-VehDyn_Integration_Manual/) | `VehDyn/doc/VehDyn_Integration_Manual.docx` |
| [VehDyn — VehDyn_MDD](./VehDyn-VehDyn_MDD/) | `VehDyn/doc/VehDyn_MDD.docx` |

*Repository path: `VehDyn/`* 
