---
title: "I2cNxtr — I2cNxtr_Integration_Manual"
description: "Converted .docx document from I2cNxtr/doc."
---

> **Converted document.** Source: `I2cNxtr/doc/I2cNxtr_Integration_Manual.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

# Integration Manual – I2cNxtr

Table of Contents

## Dependencies

### SWCs

| Module | Required Feature |
| --- | --- |
| None |  |

Note : Referencing the external components should be avoided in most cases. Only in unavoidable circumstance external components should be referred. Developer should track the references.

### Global Functions(Non RTE) to be provided to Integration Project

- I2c_Init
- I2c_Enable
- I2c_Reset
- I2c_SetupMasterTransmit
- I2c_SetupMasterReceive
- I2c_SwitchMasterReceive
- I2c_SetCount
- I2c_SetOwnAdd
- I2c_SetSlaveAdd
- I2c_SetFunctional
- I2c_SetBaudrate
- I2c_IsTxReady
- I2c_SendByte
- I2c_Send
- I2c_IsRxReady
- I2c_RxError
- I2c_ReceiveByte
- I2c_SetRecv
- I2c_SetDirection
- I2c_SetBit
- I2c_GetBit
- I2c_EnableNotification
- I2c_DisableNotification
- I2c_GenStartCond
- I2c_GenStopCond
- I2c_GetIntVect
- I2c_GetStatus
- I2c_SetStatus
## Configuration

### Build Time Config

| Modules | Notes |  |
| --- | --- | --- |
| None |  |  |

### Configuration Files to be provided by Integration Project

#### Da Vinci Parameter Configuration Changes

| Parameter | Notes | SWC |
| --- | --- | --- |
| None |  |  |

#### DaVinci Interrupt Configuration Changes

| ISR Name | VIM # | Priority Dependency | Notes |
| --- | --- | --- | --- |
| Isr_I2c | 66 | None | See comment below about enable/disable for very low priority interrupts. |

#### Interrupt Enable/Disable Functions

Verify that interrupt 66 can be enabled and disabled in interrupts.c.  It was found that only interrupts up to 63 could be enabled and disabled with current code.  Below is a suggestion of how the enable function should look:

And similarly for the disable function:

Additionally, EnableI2CInterrupt and DisableI2CInterrupt will need to be defined in interrupts.c in a fashion similar to the other Enable* and Disable* interrupts.

#### Manual Configuration Changes

| Constant | Notes | SWC |
| --- | --- | --- |
| D_COMMBUFFERSIZE_CNT_U08 | Transmit and receive buffer size in bytes. | I2cNxtr |
| I2c_Notification | Callback notification issued when I2C interrupt occurs. | I2cNxtr |
| D_I2CREG_STRCPTR | Pointer to register structure containing I2C registers. | I2cNxtr |
| D_VCLK_HZ_F32 | VCLK frequency used when calculating I2C baud rate. | I2cNxtr |

## Integration

### Required Global Data Inputs

None

### Required Global Data Outputs

None

### Specific Include Path present

Yes

## Runnable Scheduling

This section specifies the required runnable scheduling.

| Init | Scheduling Requirements | Trigger |
| --- | --- | --- |
| None | None | N/A |

| Runnable | Scheduling Requirements | Trigger |
| --- | --- | --- |
| None | None | N/A |

**.**

## Memory Mapping

### Mapping

| Memory Section | Contents | Notes |
| --- | --- | --- |
| I2CNXTR_START_SEC_VAR_CLEARED_UNSPECIFIED | I2cTransferType |  |

* Each …START_SEC… constant is terminated by a …STOP_SEC… constant as specified in the AUTOSAR Memory Mapping requirements.

### Usage

| Feature | RAM | ROM |
| --- | --- | --- |
| None |  |  |

Table 1: ARM Cortex R4 Memory Usage

### Non  RTE NvM Blocks

| Block Name |
| --- |
| None |

Note : Size of the NVM block if configured in developer

### RTE NvM Blocks

| Block Name |
| --- |
| None |

Note : Size of the NVM block if configured in developer

## Compiler Settings

### Preprocessor MACRO

None

### Optimization Settings

None

## Revision Control Log

| **Rev #** | **Change Description** | **Date ** | **Author** |
| --- | --- | --- | --- |
| 1 | Initial component creation | 22-Aug-13 | Jared |
