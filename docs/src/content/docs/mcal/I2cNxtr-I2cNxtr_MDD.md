---
title: "I2cNxtr — I2cNxtr_MDD"
description: "Converted .docx document from I2cNxtr/doc."
---

> **Converted document.** Source: `I2cNxtr/doc/I2cNxtr_MDD.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

## Module  -- I2C Nexteer

This document describes the software design and implementation of the Nexteer inter-integrated circuit (I2C) driver for EA3.x applications.

## Equations for Register Settings

Depending on the type of device attached to the I2C bus different register settings may be required. The following equations were used to determine the module clock frequency and high and low times for the required device that are documented in this MDD.

### Module Clock Frequency

The module clock frequency determines the frequency at which the I2C module operates. The value in the prescale register (I2CPSC) is programmable and divides the input clock to produce the module clock. The module clock frequency must be between 6.7 MHz and 13.3 MHz for proper operation of the I2C module. At the time this specification was created, the input clock frequency is 80MHz.

### Master Clock Frequency

The master clock frequency is the frequency that will be used on the SCL pin of the TMS570 device when in master mode. Depending on the value of the I2CPSC and the desired clock low (I2CCKL) and high (I2CCKH) times, the mast clock frequency can be calculated by one of the two equations below:

Where *d* depends on:

| I2CPSC | d |
| --- | --- |
| 0 | 7 |
| 1 | 6 |
| Greater than 1 | 5 |

## Variable Data Dictionary

For details on module input / output variable, refer to the Data Dictionary for the application.  Input / output variable names are listed here for reference.

| Module Inputs | Module Outputs | Module Outputs |
| --- | --- | --- |
| None | None | None |

### Module Internal Variables

This section identifies the name, range and resolutions for module specific data created by this module.  If there are no range restrictions on the variable, the term “FULL” is placed into the table for legal range.

| Variable Name | Resolution | Legal Range | Legal Range | Software Segment |
| --- | --- | --- | --- | --- |
| I2cNxtr_I2cTransfer_Cnt_M_str. Mode_Cnt_b32 | 1 | 0 | 0x10 | I2CNXTR_START_SEC_VAR_CLEARED_UNSPECIFIED |
| I2cNxtr_I2cTransfer_Cnt_M_str. Length_Cnt_u32 | 1 | FULL | FULL | I2CNXTR_START_SEC_VAR_CLEARED_UNSPECIFIED |
| I2cNxtr_I2cTransfer_Cnt_M_str. DataPtr_Cnt_u08 | 1 | FULL | FULL | I2CNXTR_START_SEC_VAR_CLEARED_UNSPECIFIED |

#### User defined typedef definition/declaration

This section documents any user types uniquely used for the module.

| Typedef Name | Element Name | User Defined Type | Legal Range | Legal Range |
| --- | --- | --- | --- | --- |
| i2cctrlregs_t | OAR | uint32 | 0 | 1023 |
| I2cTransferType | Mode_Cnt_b32 | uint32 | FULL | FULL |
| enum i2cMode | I2C_FD_FORMAT | uint16 | 0x0008 | 0x0008 |
| enum i2cBitCount | I2C_2_BIT | uint16 | 0x2 | 0x2 |
| enum i2cIntFlags | I2C_AL_INT | uint16 | 0x0001 | 0x0001 |
| enum i2cStatFlags | I2C_AL | uint16 | 0x0001 | 0x0001 |
| enum i2cDMA | I2C_TXDMA | uint16 | 0x20 | 0x20 |
| struct g_i2cTransfer | mode | uint32 | Full | Full |

## Constant Data Dictionary

### Calibration Constants

This section lists the calibrations used by the module.  For details on calibration constants, refer to the Data Dictionary for the application.

| Constant Name |
| --- |
| None |

### Program(fixed) Constants

#### Embedded Constants

All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

##### Local

| Constant Name | Resolution | Units | Value |
| --- | --- | --- | --- |

##### Global

This section lists the global constants used by the module.  For details on global constants, refer to the Data Dictionary for the application.

| Constant Name |
| --- |
| None |

#### Module specific Lookup Tables Constants

(This is for lookup tables (arrays) with fixed values, same name as other tables)

| Constant Name | Resolution | Value | Software Segment |
| --- | --- | --- | --- |
| None |  |  |  |

## Functions/Macros used by the Sub-Modules

### Library Functions / Macros

The library and functions / Macros that are called by the various sub modules are identified below,

1. None
### Data Hiding Functions

1. None
### Global Functions/Macros Defined by this Module

#### I2C Init

| **Function Name** | I2c_Init | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Enable

| **Function Name** | I2c_Enable | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Reset

| **Function Name** | I2c_Reset | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Setup Master Transmit

| **Function Name** | I2c_SetupMasterTransmit | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
|  | SlaveAddress_Cnt_T_u08 | uint8 | In | 0 | 127 |  |
|  | DataLength_Cnt_T_u16 | uint16 | In | FULL | FULL |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Setup Master Receive

| **Function Name** | I2c_SetupMasterReceive | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
|  | SlaveAddress_Cnt_T_u08 | uint8 | In | 0 | 127 |  |
|  | DataLength_Cnt_T_u16 | uint16 | In | FULL | FULL |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Switch Master Receive

| **Function Name** | I2c_SwitchMasterReceive | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
|  | DataLength_Cnt_T_u16 | uint16 | In | FULL | FULL |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Set Count

| **Function Name** | I2c_SetCount | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
|  | Count_Cnt_T_u16 | uint16 | In | 0 | 65535 |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Set Own Address

| **Function Name** | I2c_SetOwnAdd | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
|  | Address_Cnt_T_u16 | uint16 | In | 1 | 127 |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Set Slave Address

| **Function Name** | I2c_SetSlaveAdd | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
|  | Address_Cnt_T_u16 | uint16 | In | 1 | 127 |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Set Functional

| **Function Name** | I2c_SetFunctional | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
|  | Port_Cnt_T_u08 | Uint8 | In | FULL | FULL |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Set Baudrate

| **Function Name** | I2c_SetBaudrate | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
|  | Baud_Hz_T_u32 | uint32 | In | 1 | FULL |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Is TX Ready

| **Function Name** | I2c_IsTxReady | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
| **Return Value** | Ready_Cnt_T_lgc | boolean | Out | FALSE | TRUE | N/A |

##### Description

#### I2C Send Byte

| **Function Name** | I2c_SendByte | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
|  | Byte_Cnt_T_u08 | uint8 | In | FULL | FULL |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Send

| **Function Name** | I2c_Send | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
|  | Length_Cnt_T_u32 | uint32 | In | FULL | FULL |  |
|  | DataPtr_Cnt_T_u08 | *uint8 | In | FULL | FULL |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Is RX Ready

| **Function Name** | I2c_IsRxReady | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
| **Return Value** | Ready_Cnt_T_lgc | boolean | Out | FALSE | TRUE |  |

##### Description

#### I2C RX Error

| **Function Name** | I2c_RxError | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
| **Return Value** | Status_Cnt_T_b32 | uint32 | Out | FULL | FULL |  |

##### Description

#### I2C Receive Ready

| **Function Name** | I2c_ReceiveByte | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
| **Return Value** | Data_Cnt_T_u08 | uint8 | Out | FULL | FULL |  |

##### Description

#### I2C Set Receive

| **Function Name** | I2c_SetRecv | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
|  | Length_Cnt_T_u32 | uint32 | In | FULL | FULL |  |
|  | DataPtr_Cnt_T_u08 | *uint8 | Out | FULL | FULL |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Set Direction

| **Function Name** | I2c_SetDirection | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
|  | Dir_Cnt_T_u08 | uint8 | In | FULL | FULL |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Set Bit

| **Function Name** | I2c_SetBit | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
|  | Bit_Cnt_T_u08 | uint8 | In | 0 | 31 |  |
|  | Value_Cnt_T_u08 | uint8 | In | 0 | 1 |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Get Bit

| **Function Name** | I2c_GetBit | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
|  | Bit_Cnt_T_u08 | uint8 | In | 0 | 31 |  |
| **Return Value** | Value_Cnt_T_u08 | uint8 | Out | 0 | 1 |  |

##### Description

#### I2C Enable Notification

| **Function Name** | I2c_EnableNotification | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
|  | Flags_Cnt_T_b32 | uint32 | In | FULL | FULL |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Disable Notification

| **Function Name** | I2c_DisableNotification | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
|  | Flags_Cnt_T_b32 | uint32 | In | FULL | FULL |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Generate Start Condition

| **Function Name** | I2c_GenStartCond | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Generate Stop Condition

| **Function Name** | I2c_GenStopCond | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

#### I2C Get Interrupt Vector

| **Function Name** | I2c_GetIntVect | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
| **Return Value** | Vector_Cnt_T_u08 | uint8 | Out | 0 | 7 |  |

##### Description

#### I2C Get Status

| **Function Name** | I2c_GetStatus | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
| **Return Value** | Status_Cnt_T_u16 | uint16 | Out | FULL | FULL |  |

##### Description

#### I2C Set Status

| **Function Name** | I2c_SetStatus | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | I2cRegPtr_Cnt_T_str | i2cctrlregs_t | In/Out | See section 2.1.1 | See section 2.1.1 |  |
|  | Status_Cnt_T_u16 | uint16 | In | FULL | FULL |  |
| **Return Value** | N/A |  |  |  |  |  |

##### Description

### Local Functions/Macros Used by this MDD only

None

## Software Module Implementation

### Runtime Environment (RTE) Initial Values

This section lists the initial values of data written by this module but controlled by the RTE. After RTE initialization, the data in this table will contain these values.

| Data | Value |
| --- | --- |
| None |  |

### Initialization Functions

None

### Periodic Functions

None

### Fault Recovery Functions

None

### Shutdown Functions

None

### Interrupt Functions

#### Isr: Isr_I2c

##### Design Rationale

None

##### Program Flow Start

Metrics_TaskStart(D_I2CNXT_CNT_U08)

##### I2c Notification

##### Program Flow End

Metrics_TaskEnd(D_I2CNXT_CNT_U08)

### Serial Communication Functions

None

## Execution Requirements

### Execution Sequence of the Module

(Describe in words relevant details about the execution sequence of the different sub modules.)

### Execution Rates for sub-modules called by the Scheduler

This table serves as reference for the Scheduler design

| Function Name | Calling Frequency | System State(s) in which the function is called |
| --- | --- | --- |
| None |  |  |

### Execution Requirements for Serial Communication Functions

| Function Name | Sub-Module called by (Serial Comm Function Name) |
| --- | --- |
| None |  |

## Memory Map Definition Requirements

### Sub Modules (Functions)

This table identifies the software segments for functions identified in this module.

| Name of Sub Module | Software Segment |
| --- | --- |
| I2c_Init | N/A |
| I2c_Enable | N/A |
| I2c_Reset | N/A |
| I2c_SetupMasterTransmit | N/A |
| I2c_SetupMasterReceive | N/A |
| I2c_SwitchMasterReceive | N/A |
| I2c_SetCount | N/A |
| I2c_SetOwnAdd | N/A |
| I2c_SetSlaveAdd | N/A |
| I2c_SetFunctional | N/A |
| I2c_SetBaudrate | N/A |
| I2c_IsTxReady | N/A |
| I2c_SendByte | N/A |
| I2c_Send | N/A |
| I2c_IsRxReady | N/A |
| I2c_RxError | N/A |
| I2c_ReceiveByte | N/A |
| I2c_SetRecv | N/A |
| I2c_SetDirection | N/A |
| I2c_SetBit | N/A |
| I2c_GetBit | N/A |
| I2c_EnableNotification | N/A |
| I2c_DisableNotification | N/A |
| I2c_GenStartCond | N/A |
| I2c_GenStopCond | N/A |
| I2c_GetIntVect | N/A |
| I2c_GetStatus | N/A |
| I2c_SetStatus | N/A |

### Local Functions

This table identifies the software segments for local functions identified in this module.

| Name of Sub Module | Software Segment |
| --- | --- |
| None |  |

## Known Issues / Limitations With Design

1. None
## Revision Control Log

| **Item #** | **Rev #** | **Change Description** | **Date ** | **Author Initials** |
| --- | --- | --- | --- | --- |
| 1 | 1 | Initial component creation | 22-Aug-13 | Jared |
| 2 | 2 | Add Metrics hook. | 7-Oct-13 | BWL |
| 3 | 3 | New enum is created and receiver overrun is checked when receive data | 24-Feb-14 | Rijvi |
