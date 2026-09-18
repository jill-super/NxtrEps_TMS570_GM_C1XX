---
title: "ComplErr — ComplErr_Integration_Manual"
description: "Converted .docx document from ComplErr/doc."
---

> **Converted document.** Source: `ComplErr/doc/ComplErr_Integration_Manual.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

## Integration Manual –ComplErr

Table of Contents

## Dependencies

### SWCs

| Module | Required Feature |
| --- | --- |
| None |  |

Note: Referencing the external components should be avoided in most cases. Only in unavoidable circumstance external components should be referred. Developer should track the references.

### Global Functions (Non RTE) to be provided to Integration Project

#### ComplErr_Per1()

## Configuration

### Build Time Config

| Modules | Notes |  |
| --- | --- | --- |
| None |  |  |

### Configuration Files to be provided by Integration Project

<Configuration file that will be generated from this components that will require Da Vinci Config generation or manual generation. Describe each parameter >

#### Da Vinci Parameter Configuration Changes

| Parameter | Notes | SWC |
| --- | --- | --- |
| None |  |  |

#### DaVinci Interrupt Configuration Changes

| ISR Name | VIM # | Priority Dependency | Notes |
| --- | --- | --- | --- |
| None |  |  |  |

#### Manual Configuration Changes

| Constant | Notes | SWC |
| --- | --- | --- |
| None |  |  |

## Integration

### Required Global Data Inputs

None

### Required Global Data Outputs

None

### Specific Include Path present

None

## Runnable Scheduling

This section specifies the required runnable scheduling.

| Runnable | Scheduling Requirements | Trigger |
| --- | --- | --- |
| ComplErr_Per1 | None | RTE(2ms) |

## Memory Mapping

### Mapping

| Memory Section | Contents | Notes |
| --- | --- | --- |
| RTE_START_SEC_AP_COMPLERR_APPL_CODE |  |  |

* Each …START_SEC… constant is terminated by a …STOP_SEC… constant as specified in the AUTOSAR Memory Mapping requirements.

### Usage

| Feature | RAM | ROM |
| --- | --- | --- |
| N/A |  |  |

Table 1: ARM Cortex R4 Memory Usage

### Non  RTE NvM Blocks

| Block Name |
| --- |
| N/A |

Note : Size of the NVM block if configured in developer

### RTE NvM Blocks

| Block Name |
| --- |
| N/A |

Note : Size of the NVM block if configured in developer

## Compiler Settings

### Preprocessor MACRO

None

### Optimization Settings

None

## Revision Control Log

| **Rev #** | **Change Description** | **Date ** | **Author** |
| --- | --- | --- | --- |
| 1 | Initial version | 08/22/13 | SP |
