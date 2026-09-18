---
title: "DampingFirewall — DampingFirewall_IntegrationManual"
description: "Converted .docx document from DampingFirewall/doc."
---

> **Converted document.** Source: `DampingFirewall/doc/DampingFirewall_IntegrationManual.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

**Integration Manual**

**For**

**Damping**** Firewall**

**VERSION: ****1.****0**

**DATE: ****15****-****JAN****-****2015**

**Prepared By: **

**Spandana Balani**

**Revision History**

| **Rev #** | **Change Description** | **Date ** | **Author** |
| --- | --- | --- | --- |
| 1 | Initial version | 15-Jan-15 | SB |

**Table of Contents**

## Abbrevations And Acronyms

| **Abbreviation** | **Description** |
| --- | --- |
| DFD | Design functional diagram |
| MDD | Module design Document |
|  | <ADD  more to the table if applicable> |

## References

This section lists the title & version of all the documents that are referred for development of this document

| **Sr. No.** | **Title** | **Version** |
| --- | --- | --- |
| 1 | SF35 Damping Firewall | 011 |

## Dependencies

### SWCs

| **Module** | **Required Feature** |
| --- | --- |
| **None** | <Addition of global data, function>*. |

Note : Referencing the external components should be avoided in most cases. Only in unavoidable circumstance external components should be referred. Developer should track the references.

### Global Functions(Non RTE) to be provided to Integration Project

None

## Configuration REQUIREMeNTS

### Build Time Config

| **Modules** | **Notes** |  |
| --- | --- | --- |
| **None** |  |  |

### Configuration Files to be provided by Integration Project

Ap_DampingFirewall_Cfg.h for checkpoint enable

### Da Vinci Parameter Configuration Changes

| **Parameter** | **Notes** | **SWC** |
| --- | --- | --- |
| **Damping****FirewallGeneral**/**Damping****F****irewallCPEnable** | To enable checkpoints | DampingFirewall |

### DaVinci Interrupt Configuration Changes

| **ISR Name** | **VIM #** | **Priority Dependency** | **Notes** |
| --- | --- | --- | --- |
| **None** |  |  |  |

### Manual Configuration Changes

| **Constant** | **Notes** | **SWC** |
| --- | --- | --- |
| **None** |  |  |

## Integration  DATAFLOW REQUIREMENTS

### Required Global Data Inputs

AsstFirewallActive_Uls_f32

DampingCmd_MtrNm_f32

HwTorque_HwNm_f32

InertiaComp_MtrNm_f32

MtrVelCRF_MtrRadpS_f32

VehicleSpeed_Kph_f32

VehicleLonAccel_KphpS_f32

BaseAssistCmd_MtrNm_f32

WIRCmdAmpBlnd_MtrNm_f32

FreqDepDmpSrlComSvcDft_Cnt_lgc

Defeat_Damping_Svc_Cnt_lgc

MEC_Counter_Cnt_enum

### Required Global Data Outputs

CombinedDamping_MtrNm_f32

### Specific Include Path present

No

## Runnable Scheduling

This section specifies the required runnable scheduling.

| **Init** | **Scheduling Requirements** | **Trigger** |
| --- | --- | --- |
| **DampingFirewall_Init** |  | On Rte_Init |

| **Runnable** | **Scheduling Requirements** | **Trigger** |
| --- | --- | --- |
| **Damping****Firewall_Per1** | triggered on TimingEvent | 2ms |

**.**

## Memory Map REQUIREMENTS

### Mapping

| Memory Section | Contents | Notes |
| --- | --- | --- |
| DAMPINGFIREWALL_START_SEC_VAR_CLEARED_32 |  |  |
| DAMPINGFIREWALL_START_SEC_VAR_CLEARED_UNSPECIFIED |  |  |
| DAMPINGFIREWALL_START_SEC_VAR_CLEARED_BOOLEAN |  |  |
| DAMPINGFIREWALL_START_SEC_VAR_CLEARED_16 |  |  |

* Each …START_SEC… constant is terminated by a …STOP_SEC… constant as specified in the AUTOSAR Memory Mapping requirements.

### Usage

| **Feature** | **RAM ** | **ROM ** |
| --- | --- | --- |
| **None** |  |  |

Table 1: ARM Cortex R4 Memory Usage

### Non  RTE NvM Blocks

| **Block Name** |
| --- |
| **None** |

Note : Size of the NVM block if configured in developer

### RTE NvM Blocks

| **Block Name** |
| --- |
| **None** |

Note : Size of the NVM block if configured in developer

## Compiler Settings

### Preprocessor MACRO

None

### Optimization Settings

None

## Appendix

*<This section is for appendix>*
