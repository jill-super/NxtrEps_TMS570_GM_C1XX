---
title: "NxtrLib — NxtrLib_Systemtime Integration_Manual"
description: "Converted .docx document from NxtrLib/doc."
---

> **Converted document.** Source: `NxtrLib/doc/NxtrLib_Systemtime Integration_Manual.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

# Integration Manual – NxtrLib_SystemTime

## Dependencies

| Module | Required Feature |
| --- | --- |

## Configuration

### Build Time Config

| Constant | Notes | SWC |
| --- | --- | --- |

### Generator Config

#### System

| Constant | Notes | SWC |
| --- | --- | --- |

## Integration

The following import steps must be completed:

1. Place CBD project structure to appropriate integration folder
2. Copy SystemTime_Cfg.h.tt into the Header folder and remove the .tt extension.
3. Configure the constant D_TickRate_Cnt_u32 to the appropriate Os system tick time.
## Runnable Scheduling

This section specifies the required runnable scheduling.

| Runnable | Scheduling Requirements | Trigger |
| --- | --- | --- |

## Memory Mapping

### Mapping

| Constant | Notes |
| --- | --- |

* Each …START_SEC… constant is terminated by a …STOP_SEC… constant as specified in the AUTOSAR Memory Mapping requirements.

### Usage

| Feature | RAM | ROM |
| --- | --- | --- |
| Full driver |  |  |

Table 1: ARM Cortex R4 Memory Usage

## Revision Control Log

| **Item #** | **Rev #** | **Change Description** | **Date ** | **Author Initials** |
| --- | --- | --- | --- | --- |
| 1 |  | Initial version | 26Jul13 | SAH |
