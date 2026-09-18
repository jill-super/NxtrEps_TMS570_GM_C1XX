---
title: "Assist"
description: "Assist: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_Assist).*
## Purpose and responsibility
Software area `Assist` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_Assist.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_Assist.arxml` |
| Generation templates | `Ap_Assist_Cfg.arxml.tt`, `Ap_Assist_Cfg.h.tt`, `Ap_Assist_Generate.bat`, `Ap_Assist_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (14 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_Assist_Per1_AssistDDFactor_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_Assist_Per1_DftAsstTbl_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_Assist_Per1_DutyCycleLevel_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_Assist_Per1_DwnldAsstGain_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_Assist_Per1_HwTrqHysAdd_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_Assist_Per1_HwTrq_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_Assist_Per1_IpTrqOvr_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_Assist_Per1_VehSpd_Kph_f32` | RTE-generated symbol |
| `Rte_IRead_Assist_Per1_WIRCmdAmpBlnd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_Assist_Per1_BaseAssistCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_Assist_Per1_BaseAssistCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_FltInjection_SCom_FltInjection` | RTE-generated symbol |
| `Rte_Call_Assist_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_Assist_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_Assist_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_Assist.h` `filters.h` `fixmath.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_Assist` `Ap_Assist_Cfg.h` `Rte.h` `Rte_Ap_Assist.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [Assist — Assist_Integration_Manual](./Assist-Assist_Integration_Manual/) | `Assist/doc/Assist_Integration_Manual.docx` |
| [Assist — Assist_MDD](./Assist-Assist_MDD/) | `Assist/doc/Assist_MDD.docx` |

*Repository path: `Assist/`* 
