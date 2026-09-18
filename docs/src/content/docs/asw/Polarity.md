---
title: "Polarity"
description: "Polarity: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_Polarity).*
## Purpose and responsibility
Software area `Polarity` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_Polarity.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_Polarity.arxml` |
| Generation templates | `Ap_Polarity_Cfg.arxml.tt`, `Ap_Polarity_Cfg.h.tt`, `Ap_Polarity_Generate.bat`, `Ap_Polarity_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (32 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Pim_Polarity_Cnt_Str` | RTE-generated symbol |
| `Rte_IWrite_Polarity_Init1_AssistAssyPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IWriteRef_Polarity_Init1_AssistAssyPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IWrite_Polarity_Init1_HwPosPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IWriteRef_Polarity_Init1_HwPosPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IWrite_Polarity_Init1_HwTrqPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IWriteRef_Polarity_Init1_HwTrqPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IWrite_Polarity_Init1_MtrElecMechPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IWriteRef_Polarity_Init1_MtrElecMechPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IWrite_Polarity_Init1_MtrPosPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IWriteRef_Polarity_Init1_MtrPosPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IWrite_Polarity_Init1_MtrVelPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IWriteRef_Polarity_Init1_MtrVelPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IWrite_Polarity_Init1_SysC_MtrElecMechPolarity_Cnt_s32` | RTE-generated symbol |
| `Rte_IWriteRef_Polarity_Init1_SysC_MtrElecMechPolarity_Cnt_s32` | RTE-generated symbol |
| `Rte_IRead_Polarity_Per1_DiagAssistAssyPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IRead_Polarity_Per1_DiagHwPosPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IRead_Polarity_Per1_DiagHwTrqPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IRead_Polarity_Per1_DiagMtrElecMechPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IRead_Polarity_Per1_DiagMtrPosPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IRead_Polarity_Per1_DiagMtrVelPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_Polarity_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_Polarity_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_Polarity_Cfg.h` `MemMap.h` `Os.h` `Rte_Ap_Polarity.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_Polarity` `Ap_Polarity_Cfg.h` `Os.h` `Rte.h` `Rte_Ap_Polarity.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [Polarity — Polarity_MDD](./Polarity-Polarity_MDD/) | `Polarity/doc/Polarity_MDD.docx` |

*Repository path: `Polarity/`* 
