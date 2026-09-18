---
title: "ReturnFirewall"
description: "ReturnFirewall: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_ReturnFirewall).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> description: "Converted .docx document from ReturnFirewall/doc."

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_ReturnFirewall.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_ReturnFirewall.arxml` |
| Generation templates | `Ap_ReturnFirewall_Cfg.arxml.tt`, `Ap_ReturnFirewall_Cfg.h.tt`, `Ap_ReturnFirewall_Generate.bat`, `Ap_ReturnFirewall_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (10 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_ReturnFirewall_Per1_Defeat_Return_Svc_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_ReturnFirewall_Per1_HandwheelPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_ReturnFirewall_Per1_MEC_Counter_Cnt_enum` | RTE-generated symbol |
| `Rte_IRead_ReturnFirewall_Per1_ReturnCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_ReturnFirewall_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_ReturnFirewall_Per1_LimitedReturn_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_ReturnFirewall_Per1_LimitedReturn_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_ReturnFirewall_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_ReturnFirewall_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_ReturnFirewall_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_ReturnFirewall.h` `fixmath.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_ReturnFirewall` `Rte.h` `Rte_Ap_ReturnFirewall.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `Ap_ReturnFirewall_Cfg.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [ReturnFirewall — Return_Firewall_MDD](./ReturnFirewall-Return_Firewall_MDD/) | `ReturnFirewall/doc/Return_Firewall_MDD.docx` |

*Repository path: `ReturnFirewall/`* 
