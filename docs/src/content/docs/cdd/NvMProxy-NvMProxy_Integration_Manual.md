---
title: "NvMProxy — NvMProxy_Integration_Manual"
description: "Converted .docx document from NvMProxy/doc."
---

> **Converted document.** Source: `NvMProxy/doc/NvMProxy_Integration_Manual.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

# Integration Manual – NvM Proxy

Table of Contents

## Dependencies

### SWCs

| Module | Required Feature |
| --- | --- |
| NvM | NvM_WriteBlock() |

### Global Functions(Non RTE) to be provided to Integration Project

NvMProxy_Init

NvMProxy_MainFunction

NvMProxy_WriteBlock

NvMProxy_WriteAll

NvMProxy_GetErrorStatus

NvMProxy_SetRamBlockStatus

## Configuration

### Build Time Config

| Modules | Notes |  |
| --- | --- | --- |
| None |  |  |

### Configuration Files to be provided by Integration Project

#### Da Vinci Parameter Configuration Changes

| Parameter | Notes | SWC |
| --- | --- | --- |
| *NvMProxyConfigSet**/**NvMProxyBlock**/*NvmRamBlockDataAddressSecure | The symbol name of the secured buffer location for the block data | NvMProxy |
| *NvMProxyConfigSet**/**NvMProxyBlock**/*NvMBlockDescriptorRef | Reference to the NvMBlockDescriptor container that defines the NvM block linked to this proxy configuration. | NvMProxy |

#### DaVinci Interrupt Configuration Changes

| ISR Name | VIM # | Priority Dependency | Notes |
| --- | --- | --- | --- |
| N/A |  |  |  |

#### Manual Configuration Changes

| Constant | Notes | SWC |
| --- | --- | --- |
| NVMPROXY_EXCLUSIVE_AREA_0 | This exclusive are covers the areas of execution within the component that are operating on the request buffer.  The buffer is operated on by the MainFunction and the WriteBlock functions.  An appropriate level of protection must be employed to maintain exclusive usage of the buffer data. | SchM |

## Integration

The following import steps must be completed :

1. Place CBD project structure to appropriate integration folder
2. Execute the “Integrate.bat” script from the Tools directory of this component to perform the necessary integration steps:
  1. The script creates the required directories in the integration project, “Generators/Artt/NvMProxy” and “Generators/Components/_Schemes/NvMProxy/bswmd”
  2. The script then copies the required files from the CBD generate directory into the new directories.
3. If this is the first time integration, then perform the Davinci Configurator 3rd party component integration procedure.
4. Configure NvM proxy component per program needs
5. Generate NvM proxy and import generated Cd_NvMProxy_swc.arxml into davinci developer and map all NvM service needs on the blocks needing proxies to the NvM Proxy service component (instead of the NvM service component)
### Required Global Data Inputs

N/A

### Required Global Data Outputs

N/A

### Specific Include Path present

Yes

## Runnable Scheduling

This section specifies the required runnable scheduling.

| Init | Scheduling Requirements | Trigger |
| --- | --- | --- |
| NvMProxy_Init() | Must be executed after NvM driver has initialized the unsecured block data to be forwarded to the secured memory by this component. | Init |

| Runnable | Scheduling Requirements | Trigger |
| --- | --- | --- |
| NvMProxy_MainFunction() | Run prior to NvM_MainFunction for minimal request processing latency | Same as NvM_MainFunction |

**.**

## Memory Mapping

### Mapping

| Memory Section | Contents | Notes |
| --- | --- | --- |
| NVMPROXY_START_SEC_VAR_NOINIT_8 |  | Typically allocated to application in which NvM driver resides. |
| NVMPROXY_START_SEC_VAR_CLEARED_16 |  | Must be allocated  into Global Shared memory |
| NVMPROXY_START_SEC_VAR_CLEARED_UNSPECIFIED |  | Must be allocated  into Global Shared memory |
| NVMPROXY_START_SEC_CODE |  |  |
| NVMPROXY_START_SEC_CONST_UNSPECIFIED |  |  |

* Each …START_SEC… constant is terminated by a …STOP_SEC… constant as specified in the AUTOSAR Memory Mapping requirements.

### Usage

| Feature | RAM | ROM |
| --- | --- | --- |

Table 1: ARM Cortex R4 Memory Usage

### Non  RTE NvM Blocks

| Block Name |
| --- |
| <NVM block used Non RTE functions > |

Note : Size of the NVM block if configured in developer

### RTE NvM Blocks

| Block Name |
| --- |
| <NVM block used in RTE functions > |

Note : Size of the NVM block if configured in developer

## Compiler Settings

### Preprocessor MACRO

<Define all the preprocessor Macros needed and conditions when needed>.

### Optimization Settings

<Define Optimization levels that are needed and conditions when needed>.

## Revision Control Log

| **Rev #** | **Change Description** | **Date ** | **Author** |
| --- | --- | --- | --- |
| 1 | Initial version |  | JJW |
| 2 | Updates per generation definition | 10/18/12 | JJW |
| 3 | Updates for CRC and Redundant checking feature | 12/02/13 | LWW |
