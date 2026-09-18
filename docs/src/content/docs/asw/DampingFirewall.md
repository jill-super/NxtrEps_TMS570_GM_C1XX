---
title: "DampingFirewall"
description: "DampingFirewall: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_DampingFirewall).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> description: "Converted .docx document from DampingFirewall/doc."

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_DampingFirewall.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_DampingFirewall.arxml` |
| Generation templates | `Ap_DampingFirewall_Cfg.arxml.tt`, `Ap_DampingFirewall_Cfg.h.tt`, `Ap_DampingFirewall_Generate.bat`, `Ap_DampingFirewall_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (18 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_IRead_DampingFirewall_Per1_AsstFirewallActive_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_DampingFirewall_Per1_BaseAssistCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_DampingFirewall_Per1_DampingCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_DampingFirewall_Per1_Defeat_Damping_Svc_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_DampingFirewall_Per1_FreqDepDmpSrlComSvcDft_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_DampingFirewall_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_DampingFirewall_Per1_InertiaComp_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_DampingFirewall_Per1_MEC_Counter_Cnt_enum` | RTE-generated symbol |
| `Rte_IRead_DampingFirewall_Per1_MtrVelCRF_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_DampingFirewall_Per1_VehicleLonAccel_KphpS_f32` | RTE-generated symbol |
| `Rte_IRead_DampingFirewall_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IRead_DampingFirewall_Per1_WIRCmdAmpBlnd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_DampingFirewall_Per1_CombinedDamping_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_DampingFirewall_Per1_CombinedDamping_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_DampingFirewall_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_DampingFirewall_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_DampingFirewall_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_DampingFirewall.h` `filters.h` `fixmath.h` `interpolation.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [DampingFirewall — DampingFirewall_IntegrationManual](./DampingFirewall-DampingFirewall_IntegrationManual/) | `DampingFirewall/doc/DampingFirewall_IntegrationManual.docx` |
| [DampingFirewall — Damping_Firewall_MDD](./DampingFirewall-Damping_Firewall_MDD/) | `DampingFirewall/doc/Damping_Firewall_MDD.doc` |

*Repository path: `DampingFirewall/`* 
