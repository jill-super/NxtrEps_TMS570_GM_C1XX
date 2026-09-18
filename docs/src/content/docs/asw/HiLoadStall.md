---
title: "HiLoadStall"
description: "HiLoadStall: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_HiLoadStall).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> description: "Converted .docx document from HiLoadStall/doc."

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_HiLoadStall.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_HiLoadStall.arxml` |
| Generation templates | `Ap_HiLoadStall_Cfg.arxml.tt`, `Ap_HiLoadStall_Cfg.h.tt`, `Ap_HiLoadStall_Generate.bat`, `Ap_HiLoadStall_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (7 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_HiLoadStall_Per1_DftStallLimit_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_HiLoadStall_Per1_MtrVelCRF_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_HiLoadStall_Per1_PreLimitForStall_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_HiLoadStall_Per1_AssistStallLimit_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_HiLoadStall_Per1_AssistStallLimit_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_HiLoadStall_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_HiLoadStall_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_HiLoadStall_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_HiLoadStall.h` `filters.h` `fixmath.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_HiLoadStall_Cfg.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h` `Rte.h` `Rte_Ap_HiLoadStall.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [HiLoadStall — HiLoadStall](./HiLoadStall-HiLoadStall/) | `HiLoadStall/doc/HiLoadStall.docx` |

*Repository path: `HiLoadStall/`* 
