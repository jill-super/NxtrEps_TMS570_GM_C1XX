---
title: "TMS570_uDiag"
description: "TMS570_uDiag: purpose, files, API and documents (Complex Device Drivers (CDD))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house micro diagnostics CDD (Cd_uDiag) plus FlsTst.*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> description: "Converted .docx document from TMS570_uDiag/doc."

## Key files
| Area | Files |
| --- | --- |
| `src/` | `AbortHandler.c`, `Cd_uDiagCCRM.c`, `Cd_uDiagClockMonitor.c`, `Cd_uDiagECC.c`, `Cd_uDiagESM.c`, `Cd_uDiagFPU.c`, `Cd_uDiagIOMM.c`, `Cd_uDiagLossOfExec.c`, `Cd_uDiagParity.c`, `Cd_uDiagPeriphMPU.c`, `Cd_uDiagResetHandler.c`, `Cd_uDiagStaticRegs.c` |
| `include/` | `Cd_uDiagUtility.h`, `FlsTst.h`, `RednRpdShtdn.h`, `uDiag.h` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Cd_uDiag.arxml` |
| Generation templates | `Cd_uDiag_Cfg.arxml.tt`, `FlsTst_Cfg.c.tt`, `FlsTst_Cfg.h.tt`, `FlsTst_Generate.bat`, `FlsTst_bswmd.arxml`, `uDiag_Cfg.c.tt` |
## Public API
Top RTE/component symbols referenced in the sources (11 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_uDiagECC_Per_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_uDiagECC_Per_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_uDiagLossOfExec_Per2_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_uDiagLossOfExec_Per2_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_uDiagLossOfExec_Per3_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_uDiagLossOfExec_Per3_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_uDiagStaticRegs_Per_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_uDiagStaticRegs_Per_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_uDiagVIM_Per_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_uDiagVIM_Per_CP1_CheckpointReached` | RTE-generated symbol |
<details><summary>Top-level function definitions</summary>
| File | Function |
| --- | --- |
| Cd_uDiagVIM.c | `VIM_Fallback()` |
</details>
## Usage and dependencies
Selected project headers included by this module:
`Ap_DiagMgr.h` `CalConstants.h` `Cd_uDiagUtility.h` `Dma.h` `FlsTst.h` `FlsTst_Cfg.h` `GlobalMacro.h` `Interrupts.h` `MemMap.h` `Nhet.h` `Os.h` `RednRpdShtdn.h` `ResetCause.h` `Rte_Cd_uDiag.h` `Std_Types.h` `WdgM.h` `adc_regs.h` `appinit_cfg.h` `crc_regs.h` `dcan_regs.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_DiagMgr.h` `CalConstants.h` `Compiler_Cfg.h` `Dma.h` `FlsTst_Cfg.h` `Interrupts.h` `MemMap.h` `Nhet.h` `Os.h` `ResetCause.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [TMS570_uDiag — Cd_uDiagFPU_MDD](./TMS570_uDiag-Cd_uDiagFPU_MDD/) | `TMS570_uDiag/doc/Cd_uDiagFPU_MDD.docx` |
| [TMS570_uDiag — Cd_uDiagUtility_MDD](./TMS570_uDiag-Cd_uDiagUtility_MDD/) | `TMS570_uDiag/doc/Cd_uDiagUtility_MDD.docx` |
| [TMS570_uDiag — Cd_uDiag_Integration_Manual](./TMS570_uDiag-Cd_uDiag_Integration_Manual/) | `TMS570_uDiag/doc/Cd_uDiag_Integration_Manual.docx` |
| [TMS570_uDiag — FlsTst_Integration_Manual](./TMS570_uDiag-FlsTst_Integration_Manual/) | `TMS570_uDiag/doc/FlsTst_Integration_Manual.docx` |
| [TMS570_uDiag — FlsTst_MDD](./TMS570_uDiag-FlsTst_MDD/) | `TMS570_uDiag/doc/FlsTst_MDD.docx` |
| [TMS570_uDiag — OsErrCallouts_MDD](./TMS570_uDiag-OsErrCallouts_MDD/) | `TMS570_uDiag/doc/OsErrCallouts_MDD.docx` |

*Repository path: `TMS570_uDiag/`* 
