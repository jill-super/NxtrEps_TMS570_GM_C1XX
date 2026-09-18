---
title: "AstLmt_CM"
description: "AstLmt_CM: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_AstLmt).*
## Purpose and responsibility
Software area `AstLmt_CM` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_AstLmt.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_AstLmt.arxml` |
| Generation templates | `Ap_AstLmt_Cfg.arxml.tt`, `Ap_AstLmt_Cfg.h.tt`, `Ap_AstLmt_Generate.bat`, `Ap_AstLmt_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (38 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Pim_SteerAsstDefeat` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_AssistCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_AssistEOTDamping_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_AssistEOTGain_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_AssistEOTLimit_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_AssistStallLimit_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_AssistVehSpdLimit_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_CombinedDamping_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_DefeatLimitService_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_LimitedReturn_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_LrnPnCtrCCDisable_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_LrnPnCtrEnable_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_LrnPnCtrTCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_OpTrqOvr_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_OutputRampMult_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_PosServCCDisable_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_PowerLimitPerc_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_PrkAssistCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_PullCompCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_TSMitCommand_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_ThermalLimitPerc_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_ThermalLimit_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_VehSpd_Kph_f32` | RTE-generated symbol |
| `Rte_IRead_AstLmt_Per1_WheelImbalanceCmd_MtrNm_f32` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_AstLmt_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_AstLmt.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_AstLmt` `Ap_AstLmt_Cfg.h` `Rte.h` `Rte_Ap_AstLmt.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [AstLmt_CM — Assist_Sum_Limit_CurrentMode_MDD](./AstLmt_CM-Assist_Sum_Limit_CurrentMode_MDD/) | `AstLmt_CM/doc/Assist_Sum_Limit_CurrentMode_MDD.docx` |
| [AstLmt_CM — AstLmt_CM_IntegrationManual](./AstLmt_CM-AstLmt_CM_IntegrationManual/) | `AstLmt_CM/doc/AstLmt_CM_IntegrationManual.docx` |

*Repository path: `AstLmt_CM/`* 
