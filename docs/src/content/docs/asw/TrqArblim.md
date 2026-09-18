---
title: "TrqArblim"
description: "TrqArblim: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_TrqArblim).*
## Purpose and responsibility
Software area `TrqArblim` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_TrqArblim.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_TrqArblim.arxml` |
| Generation templates | `Ap_TrqArblim_Cfg.arxml.tt`, `Ap_TrqArblim_Cfg.h.tt`, `Ap_TrqArblim_Generate.bat`, `Ap_TrqArblim_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (30 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_IRead_TrqArblim_Per1_ESCCmd_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_TrqArblim_Per1_ESCState_State_enum` | RTE-generated symbol |
| `Rte_IRead_TrqArblim_Per1_GMOSHOscillate_State_enum` | RTE-generated symbol |
| `Rte_IRead_TrqArblim_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_TrqArblim_Per1_LKACmd_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_TrqArblim_Per1_LKAState_State_enum` | RTE-generated symbol |
| `Rte_IRead_TrqArblim_Per1_MaxSecureVehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IRead_TrqArblim_Per1_PosServEnable_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TrqArblim_Per1_PosSrvoCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_TrqArblim_Per1_TrqOscCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_TrqArblim_Per1_AssistDDFactor_Uls_f32` | RTE-generated symbol |
| `Rte_IWriteRef_TrqArblim_Per1_AssistDDFactor_Uls_f32` | RTE-generated symbol |
| `Rte_IWrite_TrqArblim_Per1_DampingDDFactor_Uls_f32` | RTE-generated symbol |
| `Rte_IWriteRef_TrqArblim_Per1_DampingDDFactor_Uls_f32` | RTE-generated symbol |
| `Rte_IWrite_TrqArblim_Per1_ESCIsLimited_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_TrqArblim_Per1_ESCIsLimited_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_TrqArblim_Per1_ESCTorqueDelivered_HwNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_TrqArblim_Per1_ESCTorqueDelivered_HwNm_f32` | RTE-generated symbol |
| `Rte_IWrite_TrqArblim_Per1_IqTrqOv_HwNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_TrqArblim_Per1_IqTrqOv_HwNm_f32` | RTE-generated symbol |
| `Rte_IWrite_TrqArblim_Per1_LKATorqueDelivered_HwNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_TrqArblim_Per1_LKATorqueDelivered_HwNm_f32` | RTE-generated symbol |
| `Rte_IWrite_TrqArblim_Per1_OpTrqOv_MtrNm_f32` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_TrqArblim_Cfg.h` `CalConstants.h` `GlobalMacro.h` `Interpolation.h` `MemMap.h` `Rte_Ap_TrqArblim.h` `filters.h` `fixmath.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_TrqArblim` `Ap_TrqArblim_Cfg.h` `Rte.h` `Rte_Ap_TrqArblim.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [TrqArblim — TrqArblim_Integration_Manual](./TrqArblim-TrqArblim_Integration_Manual/) | `TrqArblim/doc/TrqArblim_Integration_Manual.docx` |
| [TrqArblim — TrqArblim_MDD](./TrqArblim-TrqArblim_MDD/) | `TrqArblim/doc/TrqArblim_MDD.docx` |

*Repository path: `TrqArblim/`* 
