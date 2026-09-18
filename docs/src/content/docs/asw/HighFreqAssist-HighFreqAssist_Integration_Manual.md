---
title: "HighFreqAssist — HighFreqAssist_Integration_Manual"
description: "Converted .docx document from HighFreqAssist/doc."
---

> **Converted document.** Source: `HighFreqAssist/doc/HighFreqAssist_Integration_Manual.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

# Integration Manual -- HighFreqAssist

## Dependencies

| Module | Required Feature |
| --- | --- |
| Rte | Port and runnable mapping. |
| WdgM | CheckpointReached() API |

## Configuration

### Build Time Config

| Constant | Notes | SWC |
| --- | --- | --- |
| None |  |  |

### Generator Config

The HighFreqAssist module parameter description file and generator templates are located in the “generate” folder.  The generation scheme at this time relies on the ARTT generation framework developed by BMW.  Following are the recommended steps to integrate the provided generation templates and parameter description with Davinci Configurator:

1. Copy the “Artt/artt” framework folder into the “Generators” directory (if not already present)
2. Execute the “Integrate.bat” script from the Tools directory of this component to perform the necessary integration steps:
  1. The script creates the required directories in the integration project, “Generators/Artt/HighFreqAssist” and “Generators/Components/_Schemes/HighFreqAssist/bswmd”
  2. The script then copies the required files from the CBD generate directory into the new directories.
3. If this is the first time integration, then perform the Davinci Configurator 3rd party component integration procedure.
| Constant | Notes | SWC |
| --- | --- | --- |
| HighFreqAssistGeneral | General module configuration.  See HighFreqAssist technical reference for details. | HighFreqAssist |

### Rte Config

The SWC description included with this component in the “autosar” folder describes only the static portion of the SWC.  A partial SWC description describing the configurable part of the component interface is generated into the Ap_HighFreqAssist_Cfg.arxml file.  This description must be imported into the Rte configuration tool (Developer) using the “Merge Object” option to merge the static SWC description with the generated partial SWC description file.

## Runnable Scheduling

This section specifies the required runnable scheduling.

| Runnable | Scheduling Requirements | Privileged Mode | Trigger |
| --- | --- | --- | --- |
| _Per1() | Scheduled per integration project requirements | Not Required | 2ms |

## Memory Mapping

### Mapping

| Constant | Notes |
| --- | --- |
| HYSTADD_START_SEC_VAR_CLEARED_UNSPECIFIED |  |
| HIGHFREQASSIST_START_SEC_VAR_CLEARED_32 |  |

* Each …START_SEC… constant is terminated by a …STOP_SEC… constant as specified in the AUTOSAR Memory Mapping requirements.

### Usage

| Feature | RAM | ROM |
| --- | --- | --- |
| Full SWC |  |  |

Table 1: ARM Cortex R4 Memory UsageRevision Control Log

| **Item #** | **Rev #** | **Change Description** | **Date ** | **Author Initials** |
| --- | --- | --- | --- | --- |
| 1 | 1 | Initial version | 2-May-13 | Jared |
