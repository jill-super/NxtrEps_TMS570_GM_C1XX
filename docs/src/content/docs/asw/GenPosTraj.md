---
title: "GenPosTraj"
description: "GenPosTraj: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_GenPosTraj).*
## Purpose and responsibility
Software area `GenPosTraj` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_GenPosTraj.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_GenPosTraj.arxml` |
| Generation templates | `Ap_GenPosTraj_Cfg.h.tt`, `Ap_GenPosTraj_Generate.bat`, `Ap_GenPosTraj_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (6 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_GenPosTraj_Per1_HwPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_GenPosTraj_Per1_PosTrajEnable_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_GenPosTraj_Per1_PosTrajHwAngle_HwDeg_f32` | RTE-generated symbol |
| `Rte_IWriteRef_GenPosTraj_Per1_PosTrajHwAngle_HwDeg_f32` | RTE-generated symbol |
| `Rte_Call_GenPosTraj_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_GenPosTraj_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_GenPosTraj_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_GenPosTraj.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_GenPosTraj` `Ap_GenPosTraj_Cfg.h` `Rte.h` `Rte_Ap_GenPosTraj.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [GenPosTraj — GenPosTraj_Integration_Manual](./GenPosTraj-GenPosTraj_Integration_Manual/) | `GenPosTraj/doc/GenPosTraj_Integration_Manual.docx` |
| [GenPosTraj — GenPosTraj_MDD](./GenPosTraj-GenPosTraj_MDD/) | `GenPosTraj/doc/GenPosTraj_MDD.docx` |

*Repository path: `GenPosTraj/`* 
