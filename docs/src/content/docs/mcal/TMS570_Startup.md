---
title: "TMS570_Startup"
description: "TMS570_Startup: purpose, files, API and documents (MCAL & MCU Drivers)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house startup code, system init and interrupt vectors for TMS570.*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> description: "Converted .docx document from TMS570_Startup/doc."

## Key files
| Area | Files |
| --- | --- |
| `src/` | `AppStartup.c`, `BootStartup.c`, `ResetCause.c`, `fiqintvect.asm`, `prooftestv02.c`, `prooftestv02.het`, `sys_core.asm`, `sys_memory.asm`, `sys_pmu.asm`, `sys_startup.c` |
| `include/` | `ResetCause.h`, `prooftestv02.h`, `sys_core.h`, `sys_memory.h`, `sys_pmu.h` |
## Public API
| File | Function |
| --- | --- |
| AppStartup.c | `adc1ParityCheck()` |
| AppStartup.c | `adc2ParityCheck()` |
| AppStartup.c | `dcan1ParityCheck()` |
| AppStartup.c | `dcan2ParityCheck()` |
| AppStartup.c | `dcan3ParityCheck()` |
| AppStartup.c | `mibspi1ParityCheck()` |
| AppStartup.c | `mibspi3parityCheck()` |
| AppStartup.c | `mibspi5ParityCheck()` |
| AppStartup.c | `nhet1ParityCheck()` |
| AppStartup.c | `nhet2parityCheck()` |
| AppStartup.c | `htu1ParityCheck()` |
| AppStartup.c | `htu2ParityCheck()` |
| AppStartup.c | `vimParityCheck()` |
| AppStartup.c | `dmaParityCheck()` |
| AppStartup.c | `WaitForHtuTransfer()` |
| AppStartup.c | `StartupHTU1Init()` |
| AppStartup.c | `Nhet1HTUMPUCheck()` |
| AppStartup.c | `StartupHTU2Init()` |
| AppStartup.c | `Nhet2HTUMPUCheck()` |
| AppStartup.c | `WaitForDmaTransfer()` |
## Usage and dependencies
Selected project headers included by this module:
`Compiler.h` `MemMap.h` `Platform_Types.h` `ResetCause.h` `Std_Types.h` `adc_regs.h` `appinit_cfg.h` `ccm_regs.h` `dcan_regs.h` `dma_regs.h` `efc_regs.h` `esm_regs.h` `flash_regs.h` `gio_regs.h` `htu_regs.h` `mibspi_regs.h` `n2het_regs.h` `pbist_regs.h` `pcr_regs.h` `prooftestv02.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Compiler_Cfg.h` `MemMap.h` `appinit_cfg.h` `startup_cfg.h` `std_nhet.h` `uDiag.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [TMS570_Startup — TMS570_Startup_BootStartup_MDD](./TMS570_Startup-TMS570_Startup_BootStartup_MDD/) | `TMS570_Startup/doc/TMS570_Startup_BootStartup_MDD.docx` |
| [TMS570_Startup — TMS570_Startup_FiqIntVect_MDD](./TMS570_Startup-TMS570_Startup_FiqIntVect_MDD/) | `TMS570_Startup/doc/TMS570_Startup_FiqIntVect_MDD.docx` |
| [TMS570_Startup — TMS570_Startup_Integration_Manual](./TMS570_Startup-TMS570_Startup_Integration_Manual/) | `TMS570_Startup/doc/TMS570_Startup_Integration_Manual.docx` |
| [TMS570_Startup — TMS570_Startup_SysCore_MDD](./TMS570_Startup-TMS570_Startup_SysCore_MDD/) | `TMS570_Startup/doc/TMS570_Startup_SysCore_MDD.docx` |
| [TMS570_Startup — TMS570_Startup_SysStartup_MDD](./TMS570_Startup-TMS570_Startup_SysStartup_MDD/) | `TMS570_Startup/doc/TMS570_Startup_SysStartup_MDD.docx` |
| [TMS570_Startup — spna106a](./TMS570_Startup-spna106a/) | `TMS570_Startup/doc/spna106a.pdf` |

*Repository path: `TMS570_Startup/`* 
