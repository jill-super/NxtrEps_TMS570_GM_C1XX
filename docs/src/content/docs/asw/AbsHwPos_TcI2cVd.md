---
title: "AbsHwPos_TcI2cVd"
description: "AbsHwPos_TcI2cVd: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_AbsHwPos). DaVinci/RTE artefacts are Vector-generated.*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> title: "AbsHwPos_TcI2cVd — AbsHwPos_TcI2cVd_Integration_Manual"

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_AbsHwPos.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_AbsHwPos.arxml` |
| Generation templates | `Ap_AbsHwPos_Cfg.arxml.tt`, `Ap_AbsHwPos_Cfg.h.tt`, `Ap_AbsHwPos_Generate.bat`, `Ap_AbsHwPos_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (43 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Pim_EOLVehCntrOffset` | RTE-generated symbol |
| `Rte_IRead_AbsHwPos_Init1_ManufMode_Cnt_enum` | RTE-generated symbol |
| `Rte_IWrite_AbsHwPos_Init1_HwPosSource_Cnt_u16` | RTE-generated symbol |
| `Rte_IWriteRef_AbsHwPos_Init1_HwPosSource_Cnt_u16` | RTE-generated symbol |
| `Rte_IWrite_AbsHwPos_Init1_SrlComHwPosStatus_Cnt_u16` | RTE-generated symbol |
| `Rte_IWriteRef_AbsHwPos_Init1_SrlComHwPosStatus_Cnt_u16` | RTE-generated symbol |
| `Rte_IRead_AbsHwPos_Per1_AlignedCumMechMtrPosCRF_Deg_f32` | RTE-generated symbol |
| `Rte_IRead_AbsHwPos_Per1_ComplError_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_AbsHwPos_Per1_CumMechMtrPosCRF_Deg_f32` | RTE-generated symbol |
| `Rte_IWrite_AbsHwPos_Per1_RelHwPos_HwDeg_f32` | RTE-generated symbol |
| `Rte_IWriteRef_AbsHwPos_Per1_RelHwPos_HwDeg_f32` | RTE-generated symbol |
| `Rte_Call_AbsHwPos_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_AbsHwPos_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IRead_AbsHwPos_Per2_DiagStatusHwPosReducedPerf_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_AbsHwPos_Per2_I2CHwAbsPosValid_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_AbsHwPos_Per2_I2CHwAbsPos_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_AbsHwPos_Per2_ManufMode_Cnt_enum` | RTE-generated symbol |
| `Rte_IRead_AbsHwPos_Per2_TurnsCntrValidity_Cnt_u08` | RTE-generated symbol |
| `Rte_IRead_AbsHwPos_Per2_VdAuthority_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_AbsHwPos_Per2_VdHwPos_HwDeg_f32` | RTE-generated symbol |
| `Rte_IWrite_AbsHwPos_Per2_HandwheelAuthority_Uls_f32` | RTE-generated symbol |
| `Rte_IWriteRef_AbsHwPos_Per2_HandwheelAuthority_Uls_f32` | RTE-generated symbol |
| `Rte_IWrite_AbsHwPos_Per2_HandwheelPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_IWriteRef_AbsHwPos_Per2_HandwheelPosition_HwDeg_f32` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_AbsHwPos_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_AbsHwPos.h` `filters.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_AbsHwPos` `Ap_AbsHwPos_Cfg.h` `Rte.h` `Rte_Ap_AbsHwPos.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [AbsHwPos_TcI2cVd — AbsHwPos_TcI2cVd_Integration_Manual](./AbsHwPos_TcI2cVd-AbsHwPos_TcI2cVd_Integration_Manual/) | `AbsHwPos_TcI2cVd/doc/AbsHwPos_TcI2cVd_Integration_Manual.docx` |
| [AbsHwPos_TcI2cVd — Absolute_Handwheel_Position_TcI2cVd_MDD](./AbsHwPos_TcI2cVd-Absolute_Handwheel_Position_TcI2cVd_MDD/) | `AbsHwPos_TcI2cVd/doc/Absolute_Handwheel_Position_TcI2cVd_MDD.docx` |

*Repository path: `AbsHwPos_TcI2cVd/`* 
