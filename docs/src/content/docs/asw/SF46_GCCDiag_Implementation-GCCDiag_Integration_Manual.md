---
title: "SF46_GCCDiag_Implementation — GCCDiag_Integration_Manual"
description: "Converted .docx document from SF46_GCCDiag_Implementation/doc."
---

> **Converted document.** Source: `SF46_GCCDiag_Implementation/doc/GCCDiag_Integration_Manual.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

# Integration Manual - GCCDiag

Table of Contents

## Dependencies

### SWCs

| Module | Required Feature |
| --- | --- |
| <None> |  |

Note : Referencing the external components should be avoided in most cases. Only in unavoidable circumstance external components should be refered. Developer should track the references.

### Global Functions(Non RTE) to be provided to Integration Project

< None>

## Configuration

### Build Time Config

| Modules | Notes |  |
| --- | --- | --- |
| BC_GCCDIAG_FAULTINJECTIONPOINT | Fault Injection Point |  |

### Configuration Files to be provided by Integration Project

#### Da Vinci Parameter Configuration Changes

| Parameter | Notes | SWC |
| --- | --- | --- |
| <None> |  |  |

#### DaVinci Interrupt Configuration Changes

| ISR Name | VIM # | Priority Dependency | Notes |
| --- | --- | --- | --- |
| <None> |  |  |  |

#### Manual Configuration Changes

| Constant | Notes | SWC |
| --- | --- | --- |
| <None> |  |  |

## Integration

### Required Global Data Inputs

HwTorque_HwNm_f32

DftGrossCCDiag_Cnt_lgc

MRFMtrTrqCmdScl_MtrNm_f32

VehicleSpeed_Kph_f32

### Required Global Data Outputs

N/A

### Specific Include Path present

No

## Runnable Scheduling

This section specifies the required runnable scheduling.

| Init | Scheduling Requirements | Trigger |
| --- | --- | --- |
| GCCDiag_Init1 () | None | Init |

| Runnable | Scheduling Requirements | Trigger |
| --- | --- | --- |
| GCCDiag_Per1() | None | 2 ms |

**.**

## Memory Mapping

### Mapping

| Memory Section | Contents | Notes |
| --- | --- | --- |
| GCCDIAG_START_SEC_VAR_CLEARED_16 |  |  |
| GCCDIAG_START_SEC_VAR_CLEARED_UNSPECIFIED |  |  |

* Each …START_SEC… constant is terminated by a …STOP_SEC… constant as specified in the AUTOSAR Memory Mapping requirements.

### Usage

| Feature | RAM | ROM |
| --- | --- | --- |
| <Memmap usuage info> |  |  |

Table 1: ARM Cortex R4 Memory Usage

### Non  RTE NvM Blocks

| Block Name |
| --- |
| <None > |

Note : Size of the NVM block if configured in developer

### RTE NvM Blocks

| Block Name |
| --- |
| <None> |

Note : Size of the NVM block if configured in developer

## Compiler Settings

### Preprocessor MACRO

<Define all the preprocessor Macros needed and conditions when needed>.

### Optimization Settings

<Define Optimization levels that are needed and conditions when needed>.

## Revision Control Log

| **Rev #** | **Change Description** | **Date ** | **Author** |
| --- | --- | --- | --- |
| 1 | Initial version | 13-Aug-14 | VS |
