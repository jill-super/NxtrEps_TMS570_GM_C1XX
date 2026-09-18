---
title: "Fee"
description: "Fee: purpose, files, API and documents (Basic Software (BSW))."
---

:::caution[Third-party — Texas Instruments]
Third-party driver/library provided by Texas Instruments for the TMS570 MCU. Do not modify; follow the vendor documentation linked below.
:::
*Origin: **TI** — Texas Instruments FEE driver for TMS570 Flash EEPROM emulation (third-party).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> Texas Instruments Incorporated                                                      2

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Device_TMS570LS07.c`, `Device_TMS570LS12.c`, `fee.c`, `ti_fee_Info.c`, `ti_fee_cancel.c`, `ti_fee_eraseimmediateblock.c`, `ti_fee_format.c`, `ti_fee_ini.c`, `ti_fee_invalidateblock.c`, `ti_fee_main.c`, `ti_fee_read.c`, `ti_fee_readSync.c` |
| `include/` | `Device_Header.h`, `Device_TMS570LS07.h`, `Device_TMS570LS12.h`, `Device_types.h`, `Fee_Cbk.h`, `fee.h`, `fee_interface.h`, `fee_memmap.h`, `ti_fee.h`, `ti_fee_cfg.h`, `ti_fee_types.h` |
## Public API
| File | Function |
| --- | --- |
| fee.c | `Fee_Write()` |
| fee.c | `Fee_Read()` |
| fee.c | `Fee_GetVersionInfo()` |
| fee.c | `Fee_InternalUpdateGlobalStructure()` |
| ti_fee_Info.c | `TI_Fee_GetVersionInfo()` |
| ti_fee_cancel.c | `TI_Fee_Cancel()` |
| ti_fee_eraseimmediateblock.c | `TI_Fee_EraseImmediateBlock()` |
| ti_fee_format.c | `TI_Fee_Format()` |
| ti_fee_ini.c | `TI_Fee_Init()` |
| ti_fee_invalidateblock.c | `TI_Fee_InvalidateBlock()` |
| ti_fee_read.c | `TI_Fee_Read()` |
| ti_fee_readSync.c | `TI_Fee_ReadSync()` |
| ti_fee_shutdown.c | `TI_Fee_Shutdown()` |
| ti_fee_util.c | `TI_FeeInternal_InvlalidateEraseInitialize()` |
| ti_fee_util.c | `TI_FeeInternal_FindReadyForEraseVirtualSector()` |
| ti_fee_util.c | `TI_FeeInternal_FindInvalidVirtualSector()` |
| ti_fee_util.c | `TI_FeeInternal_CopyInitialize()` |
| ti_fee_util.c | `TI_FeeInternal_ConfigureBlockHeader()` |
| ti_fee_util.c | `TI_FeeInternal_ConfigureVirtualSectorHeader()` |
| ti_fee_util.c | `TI_FeeInternal_ConfigureVirtualSectorHeader()` |
## Usage and dependencies
Selected project headers included by this module:
`Det.h` `Device_TMS570LS07.h` `Device_TMS570LS12.h` `Device_header.h` `Device_types.h` `F021.h` `Fee.h` `Fee_Cbk.h` `Fee_Cfg.h` `MemMap.h` `SchM_Fee.h` `Std_Types.h` `fee_cfg.h` `fee_interface.h` `nvm.h` `ti_fee.h` `ti_fee_cfg.h` `ti_fee_types.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Fee` `Compiler_Cfg.h` `Constants.h` `Det.h` `F021.h` `Helpers.h` `MemIf_Types.h` `MemMap.h` `NvM_Cfg.h` `Registers.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [Fee — AutoSAR FEE Parameter Configuration](./Fee-AutoSAR-FEE-Parameter-Configuration/) | `Fee/doc/AutoSAR FEE Parameter Configuration.pdf` |
| [Fee — AutoSAR FEE User Guide](./Fee-AutoSAR-FEE-User-Guide/) | `Fee/doc/AutoSAR FEE User Guide.pdf` |

*Repository path: `Fee/`* 
