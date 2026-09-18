---
title: "LmtCod"
description: "LmtCod: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_LmtCod).*
## Purpose and responsibility
Software area `LmtCod` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_LmtCod.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_LmtCod.arxml` |
| Generation templates | `Ap_LmtCod_Cfg.arxml.tt`, `Ap_LmtCod_Cfg.h.tt`, `Ap_LmtCod_Generate.bat`, `Ap_LmtCod_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (23 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_LmtCod_Per1_AssistEOTGain_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_LmtCod_Per1_AssistEOTLimit_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_LmtCod_Per1_AssistStallLimit_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_LmtCod_Per1_AssistVehSpdLimit_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_LmtCod_Per1_CCLTrqRamp_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_LmtCod_Per1_OutputRampMult_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_LmtCod_Per1_ThermalLimit_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_LmtCod_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_LmtCod_Per1_EOTGainLtd_Uls_f32` | RTE-generated symbol |
| `Rte_IWriteRef_LmtCod_Per1_EOTGainLtd_Uls_f32` | RTE-generated symbol |
| `Rte_IWrite_LmtCod_Per1_EOTLimitLtd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_LmtCod_Per1_EOTLimitLtd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_LmtCod_Per1_OutputRampMultLtd_Uls_f32` | RTE-generated symbol |
| `Rte_IWriteRef_LmtCod_Per1_OutputRampMultLtd_Uls_f32` | RTE-generated symbol |
| `Rte_IWrite_LmtCod_Per1_StallLimitLtd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_LmtCod_Per1_StallLimitLtd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_LmtCod_Per1_ThermalLimitLtd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_LmtCod_Per1_ThermalLimitLtd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_LmtCod_Per1_VehSpdLimitLtd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_LmtCod_Per1_VehSpdLimitLtd_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_FltInjection_SCom_FltInjection` | RTE-generated symbol |
| `Rte_Call_LmtCod_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_LmtCod_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_LmtCod_Cfg.h` `CalConstants.h` `GlobalMacro.h` `Interpolation.h` `MemMap.h` `Rte_Ap_LmtCod.h` `fixmath.h` `fpmtype.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_LmtCod` `Ap_LmtCod_Cfg.h` `Rte.h` `Rte_Ap_LmtCod.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [LmtCod — Limiter_Conditioning_MDD](./LmtCod-Limiter_Conditioning_MDD/) | `LmtCod/doc/Limiter_Conditioning_MDD.doc` |

*Repository path: `LmtCod/`* 
