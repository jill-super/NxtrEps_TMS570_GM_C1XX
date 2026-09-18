---
title: "TqRsDg"
description: "TqRsDg: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_TqRsDg).*
## Purpose and responsibility
Software area `TqRsDg` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_TqRsDg.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_TqRsDg.arxml` |
| Generation templates | `Ap_TqRsDg_Cfg.arxml.tt`, `Ap_TqRsDg_Cfg.h.tt`, `Ap_TqRsDg_Generate.bat`, `Ap_TqRsDg_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (8 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_IRead_TqRsDg_Per1_DervLambdaAlphaDiag_Volt_f32` | RTE-generated symbol |
| `Rte_IRead_TqRsDg_Per1_DervLambdaBetaDiag_Volt_f32` | RTE-generated symbol |
| `Rte_IRead_TqRsDg_Per1_OutputRampMult_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_TqRsDg_Per1_TrqLimitMin_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_TqRsDg_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_TqRsDg_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_TqRsDg_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_TqRsDg.h` `filters.h` `fixmath.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_TqRsDg` `Ap_TqRsDg_Cfg.h` `Rte.h` `Rte_Ap_TqRsDg.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [TqRsDg — TorqueReasonableDiagnostics](./TqRsDg-TorqueReasonableDiagnostics/) | `TqRsDg/doc/TorqueReasonableDiagnostics.docx` |
| [TqRsDg — TrqReasonableness_Integration_Manual](./TqRsDg-TrqReasonableness_Integration_Manual/) | `TqRsDg/doc/TrqReasonableness_Integration_Manual.docx` |

*Repository path: `TqRsDg/`* 
