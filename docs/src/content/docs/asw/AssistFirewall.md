---
title: "AssistFirewall"
description: "AssistFirewall: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_AssistFirewall).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> description: "Converted .docx document from AssistFirewall/doc."

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_AssistFirewall.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_AssistFirewall.arxml` |
| Generation templates | `Ap_AssistFirewall_Cfg.arxml.tt`, `Ap_AssistFirewall_Cfg.h.tt`, `Ap_AssistFirewall_Generate.bat`, `Ap_AssistFirewall_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (14 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_AssistFirewall_Per1_BaseAssistCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_AssistFirewall_Per1_Defeat_AsstTbl_Service_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_AssistFirewall_Per1_HighFreqAssist_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_AssistFirewall_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_AssistFirewall_Per1_HysteresisComp_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_AssistFirewall_Per1_MEC_Counter_Cnt_enum` | RTE-generated symbol |
| `Rte_IRead_AssistFirewall_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_AssistFirewall_Per1_AsstFirewallActive_Uls_f32` | RTE-generated symbol |
| `Rte_IWriteRef_AssistFirewall_Per1_AsstFirewallActive_Uls_f32` | RTE-generated symbol |
| `Rte_IWrite_AssistFirewall_Per1_CombinedAssist_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_AssistFirewall_Per1_CombinedAssist_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_AssistFirewall_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_AssistFirewall_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_AssistFirewall_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_AssistFirewall.h` `filters.h` `fixmath.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_AssistFirewall` `Rte.h` `Rte_Ap_AssistFirewall.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `Ap_AssistFirewall_Cfg.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [AssistFirewall — Assist_Firewall_MDD](./AssistFirewall-Assist_Firewall_MDD/) | `AssistFirewall/doc/Assist_Firewall_MDD.docx` |

*Repository path: `AssistFirewall/`* 
