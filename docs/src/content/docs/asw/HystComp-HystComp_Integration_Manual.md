---
title: "HystComp — HystComp_Integration_Manual"
description: "Converted .docx document from HystComp/doc."
---

> **Converted document.** Source: `HystComp/doc/HystComp_Integration_Manual.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

# Integration Manual -- HystComp

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

The HystComp module parameter description file and generator templates are located in the “generate” folder.  The generation scheme at this time relies on the ARTT generation framework developed by BMW.  Following are the recommended steps to integrate the provided generation templates and parameter description with Davinci Configurator:

1. Copy the “Artt/artt” framework folder into the “Generators” directory (if not already present)
2. Execute the “Integrate.bat” script from the Tools directory of this component to perform the necessary integration steps:
  1. The script creates the required directories in the integration project, “Generators/Artt/HystComp” and “Generators/Components/_Schemes/HystComp/bswmd”
  2. The script then copies the required files from the CBD generate directory into the new directories.
3. If this is the first time integration, then perform the Davinci Configurator 3rd party component integration procedure.
| Constant | Notes | SWC |
| --- | --- | --- |
| HystCompGeneral | General module configuration.  See HystComp technical reference for details. | HystComp |

### Rte Config

The SWC description included with this component in the “autosar” folder describes only the static portion of the SWC.  A partial SWC description describing the configurable part of the component interface is generated into the Ap_HystComp _Cfg.arxml file.  This description must be imported into the Rte configuration tool (Developer) using the “Merge Object” option to merge the static SWC description with the generated partial SWC description file.

## Runnable Scheduling

This section specifies the required runnable scheduling.

| Runnable | Scheduling Requirements | Privileged Mode | Trigger |
| --- | --- | --- | --- |
| HystComp_Per1() | Scheduled per integration project requirements | Not Required | 2ms |

## Memory Mapping

### Mapping

| Constant | Notes |
| --- | --- |
| HYSTCOMP_START_SEC_VAR_CLEARED_UNSPECIFIED |  |

* Each …START_SEC… constant is terminated by a …STOP_SEC… constant as specified in the AUTOSAR Memory Mapping requirements.

### Usage

| Feature | RAM | ROM |
| --- | --- | --- |
| Full SWC |  |  |

Table 1: ARM Cortex R4 Memory UsageRevision Control Log

| **Item #** | **Rev #** | **Change Description** | **Date ** | **Author Initials** |
| --- | --- | --- | --- | --- |
| 1 | 1 | Initial version | 26-Apr-13 | Jared |
