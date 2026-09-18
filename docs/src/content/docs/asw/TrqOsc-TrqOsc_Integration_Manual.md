---
title: "TrqOsc — TrqOsc_Integration_Manual"
description: "Converted .docx document from TrqOsc/doc."
---

> **Converted document.** Source: `TrqOsc/doc/TrqOsc_Integration_Manual.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

# Integration Manual – TrqOsc

Table of Contents

## Dependencies

### SWCs

| Module | Required Feature |
| --- | --- |
| <None> |  |

Note : Referencing the external components should be avoided in most cases. Only in unavoidable circumstance external components should be refered. Developer should track the references.

### Global Functions (Non RTE) to be provided to Integration Project

< None>

## Configuration

### Build Time Config

| Modules | Notes |  |
| --- | --- | --- |
| None |  |  |

### Configuration Files to be provided by Integration Project

Ap_TrqOsc_Cfg.h for checkpoint enables

#### Da Vinci Parameter Configuration Changes

| Parameter | Notes | SWC |
| --- | --- | --- |
| TrqOscGeneral/TrqOscCPEnable | To enable checkpoints | TrqOsc |

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

1. TrqOscEnable_lgc from CF-09 (GM Overlay State Handler)
2. TrqOscAmp_MtrNm CF-09 (GM Overlay State Handler)
3. TrqOscFreq_Hz CF-09 (GM Overlay State Handler)
### Required Global Data Outputs

4. TrqOscDCExceeded_Cnt_lgc
5. TrqOscCmd_MtrNm_f32
### Specific Include Path present

No

## Runnable Scheduling

This section specifies the required runnable scheduling.

| Init | Scheduling Requirements | Trigger |
| --- | --- | --- |
| TrqOsc_Init | None | RTE/Init |

| Runnable | Scheduling Requirements | Trigger |
| --- | --- | --- |
| TrqOsc_Per1() | None | RTE(2ms) |

**.**

## Memory Mapping

### Mapping

| Memory Section | Contents | Notes |
| --- | --- | --- |
| TRQOSC_START_SEC_VAR_CLEARED_BOOLEAN |  |  |
| TRQOSC_START_SEC_VAR_CLEARED_32 |  |  |
| TRQOSC_START_SEC_VAR_CLEARED_UNSPECIFIED |  |  |
| RTE_START_SEC_AP_TRQOSC_APPL_CODE |  |  |

* Each …START_SEC… constant is terminated by a …STOP_SEC… constant as specified in the AUTOSAR Memory Mapping requirements.

### Usage

| Feature | RAM | ROM |
| --- | --- | --- |
| None |  |  |

Table 1: ARM Cortex R4 Memory Usage

### Non  RTE NvM Blocks

| Block Name |
| --- |
| None |

Note : Size of the NVM block if configured in developer

### RTE NvM Blocks

| Block Name |
| --- |
| None |

Note : Size of the NVM block if configured in developer

## Compiler Settings

### Preprocessor MACRO

None

### Optimization Settings

None

## Revision Control Log

| **Rev #** | **Change Description** | **Date ** | **Author** |
| --- | --- | --- | --- |
| 1 | Initial version | 02-Apr-2014 | gz7pm0 |
