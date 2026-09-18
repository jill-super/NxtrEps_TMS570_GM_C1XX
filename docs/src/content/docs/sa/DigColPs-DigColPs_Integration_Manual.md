---
title: "DigColPs — DigColPs_Integration_Manual"
description: "Converted .docx document from DigColPs/doc."
---

> **Converted document.** Source: `DigColPs/doc/DigColPs_Integration_Manual.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

**Integration Manual**

**For**

**DigColPs**

**VERSION: ****2.0**

**DATE: ****12-MAY-2016**

**Prepared By: **

**Software Engineering Group****,**

**Nexteer Automotive,**

** Saginaw,** **MI****, ****USA**

**Location:** The official version of this document is stored in the Nexteer Configuration Management System.

**Revision History**

| **Sl. No.** | **Description** | **Author** | **Version** | **Date** |
| --- | --- | --- | --- | --- |
| 1 | Initial version | Jared | 1.0 | 08/22/13 |
| 2 | Implemented FDD v015 – ES20D | JK | 2.0 | 05/12/16 |

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
| 1 | ES20D FDD | 015 |
|  | <Add if more available> |  |

## Dependencies

### SWCs

| **Module** | **Required Feature** |
| --- | --- |
| I2cNxtr | All functions |

Note : Referencing the external components should be avoided in most cases. Only in unavoidable circumstance external components should be referred. Developer should track the references.

### Global Functions(Non RTE) to be provided to Integration Project

None

## Configuration REQUIREMeNTS

### Build Time Config

| **Modules** | **Notes** |  |
| --- | --- | --- |
| **None** |  |  |

### Configuration Files to be provided by Integration Project

<Configuration file that will generated from this components that will require Da Vinci Config generation or manual generation. Describe each parameter >

### Da Vinci Parameter Configuration Changes

| **Parameter** | **Notes** | **SWC** |
| --- | --- | --- |
| **<Configurator  Changes for parameters>** |  |  |

### DaVinci Interrupt Configuration Changes

| **ISR Name** | **VIM #** | **Priority Dependency** | **Notes** |
| --- | --- | --- | --- |
| **<Configurator  Changes for  Interrupts>** |  |  |  |

### Manual Configuration Changes

| **Constant** | **Notes** | **SWC** |
| --- | --- | --- |
| D_COMMBUFFERSIZE_CNT_U08 | 3 | I2cNxtr |
| I2c_Notification | DigColPsInt_InterruptNotification | I2cNxtr |
| D_I2CREG_STRCPTR | i2cREG1 | I2cNxtr |
| D_VCLK_HZ_F32 | Set to corresponding VCLK frequency, commonly 8000000.0 for a 160.0 MHz part. | I2cNxtr |

## Integration  DATAFLOW REQUIREMENTS

### Required Global Data Inputs

Refer .m file in FDD

### Required Global Data Outputs

Refer .m file in FDD

### Specific Include Path present

Yes

## Runnable Scheduling

This section specifies the required runnable scheduling.

| **Init** | **Scheduling Requirements** | **Trigger** |
| --- | --- | --- |
| DigColPs_Init1 | None | RTE(Init) |

| **Runnable** | **Scheduling Requirements** | **Trigger** |
| --- | --- | --- |
| DigColPs_Per1 | Early in 2 ms task to minimize jitter | RTE (2 ms) |
| DigColPs_Per2 | None | RTE (4 ms) |
| DigColPs_Per3 | None | RTE (100 ms) |

**.**

## Memory Map REQUIREMENTS

### Mapping

| **Memory Section** | **Contents** | **Notes** |
| --- | --- | --- |
| DIGCOLPS_START_SEC_VAR_CLEARED_32 | float32,uint32 |  |
| DIGCOLPS_START_SEC_VAR_CLEARED_16 | uint16 |  |
| DIGCOLPS_START_SEC_VAR_CLEARED_8 | uint8, sint8 |  |
| DIGCOLPS_START_SEC_VAR_CLEARED_BOOLEAN | Boolean |  |
| DIGCOLPS_START_SEC_VAR_CLEARED_UNSPECIFIED | LPF32KSV_Str |  |

* Each …START_SEC… constant is terminated by a …STOP_SEC… constant as specified in the AUTOSAR Memory Mapping requirements.

### Usage

| **Feature** | **RAM ** | **ROM ** |
| --- | --- | --- |
| **None** |  |  |

Table 1: ARM Cortex R4 Memory Usage

### NvM Blocks

Rte_Pim_DigColPsEOL

## Compiler Settings

### Preprocessor MACRO

None

### Optimization Settings

None

## Appendix

None
