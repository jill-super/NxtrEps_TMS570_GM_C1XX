---
title: "Sweep"
description: "Sweep: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-Cs (Ap_Sweep/2).*
## Purpose and responsibility
Software area `Sweep` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_Sweep.c`, `Ap_Sweep2.c` |
| `include/` | `Ap_Sweep.h` |
| AUTOSAR model | 5 `.arxml` file(s), e.g. `Ap_Sweep.arxml` |
| Generation templates | `Ap_Sweep2_Cfg.arxml.tt`, `Ap_Sweep2_Cfg.h.tt`, `Ap_Sweep2_Generate.bat`, `Ap_Sweep2_bswmd.arxml`, `Ap_Sweep_Cfg.arxml.tt`, `Ap_Sweep_Cfg.h.tt` |
## Public API
Top RTE/component symbols referenced in the sources (14 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_Sweep_Per1_InputHwTrq_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_Sweep_Per1_VehSpdValid_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_Sweep_Per1_VehSpd_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_Sweep_Per1_OutputHwTrq_HwNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_Sweep_Per1_OutputHwTrq_HwNm_f32` | RTE-generated symbol |
| `Rte_Call_SystemTime_DtrmnElapsedTime_mS_u16` | RTE-generated symbol |
| `Rte_Call_SystemTime_GetSystemTime_mS_u32` | RTE-generated symbol |
| `Rte_Call_Sweep_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_Sweep_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IRead_Sweep2_Per1_InputMtrTrq_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_Sweep2_Per1_OutputMtrTrq_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_Sweep2_Per1_OutputMtrTrq_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_Sweep2_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_Sweep2_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_Sweep.h` `Ap_Sweep2_Cfg.h` `Ap_Sweep_Cfg.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_Sweep.h` `Rte_Ap_Sweep2.h` `fixmath.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_Sweep` `Ap_Sweep_Cfg.h` `Rte.h` `Rte_Ap_Sweep.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `Ap_Sweep2` `Ap_Sweep2_Cfg.h` `Rte.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [Sweep — Sweep1_MDD](./Sweep-Sweep1_MDD/) | `Sweep/doc/Sweep1_MDD.docx` |
| [Sweep — Sweep2_MDD](./Sweep-Sweep2_MDD/) | `Sweep/doc/Sweep2_MDD.docx` |

*Repository path: `Sweep/`* 
