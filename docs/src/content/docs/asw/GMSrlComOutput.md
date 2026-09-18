---
title: "GMSrlComOutput"
description: "GMSrlComOutput: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_SrlComOutput).*
## Purpose and responsibility
Software area `GMSrlComOutput` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_SrlComOutput.c` |
| `include/` | `Ap_SrlComOutput.h` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_SrlComOutput.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (30 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Pim_DTCTrigSts` | RTE-generated symbol |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_Call_ComM_UserRequest_0_RequestComMode` | RTE-generated symbol |
| `Rte_Call_ComM_UserRequest_1_RequestComMode` | RTE-generated symbol |
| `Rte_Call_ComM_UserRequest_2_RequestComMode` | RTE-generated symbol |
| `Rte_Call_ComM_UserRequest_3_RequestComMode` | RTE-generated symbol |
| `Rte_Call_ComM_UserRequest_4_RequestComMode` | RTE-generated symbol |
| `Rte_Call_ComM_UserRequest_5_RequestComMode` | RTE-generated symbol |
| `Rte_Read_APADrvrInterventionDetected_Cnt_lgc` | RTE-generated symbol |
| `Rte_Read_APAState_State_enum` | RTE-generated symbol |
| `Rte_Read_DiagRmpToZeroActive_Cnt_lgc` | RTE-generated symbol |
| `Rte_Read_ESCState_State_enum` | RTE-generated symbol |
| `Rte_Read_ESCTorqueDelivered_HwNm_f32` | RTE-generated symbol |
| `Rte_Read_HOWEstimate_Uls_f32` | RTE-generated symbol |
| `Rte_Read_HwTrq_HwNm_f32` | RTE-generated symbol |
| `Rte_Read_LKAState_State_enum` | RTE-generated symbol |
| `Rte_Read_LKATrqDelivered_HwNm_f32` | RTE-generated symbol |
| `Rte_Call_SystemTime_DtrmnElapsedTime_mS_u16` | RTE-generated symbol |
| `Rte_Call_SystemTime_GetSystemTime_mS_u32` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_GetNTCActive` | RTE-generated symbol |
| `Rte_Read_DiagStsHwPosDis_Cnt_lgc` | RTE-generated symbol |
| `Rte_Read_HandwheelVel_HwRadpS_f32` | RTE-generated symbol |
| `Rte_Read_HwVelValid_Cnt_lgc` | RTE-generated symbol |
| `Rte_Read_SrlComHwPos_HwDeg_f32` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_DemIf.h` `Ap_DfltConfigData.h` `Ap_SrlComOutput.h` `Ap_SrlComOutput_Cfg.h` `CDD_Data.h` `CalConstants.h` `Dem.h` `Dem_Lcfg.h` `DiagMgr_Cfg.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_SrlComOutput.h` `T1_AppInterface.h` `can_par.h` `fixmath.h` `il_inc.h` `il_par.h` `string.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_DemIf.h` `Ap_DfltConfigData.h` `Ap_SrlComOutput_Cfg.h` `CDD_Data.h` `CalConstants.h` `Compiler_Cfg.h` `Dem.h` `Dem_Lcfg.h` `DiagMgr_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [GMSrlComOutput — Serial_Communication_Output_MDD](./GMSrlComOutput-Serial_Communication_Output_MDD/) | `GMSrlComOutput/doc/Serial_Communication_Output_MDD.doc` |

*Repository path: `GMSrlComOutput/`* 
