---
title: "Metrics — Metrics_Integration_Manual"
description: "Converted .docx document from Metrics/doc."
---

> **Converted document.** Source: `Metrics/doc/Metrics_Integration_Manual.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

# Integration Manual --

## Dependencies

| Module | Required Feature |
| --- | --- |
| Rte | Rte_Task_Dispatch() hooks |
| Dio | Dio_WriteChannel() |
| NxtrLib | DtrmnElapsedTime_uS_u32() |
| Os | osdNumberOfAllTasks constant value |

## Configuration

### Build Time Config

| Constant | Notes | SWC |
| --- | --- | --- |
| ENABLE_CPUUSE_DIO | If defined then CPU usage is output via a DIO where the DIO is high while the CPU is not in the background task. | Metrics |
| RTE_VFB_TRACE=1 | Enable Rte’s VFB trace functionality to support Rte_Task_Dispatch() hooks | Rte |
| Rte_Task_Dispatch | Enable Rte’s Rte_Task_Dispatch() hooks | Rte |

### Generator Config

| Constant | Notes | SWC |
| --- | --- | --- |
| Dio Channel Name: “Metrics” | Required when ENABLE_CPUUSE_DIO is defined | Dio |

## Memory Mapping

### Mapping

| Constant | Notes |
| --- | --- |
| METRICS_START_SEC_VAR_CLEARED_UNSPECIFIED | Writable across all applications |

* Each …START_SEC… constant is terminated by a …STOP_SEC… constant as specified in the AUTOSAR Memory Mapping requirements.

### Usage

| Feature | RAM | ROM |
| --- | --- | --- |
| Software task time stamping of task execution |  |  |
| Stack usage monitoring |  |  |

Table : ARM Cortex R4 Memory UsageRevision Control Log

| **Item #** | **Rev #** | **Change Description** | **Date ** | **Author Initials** |
| --- | --- | --- | --- | --- |
| 1 |  |  |  |  |
