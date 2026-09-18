---
title: "FltInjection"
description: "FltInjection: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_FltInjection) used for fault-injection testing.*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> description: "Converted .docx document from FltInjection/doc."

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_FltInjection.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_FltInjection.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (3 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_FltInjection_Per1_MotorVelCRF_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_Call_SystemTime_DtrmnElapsedTime_mS_u32` | RTE-generated symbol |
| `Rte_Call_SystemTime_GetSystemTime_mS_u32` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`GlobalMacro.h` `MemMap.h` `Rte_Ap_FltInjection.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Compiler_Cfg.h` `MemMap.h` `Rte.h` `Rte_Ap_FltInjection.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [FltInjection — Fault_Injection_MDD](./FltInjection-Fault_Injection_MDD/) | `FltInjection/doc/Fault_Injection_MDD.docx` |

*Repository path: `FltInjection/`* 
