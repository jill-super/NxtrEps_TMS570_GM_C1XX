---
title: "StOpCtrl — StateOutput Control_IntegrationManual"
description: "Converted .docx document from StOpCtrl/doc."
---

> **Converted document.** Source: `StOpCtrl/doc/StateOutput Control_IntegrationManual.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

**Integration Manual**

**For**

**State Output Control**

**VERSION: ****.****0**

**DATE: ****-****-****2015**

**Prepared By: **

**,**

**Nexteer Automotive,**

** Saginaw,** **MI, USA**

**Revision History**

| **Rev #** | **Change Description** | **Date ** | **Author** |
| --- | --- | --- | --- |
| 1 | Initial version | 30-Jan-15 | SB |
| 2 | Updated SF-05 v004 based on FDD v4.0.0 | 10-Apr-15 | KK |

**Table of Contents**

## Abbrevations And Acronyms

| **Abbreviation** | **Description** |
| --- | --- |
| DFD | Design functional diagram |
| MDD | Module design Document |

## References

This section lists the title & version of all the documents that are referred for development of this document

| **Sr. No.** | **Title** | **Version** |
| --- | --- | --- |
| 1 | SF05A State Output Control | 4. |

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

### Da Vinci Parameter Configuration Changes

| **Parameter** | **Notes** | **SWC** |
| --- | --- | --- |
| **None** |  |  |

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

DiagRampRate_XpmS_f32

DiagRampValue_Uls_f32

DiagStsDiagRmpActive_Cnt_lgc

OperRampRate_XpmS_f32

OperRampValue_Uls_f32

RampSrlComSvcDft_Cnt_lgc

LoaRateLimit_UlspS_f32

LoaScaleFctr_Uls_f32

StrtStopRateLimit_UlspS_f32

StrtStopScaleFctr_Uls_f32

### Required Global Data Outputs

OutputRampMult_Uls_f32

### SysStReqDi_Cnt_lgcSpecific Include Path present

No

## Runnable Scheduling

This section specifies the required runnable scheduling.

| **Init** | **Scheduling Requirements** | **Trigger** |
| --- | --- | --- |

| **Runnable** | **Scheduling Requirements** | **Trigger** |
| --- | --- | --- |
| **StOpCtrl****_Per1** | triggered on TimingEvent | RTE 2ms |

**.**

## Memory Map REQUIREMENTS

### Mapping

| **Memory Section** | **Contents** | **Notes** |
| --- | --- | --- |
| STOPCTRL_START_SEC_VAR_INIT_08 |  |  |
| STOPCTRL_START_SEC_VAR_CLEARED_32 |  |  |

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
