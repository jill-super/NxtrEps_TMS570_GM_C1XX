---
title: "TrqOsc"
description: "TrqOsc: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_TrqOsc).*
## Purpose and responsibility
Software area `TrqOsc` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_TrqOsc.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_TrqOsc.arxml` |
| Generation templates | `Ap_TrqOsc_Cfg.arxml.tt`, `Ap_TrqOsc_Cfg.h.tt`, `Ap_TrqOsc_Generate.bat`, `Ap_TrqOsc_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (9 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_TrqOsc_Per1_TrqOscAmp_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_TrqOsc_Per1_TrqOscEnable_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TrqOsc_Per1_TrqOscFreq_Hz_f32` | RTE-generated symbol |
| `Rte_IWrite_TrqOsc_Per1_TrqOscCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_TrqOsc_Per1_TrqOscCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_TrqOsc_Per1_TrqOscDCExceeded_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_TrqOsc_Per1_TrqOscDCExceeded_Cnt_lgc` | RTE-generated symbol |
| `Rte_Call_TrqOsc_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_TrqOsc_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_TrqOsc_Cfg.h` `CalConstants.h` `MemMap.h` `Rte_Ap_TrqOsc.h` `filters.h` `fixmath.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_TrqOsc` `Ap_TrqOsc_Cfg.h` `Rte.h` `Rte_Ap_TrqOsc.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [TrqOsc — Torque_Oscillation_Function_CM_MDD](./TrqOsc-Torque_Oscillation_Function_CM_MDD/) | `TrqOsc/doc/Torque_Oscillation_Function_CM_MDD.doc` |
| [TrqOsc — TrqOsc_Integration_Manual](./TrqOsc-TrqOsc_Integration_Manual/) | `TrqOsc/doc/TrqOsc_Integration_Manual.docx` |

*Repository path: `TrqOsc/`* 
