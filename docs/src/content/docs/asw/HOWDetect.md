---
title: "HOWDetect"
description: "HOWDetect: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_HOWDetect).*
## Purpose and responsibility
Software area `HOWDetect` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_HOWDetect.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_HOWDetect.arxml` |
| Generation templates | `Ap_HOWDetect_Cfg.arxml.tt`, `Ap_HOWDetect_Cfg.h.tt`, `Ap_HOWDetect_Generate.bat`, `Ap_HOWDetect_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (8 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_HOWDetect_Per1_HwTrq_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_HOWDetect_Per1_VehSpd_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_HOWDetect_Per1_HOWEstimate_Uls_f32` | RTE-generated symbol |
| `Rte_IWriteRef_HOWDetect_Per1_HOWEstimate_Uls_f32` | RTE-generated symbol |
| `Rte_IWrite_HOWDetect_Per1_HOWState_Cnt_s08` | RTE-generated symbol |
| `Rte_IWriteRef_HOWDetect_Per1_HOWState_Cnt_s08` | RTE-generated symbol |
| `Rte_Call_HOWDetect_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_HOWDetect_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_HOWDetect_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_HOWDetect.h` `filters.h` `fixmath.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_HOWDetect` `Ap_HOWDetect_Cfg.h` `Rte.h` `Rte_Ap_HOWDetect.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [HOWDetect — HOWDetect_Integration_Manual](./HOWDetect-HOWDetect_Integration_Manual/) | `HOWDetect/doc/HOWDetect_Integration_Manual.docx` |
| [HOWDetect — HOWDetect_MDD](./HOWDetect-HOWDetect_MDD/) | `HOWDetect/doc/HOWDetect_MDD.docx` |

*Repository path: `HOWDetect/`* 
