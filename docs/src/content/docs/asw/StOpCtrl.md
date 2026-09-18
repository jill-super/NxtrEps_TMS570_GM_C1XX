---
title: "StOpCtrl"
description: "StOpCtrl: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_StOpCtrl).*
## Purpose and responsibility
Software area `StOpCtrl` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_StOpCtrl.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_StOpCtrl.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (14 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_StOpCtrl_Per1_DiagRampRate_XpmS_f32` | RTE-generated symbol |
| `Rte_IRead_StOpCtrl_Per1_DiagRampValue_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_StOpCtrl_Per1_DiagStsDiagRmpActive_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_StOpCtrl_Per1_LoaRateLimit_UlspS_f32` | RTE-generated symbol |
| `Rte_IRead_StOpCtrl_Per1_LoaScaleFctr_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_StOpCtrl_Per1_OperRampRate_XpmS_f32` | RTE-generated symbol |
| `Rte_IRead_StOpCtrl_Per1_OperRampValue_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_StOpCtrl_Per1_RampSrlComSvcDft_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_StOpCtrl_Per1_StrtStopRateLimit_UlspS_f32` | RTE-generated symbol |
| `Rte_IRead_StOpCtrl_Per1_StrtStopScaleFctr_Uls_f32` | RTE-generated symbol |
| `Rte_IWrite_StOpCtrl_Per1_OutputRampMult_Uls_f32` | RTE-generated symbol |
| `Rte_IWriteRef_StOpCtrl_Per1_OutputRampMult_Uls_f32` | RTE-generated symbol |
| `Rte_IWrite_StOpCtrl_Per1_SysStReqDi_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_StOpCtrl_Per1_SysStReqDi_Cnt_lgc` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`GlobalMacro.h` `MemMap.h` `Rte_Ap_StOpCtrl.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [StOpCtrl — StateOutput Control_IntegrationManual](./StOpCtrl-StateOutput-Control_IntegrationManual/) | `StOpCtrl/doc/StateOutput Control_IntegrationManual.docx` |
| [StOpCtrl — State_Output_Control_MDD](./StOpCtrl-State_Output_Control_MDD/) | `StOpCtrl/doc/State_Output_Control_MDD.docx` |

*Repository path: `StOpCtrl/`* 
