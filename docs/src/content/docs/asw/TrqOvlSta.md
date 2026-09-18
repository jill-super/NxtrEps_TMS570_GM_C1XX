---
title: "TrqOvlSta"
description: "TrqOvlSta: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_TrqOvlSta).*
## Purpose and responsibility
Software area `TrqOvlSta` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_TrqOvlSta.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_TrqOvlSta.arxml` |
| Generation templates | `Ap_TrqOvlSta_Cfg.arxml.tt`, `Ap_TrqOvlSta_Cfg.h.tt`, `Ap_TrqOvlSta_Generate.bat`, `Ap_TrqOvlSta_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (48 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_Call_SystemTime_GetSystemTime_mS_u32` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_APANonRecoverableFaults_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_APARecoverableFaults_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_APARequest_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_CCWPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_CWPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_ESCFault_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_ESCIsLimited_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_ESCRequest_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_GMOSH_APAMfgEnable_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_GMOSH_ESCMfgEnable_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_GMOSH_LKAMfgEnable_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_HapticRequest_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_LKAFault_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_LKAInhibit_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_LKARequest_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_MaxSecureVehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_MinSecureVehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_PosTrajEnable_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_PosTrajHwAngle_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_SWARTrgtAngRequest_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_TrqOvlSta_Per1_ShiftLeverIsInReverse_Cnt_lgc` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_TrqOvlSta_Cfg.h` `CalConstants.h` `GlobalMacro.h` `Interpolation.h` `MemMap.h` `Rte_Ap_TrqOvlSta.h` `filters.h` `fixmath.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_TrqOvlSta` `Ap_TrqOvlSta_Cfg.h` `Rte.h` `Rte_Ap_TrqOvlSta.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [TrqOvlSta — TrqOvlSta_Integration_Manual](./TrqOvlSta-TrqOvlSta_Integration_Manual/) | `TrqOvlSta/doc/TrqOvlSta_Integration_Manual.docx` |
| [TrqOvlSta — TrqOvlSta_MDD](./TrqOvlSta-TrqOvlSta_MDD/) | `TrqOvlSta/doc/TrqOvlSta_MDD.docx` |

*Repository path: `TrqOvlSta/`* 
