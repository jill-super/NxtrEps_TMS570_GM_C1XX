---
title: "PosServo"
description: "PosServo: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_PosServo).*
## Purpose and responsibility
Software area `PosServo` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_PosServo.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_PosServo.arxml` |
| Generation templates | `Ap_PosServo_Cfg.arxml.tt`, `Ap_PosServo_Cfg.h.tt`, `Ap_PosServo_Generate.bat`, `Ap_PosServo_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (14 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_PosServo_Per1_HandwheelPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_PosServo_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_PosServo_Per1_MotorVelCRF_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_PosServo_Per1_PosSrvoEnable_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_PosServo_Per1_PosSrvoHwAngle_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_PosServo_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_PosServo_Per1_PosSrvoCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_PosServo_Per1_PosSrvoCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_PosServo_Per1_PosSrvoReturnSclFct_Uls_f32` | RTE-generated symbol |
| `Rte_IWriteRef_PosServo_Per1_PosSrvoReturnSclFct_Uls_f32` | RTE-generated symbol |
| `Rte_IWrite_PosServo_Per1_PosSrvoSmoothEnable_Uls_f32` | RTE-generated symbol |
| `Rte_IWriteRef_PosServo_Per1_PosSrvoSmoothEnable_Uls_f32` | RTE-generated symbol |
| `Rte_Call_PosServo_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_PosServo_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_PosServo_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_PosServo.h` `SystemTime.h` `filters.h` `fixmath.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_PosServo` `Ap_PosServo_Cfg.h` `Rte.h` `Rte_Ap_PosServo.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [PosServo — PosServo_MDD](./PosServo-PosServo_MDD/) | `PosServo/doc/PosServo_MDD.docx` |

*Repository path: `PosServo/`* 
