---
title: "ComplErr"
description: "ComplErr: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_ComplErr).*
## Purpose and responsibility
Software area `ComplErr` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_ComplErr.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_ComplErr.arxml` |
| Generation templates | `Ap_ComplErr_Cfg.arxml.tt`, `Ap_ComplErr_Cfg.h.tt`, `Ap_ComplErr_Generate.bat`, `Ap_ComplErr_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (5 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_ComplErr_Per1_TorqueCmdCRF_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_ComplErr_Per1_ComplErr_HwDeg_f32` | RTE-generated symbol |
| `Rte_IWriteRef_ComplErr_Per1_ComplErr_HwDeg_f32` | RTE-generated symbol |
| `Rte_Call_ComplErr_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_ComplErr_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_ComplErr_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_ComplErr.h` `fixmath.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_ComplErr` `Ap_ComplErr_Cfg.h` `Rte.h` `Rte_Ap_ComplErr.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [ComplErr — ComplErr_Integration_Manual](./ComplErr-ComplErr_Integration_Manual/) | `ComplErr/doc/ComplErr_Integration_Manual.docx` |
| [ComplErr — Compliance_Error_MDD](./ComplErr-Compliance_Error_MDD/) | `ComplErr/doc/Compliance_Error_MDD.docx` |

*Repository path: `ComplErr/`* 
