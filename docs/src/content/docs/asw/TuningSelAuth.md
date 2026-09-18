---
title: "TuningSelAuth"
description: "TuningSelAuth: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_TuningSelAuth).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> description: "Converted .docx document from TuningSelAuth/doc."

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_TuningSelAuth.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_TuningSelAuth.arxml` |
| Generation templates | `Ap_TuningSelAuth_Cfg.arxml.tt`, `Ap_TuningSelAuth_Cfg.h.tt`, `Ap_TuningSelAuth_Generate.bat`, `Ap_TuningSelAuth_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (18 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_TuningSelAuth_Init1_DesiredTunPers_Cnt_u16` | RTE-generated symbol |
| `Rte_IRead_TuningSelAuth_Init1_DesiredTunSet_Cnt_u16` | RTE-generated symbol |
| `Rte_IWrite_TuningSelAuth_Init1_ActiveTunPers_Cnt_u16` | RTE-generated symbol |
| `Rte_IWriteRef_TuningSelAuth_Init1_ActiveTunPers_Cnt_u16` | RTE-generated symbol |
| `Rte_IWrite_TuningSelAuth_Init1_ActiveTunSet_Cnt_u16` | RTE-generated symbol |
| `Rte_IWriteRef_TuningSelAuth_Init1_ActiveTunSet_Cnt_u16` | RTE-generated symbol |
| `Rte_IRead_TuningSelAuth_Per1_ActiveTunOvrPtrAddr_Cnt_u32` | RTE-generated symbol |
| `Rte_IRead_TuningSelAuth_Per1_DesiredTunPers_Cnt_u16` | RTE-generated symbol |
| `Rte_IRead_TuningSelAuth_Per1_DesiredTunSet_Cnt_u16` | RTE-generated symbol |
| `Rte_IRead_TuningSelAuth_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_TuningSelAuth_Per1_TuningSessionActPtr_Cnt_u8` | RTE-generated symbol |
| `Rte_IRead_TuningSelAuth_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_TuningSelAuth_Per1_ActiveTunPers_Cnt_u16` | RTE-generated symbol |
| `Rte_IWriteRef_TuningSelAuth_Per1_ActiveTunPers_Cnt_u16` | RTE-generated symbol |
| `Rte_IWrite_TuningSelAuth_Per1_ActiveTunSet_Cnt_u16` | RTE-generated symbol |
| `Rte_IWriteRef_TuningSelAuth_Per1_ActiveTunSet_Cnt_u16` | RTE-generated symbol |
| `Rte_Call_TuningSelAuth_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_TuningSelAuth_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_TuningSelAuth_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_TuningSelAuth.h` `XcpProf.h` `filters.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_TuningSelAuth_Cfg.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h` `Rte.h` `Rte_Ap_TuningSelAuth.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [TuningSelAuth — Tuning_Select_Authority_MDD](./TuningSelAuth-Tuning_Select_Authority_MDD/) | `TuningSelAuth/doc/Tuning_Select_Authority_MDD.docx` |

*Repository path: `TuningSelAuth/`* 
