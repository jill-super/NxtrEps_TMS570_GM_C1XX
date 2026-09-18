---
title: "MtrCtrl_CM — MtrCntrl_Integration_Manual"
description: "Converted .docx document from MtrCtrl_CM/doc."
---

> **Converted document.** Source: `MtrCtrl_CM/doc/MtrCntrl_Integration_Manual.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

# Integration Manual --

Table of Contents

## Dependencies

### SWCs

| Module | Required Feature |
| --- | --- |

### Configuration Files to be provided by Integration Project

MtrCtrl_Cfg.h

### Functions to be provided to Integration Project

PICurrCntrl_Per1()

TrqCogCancRefPer1()

## Configuration

### Build Time Config

| Modules | Notes |  |
| --- | --- | --- |
| PICurrentCntrl | Optimization level greater than 3 |  |

### Generator Config

| Constant | Notes | SWC |
| --- | --- | --- |
| None |  |  |

## Integration

### Global Data

The global symbols mapping done in MtrCtrl_Cfg.h.

### Component Conflicts

None

### Include Path

The “include” directory of this SWC needs to be included in the integration project include search path.

.

### Configurator Changes

None

## Runnable Scheduling

This section specifies the required runnable scheduling.

| Runnable | Scheduling Requirements | Trigger |
| --- | --- | --- |
| TrqCogCancRefPer1() | Must be placed in the motor control ISR, after MtrPos | Cyclic (ISR) |
| PICurrCntrl_Per1() | Must be placed in the motor control ISR after TrqCogCancRefPer1() | Cyclic (ISR) |

| Runnable | Scheduling Requirements | Trigger |
| --- | --- | --- |
| CurrParamComp_Init() |  | RTE (init) |
| TrqCanc_Init | Must be placed after CurrParamComp_Init | RTE (init) |
| QuadDet_Per1 | Must run after TrqReasonable Diagnostics | RTE (2ms) |
| CurrCmd_Per1 | Must run after  QuadDet | RTE (2ms) |
| TrqCanc_Per1 | Must run after CurrCmd_Per1 | RTE (2ms) |
| PICurrCntrl_Per2() | Must be placed after TrqCanc_Per1 | RTE (2ms) |
| CurrParamComp_Per1() | Must be placed after PICurrCntrl_Per2 | RTE (2ms) |
| PeakCurrEst_Per1() | Must be placed after PICurrCntrl_Per2 | RTE (2ms) |

*Note: In motor control ISR include Ap_MtrCtrl.h instead of CDD_Func.h

Proper Initialization of input signals should occur before running each function for the first time.  **(CurrParamComp_Init)****.**

## Memory Mapping

### Mapping

| Memory Section | Contents | Notes |
| --- | --- | --- |
| RTE Memory mapping |  |  |

* Each …START_SEC… constant is terminated by a …STOP_SEC… constant as specified in the AUTOSAR Memory Mapping requirements.

### Usage

| Feature | RAM | ROM |
| --- | --- | --- |
| Full driver |  |  |

### Table 1: ARM Cortex R4 Memory Usage

### RTE NvM Blocks

| Block Name                                                         Size |
| --- |
| Rte_Pim_CogTrqCal                                           512 |
| Rte_Pim_CogTrqRplComp                               9 |

Note : Size of the NVM block is changed.

## Revision Control Log

| **Rev #** | **Change Description** | **Date ** | **Author** |
| --- | --- | --- | --- |
| 1 | Initial version | 25-Mar-13 | Selva |
| 2 | Updated  TrqCanc_Init in RTE Runnables and size of the NVM block CogTrqCal  is changed from 512 to 521 | 21-Oct-13 | Selva |
| 3 | Added new NVM block “Rte_Pim_CogTrqRplComp” | 23-Oct-13 | Selva |
