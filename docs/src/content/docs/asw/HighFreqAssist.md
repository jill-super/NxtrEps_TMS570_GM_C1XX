---
title: "HighFreqAssist"
description: "HighFreqAssist: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_HighFreqAssist).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> description: "Converted .docx document from HighFreqAssist/doc."

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_HighFreqAssist.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_HighFreqAssist.arxml` |
| Generation templates | `Ap_HighFreqAssist_Cfg.arxml.tt`, `Ap_HighFreqAssist_Cfg.h.tt`, `Ap_HighFreqAssist_Generate.bat`, `Ap_HighFreqAssist_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (7 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_HighFreqAssist_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_HighFreqAssist_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IRead_HighFreqAssist_Per1_WIRCmdAmpBlnd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_HighFreqAssist_Per1_HighFreqAssist_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_HighFreqAssist_Per1_HighFreqAssist_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_HighFreqAssist_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_HighFreqAssist_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_HighFreqAssist_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_HighFreqAssist.h` `filters.h` `fixmath.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_HighFreqAssist` `Ap_HighFreqAssist_Cfg.h` `Rte.h` `Rte_Ap_HighFreqAssist.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [HighFreqAssist — HighFreqAssist_Integration_Manual](./HighFreqAssist-HighFreqAssist_Integration_Manual/) | `HighFreqAssist/doc/HighFreqAssist_Integration_Manual.docx` |
| [HighFreqAssist — High_Frequency_Assist_MDD](./HighFreqAssist-High_Frequency_Assist_MDD/) | `HighFreqAssist/doc/High_Frequency_Assist_MDD.docx` |

*Repository path: `HighFreqAssist/`* 
