---
title: "ePWM"
description: "ePWM: purpose, files, API and documents (MCAL & MCU Drivers)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house ePWM/NHet driver incl. generated NHET programs.*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> /0 /1 /2 /3 /4/5 /6 /7 /8 /9 /6 /10 /11 /12 /13 /14 /15 /8 /12 /9 /15 /16 /16 /16 /17 /18 /19 /17 /20 /21 /22

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_ePWM2.c`, `Cd_Nhet1.c`, `Nhet.c`, `Nhet2_ePWM_Prog.c`, `Nhet2_ePWM_Prog.het`, `Nhet_SENT_Prog.c`, `Nhet_SENT_Prog.het`, `ePWM.c` |
| `include/` | `Nhet.h`, `Nhet2_ePWM_Prog.h`, `Nhet_SENT_Prog.h`, `ePWM.h`, `std_nhet.h` |
| AUTOSAR model | 5 `.arxml` file(s), e.g. `Ap_ePWM2.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (10 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_ePWM2_Per1_CtrldDmpStsCmp_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_ePWM2_Per1_DiagStsCtrldDisRmpPres_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_ePWM2_Per1_DiagStsNonRecRmpToZeroFltPres_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_ePWM2_Per1_RampDwnStatusComplete_Cnt_lgc` | RTE-generated symbol |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_IWrite_Nhet1_Per2_DigHwTrqT1_HwNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_Nhet1_Per2_DigHwTrqT1_HwNm_f32` | RTE-generated symbol |
| `Rte_IWrite_Nhet1_Per2_DigHwTrqT2_HwNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_Nhet1_Per2_DigHwTrqT2_HwNm_f32` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`CalConstants.h` `GlobalMacro.h` `MemMap.h` `Nhet.h` `Nhet2_ePWM_Prog.h` `Nhet_SENT_Prog.h` `Rte_Ap_ePWM2.h` `Rte_Cd_Nhet1.h` `Std_Types.h` `ePWM_Cfg.h` `ePwm.h` `epwm_regs.h` `htu_regs.h` `n2het_regs.h` `std_nhet.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_ePWM2` `Rte.h` `Rte_Ap_ePWM2.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CDD_Data.h` `CalConstants.h` `Cd_Nhet1` `Rte.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [ePWM — CD_NHET_1_MDD](./ePWM-CD_NHET_1_MDD/) | `ePWM/doc/CD_NHET_1_MDD.docx` |
| [ePWM — NHetRegisters](./ePWM-NHetRegisters/) | `ePWM/doc/NHetRegisters.pdf` |
| [ePWM — Nhet_1_MDD](./ePWM-Nhet_1_MDD/) | `ePWM/doc/Nhet_1_MDD.docx` |
| [ePWM — RegisterReference_EPWM](./ePWM-RegisterReference_EPWM/) | `ePWM/doc/RegisterReference_EPWM.pdf` |
| [ePWM — ePWM_1_MDD](./ePWM-ePWM_1_MDD/) | `ePWM/doc/ePWM_1_MDD.docx` |
| [ePWM — ePWM_2_MDD](./ePWM-ePWM_2_MDD/) | `ePWM/doc/ePWM_2_MDD.docx` |
| [ePWM — ePWM_Integration_Manual](./ePWM-ePWM_Integration_Manual/) | `ePWM/doc/ePWM_Integration_Manual.docx` |

*Repository path: `ePWM/`* 
