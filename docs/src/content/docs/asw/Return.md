---
title: "Return"
description: "Return: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_Return).*
## Purpose and responsibility
Software area `Return` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_Return.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_Return.arxml` |
| Generation templates | `Ap_Return_Cfg.arxml.tt`, `Ap_Return_Cfg.h.tt`, `Ap_Return_Generate.bat`, `Ap_Return_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (16 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_Return_Per1_AssistMechTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IRead_Return_Per1_DefeatReturnSvc_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_Return_Per1_DiagStsHwPosDis_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_Return_Per1_HandwheelAuthority_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_Return_Per1_HandwheelPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_Return_Per1_HandwheelVel_HwRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_Return_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_Return_Per1_PAReturnSclFct_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_Return_Per1_ReturnDDFactor_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_Return_Per1_ReturnOffset_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_Return_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_Return_Per1_ReturnCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_Return_Per1_ReturnCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_FltInjection_SCom_FltInjection` | RTE-generated symbol |
| `Rte_Call_Return_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_Return_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_Return_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_Return.h` `fixmath.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_Return` `Ap_Return_Cfg.h` `Rte.h` `Rte_Ap_Return.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `Ap_Return_Cfg.h` `CalConstants.h` `Compiler_Cfg.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [Return — Return_MDD](./Return-Return_MDD/) | `Return/doc/Return_MDD.docx` |

*Repository path: `Return/`* 
