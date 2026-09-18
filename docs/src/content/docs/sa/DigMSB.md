---
title: "DigMSB"
description: "DigMSB: purpose, files, API and documents (Sensor / Actuator Abstraction)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Sa_DigMSB).*
## Purpose and responsibility
Software area `DigMSB` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Sa_DigMSB.c` |
| `include/` | `Sa_DigMSB.h` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Sa_DigMSB.arxml` |
| Generation templates | `Sa_DigMSB_Cfg.arxml.tt`, `Sa_DigMSB_Cfg.h.tt`, `Sa_DigMSB_Generate.bat`, `Sa_DigMSB_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (35 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Pim_DigMSBEOLData` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_IRead_DigMSB_Per2_AssistAssemblyPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IRead_DigMSB_Per2_CorrectedElecMtrPos_Rev_u0p16` | RTE-generated symbol |
| `Rte_IRead_DigMSB_Per2_CumMechMtrPos_Rev_f32` | RTE-generated symbol |
| `Rte_IRead_DigMSB_Per2_Die1RxError_Cnt_u16` | RTE-generated symbol |
| `Rte_IRead_DigMSB_Per2_Die1RxMtrPos_Cnt_u16` | RTE-generated symbol |
| `Rte_IRead_DigMSB_Per2_Die1RxRevCtr_Cnt_u16` | RTE-generated symbol |
| `Rte_IRead_DigMSB_Per2_Die1UnderVoltgFltAccum_Cnt_u16` | RTE-generated symbol |
| `Rte_IRead_DigMSB_Per2_Die2RxError_Cnt_u16` | RTE-generated symbol |
| `Rte_IRead_DigMSB_Per2_Die2RxMtrPos_Cnt_u16` | RTE-generated symbol |
| `Rte_IRead_DigMSB_Per2_Die2RxRevCtr_Cnt_u16` | RTE-generated symbol |
| `Rte_IRead_DigMSB_Per2_MtrPosPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IRead_DigMSB_Per2_RxMtrPosParityAccum_Cnt_u16` | RTE-generated symbol |
| `Rte_IRead_DigMSB_Per2_UncorrMechMtrPos1_Rev_u0p16` | RTE-generated symbol |
| `Rte_IWrite_DigMSB_Per2_AlignedCumMechMtrPosCRF_Deg_f32` | RTE-generated symbol |
| `Rte_IWriteRef_DigMSB_Per2_AlignedCumMechMtrPosCRF_Deg_f32` | RTE-generated symbol |
| `Rte_IWrite_DigMSB_Per2_AlignedCumMechMtrPosMRF_Deg_f32` | RTE-generated symbol |
| `Rte_IWriteRef_DigMSB_Per2_AlignedCumMechMtrPosMRF_Deg_f32` | RTE-generated symbol |
| `Rte_IWrite_DigMSB_Per2_AlignedCumMechMtrPosStatus_Cnt_u08` | RTE-generated symbol |
| `Rte_IWriteRef_DigMSB_Per2_AlignedCumMechMtrPosStatus_Cnt_u08` | RTE-generated symbol |
| `Rte_IWrite_DigMSB_Per2_CumMechMtrPosCRF_Deg_f32` | RTE-generated symbol |
| `Rte_IWriteRef_DigMSB_Per2_CumMechMtrPosCRF_Deg_f32` | RTE-generated symbol |
| `Rte_IWrite_DigMSB_Per2_CumMechMtrPosMRF_Deg_f32` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`CalConstants.h` `DigMSB_Cfg.h` `GlobalMacro.h` `MemMap.h` `Rte_Sa_DigMSB.h` `Sa_DigMSB.h` `Sa_DigMSB_Cfg.h` `SystemTime.h` `fixmath.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [DigMSB — DigMSB_Integration_Manual](./DigMSB-DigMSB_Integration_Manual/) | `DigMSB/doc/DigMSB_Integration_Manual.docx` |
| [DigMSB — DigtalMSB_MDD](./DigMSB-DigtalMSB_MDD/) | `DigMSB/doc/DigtalMSB_MDD.docx` |

*Repository path: `DigMSB/`* 
