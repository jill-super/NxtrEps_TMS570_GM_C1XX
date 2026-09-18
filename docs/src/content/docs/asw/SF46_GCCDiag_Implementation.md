---
title: "SF46_GCCDiag_Implementation"
description: "SF46_GCCDiag_Implementation: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_GCCDiag).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> title: "SF46_GCCDiag_Implementation — GCCDiag_Integration_Manual"

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_GCCDiag.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_GCCDiag.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (6 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_GCCDiag_Per1_DftGrossCCDiag_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_GCCDiag_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_GCCDiag_Per1_MRFMtrTrqCmdScl_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_GCCDiag_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_Call_FltInjection_SCom_FltInjection` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_GCCDiag.h` `filters.h` `fixmath.h` `interpolation.h`
## Documents
| Document | Source file |
| --- | --- |
| [SF46_GCCDiag_Implementation — GCCDiag_Integration_Manual](./SF46_GCCDiag_Implementation-GCCDiag_Integration_Manual/) | `SF46_GCCDiag_Implementation/doc/GCCDiag_Integration_Manual.docx` |
| [SF46_GCCDiag_Implementation — GCCDiag_MDD](./SF46_GCCDiag_Implementation-GCCDiag_MDD/) | `SF46_GCCDiag_Implementation/doc/GCCDiag_MDD.docx` |

*Repository path: `SF46_GCCDiag_Implementation/`* 
