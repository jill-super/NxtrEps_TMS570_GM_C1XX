---
title: "MtrTempEst — Motor_Temperature_Estimation_Integration_Manual"
description: "Converted .docx document from MtrTempEst/doc."
---

> **Converted document.** Source: `MtrTempEst/doc/Motor_Temperature_Estimation_Integration_Manual.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

# Integration Manual – TempEstimation

Table of Contents

## Dependencies

### SWCs

| Module | Required Feature |
| --- | --- |
| None |  |

### Configuration Files to be provided by Integration Project

None

### Functions to be provided to Integration Project

None

## Configuration

### Build Time Config

| Modules | Notes |  |
| --- | --- | --- |
| None |  |  |

### Generator Config

| Constant | Notes | SWC |
| --- | --- | --- |
| None |  |  |

## Integration

### Global Data

None

### Component Conflicts

None

### Include Path

None.

### Configurator Changes

None

## Runnable Scheduling

This section specifies the required runnable scheduling.

| Runnable | Scheduling Requirements | Trigger |
| --- | --- | --- |
| MtrTempEst_Per1 | None | RTE (100ms) |

*Note:

Proper Initialization of input signals should occur before running each function for the first time.  (MtrTempEst _Init1).

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

Table 1: ARM Cortex R4 Memory Usage

## Revision Control Log

| **Rev #** | **Change Description** | **Date ** | **Author** |
| --- | --- | --- | --- |
| 1 | Initial version | 25-Mar-13 | Selva |
