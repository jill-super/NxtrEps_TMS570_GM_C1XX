---
title: "VehSpdLmt"
description: "VehSpdLmt: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_VehSpdLmt).*
## Purpose and responsibility
Software area `VehSpdLmt` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_VehSpdLmt.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_VehSpdLmt.arxml` |
| Generation templates | `Ap_VehSpdLmt_Cfg.arxml.tt`, `Ap_VehSpdLmt_Cfg.h.tt`, `Ap_VehSpdLmt_Generate.bat`, `Ap_VehSpdLmt_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (9 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_VehSpdLmt_Per1_CCWPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_VehSpdLmt_Per1_CWPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_VehSpdLmt_Per1_HwPosAuth_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_VehSpdLmt_Per1_HwPos_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_VehSpdLmt_Per1_VehSpd_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_VehSpdLmt_Per1_AstVehSpdLimit_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_VehSpdLmt_Per1_AstVehSpdLimit_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_VehSpdLmt_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_VehSpdLmt_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_VehSpdLmt_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_VehSpdLmt.h` `fixmath.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_VehSpdLmt_Cfg.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h` `Rte.h` `Rte_Ap_VehSpdLmt.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [VehSpdLmt — VehSpdLmt_MDD](./VehSpdLmt-VehSpdLmt_MDD/) | `VehSpdLmt/doc/VehSpdLmt_MDD.docx` |

*Repository path: `VehSpdLmt/`* 
