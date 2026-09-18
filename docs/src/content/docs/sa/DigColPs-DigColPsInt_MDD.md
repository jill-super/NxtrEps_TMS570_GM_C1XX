---
title: "DigColPs — DigColPsInt_MDD"
description: "Converted .docx document from DigColPs/doc."
---

> **Converted document.** Source: `DigColPs/doc/DigColPsInt_MDD.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

## Module  --

## High-Level Description

This module is responsible for the transport of sensor data between the I2C peripheral and the DigColPs Component.  This module accomplishes this task by providing a number of interface functions.  The functions handle the complexities of making request and handling the underlying interrupts to present the periodic task in the DigColPs module with the requested data on the next iteration.

## Figures

### Diagram – Function Data Sharing

See DigColPs_MDD for sequence diagram and interaction between this module, the DigColPs module and the physical sensor.

## Variable Data Dictionary

For details on module input / output variable, refer to the Data Dictionary for the application.  Input / output variable names are listed here for reference.

| Module Inputs | Module Outputs | Module Outputs |
| --- | --- | --- |
| Type_Cnt_u08 | Type_Cnt_u08 | CommFaults_Cnt_b08 |
|  |  | DataType_Cnt_u08 |
|  |  | ColSnsrData_Cnt_u16 |
|  |  | SpurSnsrData_Cnt_u16 |
|  |  | DigColPsInt_I2CHwCustData_Uls_M_u16 |

### Module Internal Variables

This section identifies the name, range and resolutions for module specific data created by this module.  If there are no range restrictions on the variable, the term “FULL” is placed into the table for legal range.

| Variable Name | Resolution | Legal Range | Legal Range | Software Segment |
| --- | --- | --- | --- | --- |
| DigColPsInt_CurrentStepNo_Cnt_M_enum | 1 | 0 | 36 | DIGCOLPSINT_START_SEC_VAR_CLEARED_UNSPECIFIED |
| DigColPsInt_InitialTime_mS_M_u32 | 1 | 0 | FULL | DIGCOLPSINT_START_SEC_VAR_CLEARED_32 |
| DigColPsInt_ColSnsrData_Cnt_M_u16 | 1 | 0 | 65535 | DIGCOLPSINT_START_SEC_VAR_CLEARED_16 |
| DigColPsInt_SpurSnsrData_Cnt_M_u16 | 1 | 0 | 65535 | DIGCOLPSINT_START_SEC_VAR_CLEARED_16 |
| DigColPsInt_ColSnsrErrData_Cnt_D_u16 | 1 | 0 | FULL | DIGCOLPSINT_START_SEC_VAR_CLEARED_16 |
| DigColPsInt_ColSnsrExtErrData_Cnt_D_u16 | 1 | 0 | FULL | DIGCOLPSINT_START_SEC_VAR_CLEARED_16 |
| DigColPsInt_ColSnsrCheckStatData_Cnt_D_u16 | 1 | 0 | FULL | DIGCOLPSINT_START_SEC_VAR_CLEARED_16 |
| DigColPsInt_SpurSnsrErrData_Cnt_D_u16 | 1 | 0 | FULL | DIGCOLPSINT_START_SEC_VAR_CLEARED_16 |
| DigColPsInt_SpurSnsrExtErrData_Cnt_D_u16 | 1 | 0 | FULL | DIGCOLPSINT_START_SEC_VAR_CLEARED_16 |
| DigColPsInt_SpurSnsrCheckStatData_Cnt_D_u16 | 1 | 0 | FULL | DIGCOLPSINT_START_SEC_VAR_CLEARED_16 |
| DigColPsInt_CurrentSlave_Cnt_M_u08 | 1 | 0 | 127 | DIGCOLPSINT_START_SEC_VAR_CLEARED_8 |
| DigColPsInt_RecvdDataType_Cnt_M_u08 | 1 | 0 | 5 | DIGCOLPSINT_START_SEC_VAR_CLEARED_8 |
| DigColPsInt_Buffer_Cnt_M_u08[] | 1 | 0 | 255 | DIGCOLPSINT_START_SEC_VAR_CLEARED_8 |
| DigColPsInt_PrevReqDataType_Cnt_M_u08 | 1 | 0 | 5 | DIGCOLPSINT_START_SEC_VAR_CLEARED_8 |
| DigColPsInt_TransactionCnt_Cnt_M_u08 | 1 | 0 | 255 | DIGCOLPSINT_START_SEC_VAR_CLEARED_8 |
| DigColPsInt_PrevTransactionCnt_Cnt_M_u0 8 | 1 | 0 | 255 | DIGCOLPSINT_START_SEC_VAR_CLEARED_8 |
| DigColPsInt_InitFailedOnce_Cnt_M_lgc | N/A | FALSE | TRUE | DIGCOLPSINT_START_SEC_VAR_CLEARED_BOOLEAN |
| DigColPsInt_BusBusySeqError_Cnt_M_lgc | N/A | FALSE | TRUE | DIGCOLPSINT_START_SEC_VAR_CLEARED_BOOLEAN |
| DigColPsInt_NackOccured_Cnt_M_lgc | N/A | FALSE | TRUE | DIGCOLPSINT_START_SEC_VAR_CLEARED_BOOLEAN |
| DigColPsInt_SkipRegisterWrite_Cnt_M_lgc | N/A | FALSE | TRUE | DIGCOLPSINT_START_SEC_VAR_CLEARED_BOOLEAN |
| DigColPsInt_RecvOverrunError_Cnt_M_lgc | N/A | FALSE | TRUE | DIGCOLPSINT_START_SEC_VAR_CLEARED_BOOLEAN |
| DigColPsInt_SensInitialized_Cnt_M_lgc | N/A | FALSE | TRUE | DIGCOLPSINT_START_SEC_VAR_CLEARED_BOOLEAN |
| DigColPsInt_I2CHwCustData_Uls_M_u16 | 1 | 0 | 511 | DIGCOLPSINT_START_SEC_VAR_CLEARED_16 |
| DigColPsInt_I2CHwIncompleteCustData_Uls_M_u16 | 1 | 0 | 255 | DIGCOLPSINT_START_SEC_VAR_CLEARED_16 |
| DigColPsInt_AttempOccurForCustDatRead_Cnt_M_u08 | 1 | 0 | 11 | DIGCOLPSINT_START_SEC_VAR_CLEARED_8 |
| DigColPsInt_CmdFailOccurred_Cnt_M_lgc | N/A | FALSE | TRUE | DIGCOLPSINT_START_SEC_VAR_CLEARED_BOOLEAN |
| DigColPsInt_ColCustDatFound_Cnt_M_lgc | N/A | FALSE | TRUE | DIGCOLPSINT_START_SEC_VAR_CLEARED_BOOLEAN |
| DigColPsInt_SpurCustDatFound_Cnt_M_lgc | N/A | FALSE | TRUE | DIGCOLPSINT_START_SEC_VAR_CLEARED_BOOLEAN |
| DigColPsInt_ResetSensor_Cnt_M_lgc | N/A | FALSE | TRUE | DIGCOLPSINT_START_SEC_VAR_CLEARED_BOOLEAN |

#### User defined typedef definition/declaration

This section documents any user types uniquely used for the module.

| Typedef Name | Element Name | User Defined Type | Legal Range | Legal Range |
| --- | --- | --- | --- | --- |
| CommStepType | INIT_NOT_INITIALIZED | uint8 | 0 | 0 |

## Constant Data Dictionary

### Calibration Constants

This section lists the calibrations used by the module.  For details on calibration constants, refer to the Data Dictionary for the application.

| Constant Name |
| --- |
| k_ColSensorI2CAddress_Cnt_u08 |
| k_I2CHWInitTransactionTime_Sec_f32 |
| k_SpurSensorI2CAddress_Cnt_u08 |

### Program(fixed) Constants

#### Embedded Constants

All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

##### Local

| Constant Name | Resolution | Units | Value |
| --- | --- | --- | --- |
| D_COLSENSOR_CNT_U08 | 1 | Cnt | 0 |
| D_SPURSENSOR_CNT_U08 | 1 | Cnt | 1 |
| D_CLEARSTATUSBITS_CNT_U16 | 1 | Cnt | 0x0007 |
| D_RESETCMD_CNT_U16 | 1 | Cnt | 0x0746 |
| D_EXTREADADDRREGCMD_CNT_U16 | 1 | Cnt | 0x0307 |
| D_EXTREADCTRLREGCMD_CNT_U16 | 1 | Cnt | 0x8000 |
| D_NACKOCCURRED_CNT_U08 | 1 | Cnt | 2 |
| D_BBSEQERR_CNT_U08 | 1 | Cnt | 4 |
| D_TRANSNOTCOMP_CNT_U08 | 1 | Cnt | 16 |
| D_ANGLEDATA_CNT_U08 | 1 | Cnt | 1 |
| D_NONE_CNT_U08 | 1 | Cnt | 0x00 |
| D_ANGLEREG_CNT_U08 | 1 | Cnt | 0x20 |
| D_CONTROLREG_CNT_U08 | 1 | Cnt | 0x1E |
| D_ERRORREG_CNT_U08 | 1 | Cnt | 0x24 |
| D_EXTERRORREG_CNT_U08 | 1 | Cnt | 0x26 |
| D_STATUSREG_CNT_U08 | 1 | Cnt | 0x22 |
| D_RECVOVERRUNERR_CNT_U08 | 1 | Cnt | 0x08 |
| D_SENSINITDELAY_MS_U08 | 1 | mS | 32 |
| D_CMDFAILED_CNT_U08 | 1 | Cnt | 0x20 |
| D_EXTREADADDRREG_CNT_U08 | 1 | Cnt | 0x0A |
| D_EXTREADCTRLREG_CNT_U08 | 1 | Cnt | 0x0C |
| D_EXTREADDATREG_CNT_U08 | 1 | Cnt | 0x0E |
| D_MAXATTEMPTSFORCUSTDATREAD_CNT_U08 | 1 | Cnt | 10 |
| D_SENSINITNOTDONE_CNT_U08 | 1 | Cnt | 1<<7U (0x80) |
| D_SECTOMILLSEC_CNT_F32 | 1 | Cnt | 1000.0F |
| D_RESETDELAY_MS_U08 | 1 | mS | 7U |

##### Global

This section lists the global constants used by the module.  For details on global constants, refer to the Data Dictionary for the application.

| Constant Name |
| --- |
| None |

#### Module specific Lookup Tables Constants

(This is for lookup tables (arrays) with fixed values, same name as other tables)

| Constant Name | Resolution | Value | Software Segment |
| --- | --- | --- | --- |
| T_DataRegisters_Cnt_u08[6] | 1 | D_NONE_CNT_U08, | DIGCOLPSINT_START_SEC_CONST_8 |

## Functions/Macros used by the Sub-Modules

### Library Functions / Macros

The library and functions / Macros that are called by the various sub modules are identified below,

1. None
### Data Hiding Functions

1. None
### Global Functions/Macros Defined by this Module

#### DigColPsInt_Reset

| **Function Name** | DigColPsInt_Reset | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | None |  |  |  |  |  |
| **Return Value** | None |  |  |  |  |  |

##### Description

#### Initialize

| **Function Name** | DigColPsInt_Init | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | None |  |  |  |  |  |
| **Return Value** | None |  |  |  |  |  |

##### Description

#### Get Data

| **Function Name** | DigColPsInt_GetData | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | ColSnsrDataPtr_Cnt_T_u16 | uint16 | Out | FULL | FULL |  |
|  | SpurSnsrDataPtr_Cnt_T_u16 | uint16 | Out | FULL | FULL |  |
|  | DataTypePtr_Cnt_T_u08 | uint8 | Out | 0 | 5 |  |
| **Return Value** | CommFaults_Cnt_T_b08 | uint8 | Out | 0 | 16 | 0 |

##### Description

#### Start Request

| **Function Name** | DigColPsInt_StartRequest | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | Type_Cnt_T_u08 | uint8 | Out | 0 | 5 |  |
| **Return Value** | None |  |  |  |  |  |

##### Description

#### Interrupt Notification

| **Function Name** | DigColPsInt_InterruptNotification | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | Flags_Cnt_T_b16 | uint16 | In | 1 | 64 |  |
| **Return Value** | None |  |  |  |  |  |

##### Design Rationale

The interrupt notification function needs to be setup by the integrator to be called by the Isr_I2C interrupt service inside of the I2cNxtr component through the use of the I2cNxtr_Cfg.h header file.  A template for that header file can be found in the I2cNxtr includes directory.

In the FDD rev.005 the timeout requirement for ‘Customer Data’ read was 5 to 10 ms. Instead of timeout it is implemented by counting the ‘Number of Attempts’ occurred to read ‘Customer Data’, because it speeds up the interrupt execution time. ‘Number of Attempts’ required to fulfill the same timeout operation is determined in the following calculation.

Number of bits sends and receives by the master to determine whether the ‘Customer Data’ is ready to read is 47bits.

So for 100Kb baud speed total time required to check control register data for both column and spur sensors is   (47*2)/100K  =  0.94 ms

Therefore for 5 ms timeout ‘Number of Attempts’ occurred = 5/0.94  = 5.32

Similarly for 10 ms timeout ‘Number of Attempts’ occurred = 10/0.94 = 10.64

Number **10** is chosen in this implementation

##### Notification Processing

#### Get Cust Data

| **Function Name** | DigColPsInt_GetCustData | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | None |  |  |  |  |  |
| **Return Value** | DigColPsInt_I2CHwCustData_Uls_M_u16 | Uint16 | Out | 0 | 511 | 0 |

##### Description

### Local Functions/Macros Used by this MDD only

#### Setup Write - Data

| **Function Name** | SetupWriteData | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | Register_Cnt_T_u08 | uint8 | In | 0 | 127 |  |
|  | Data_Cnt_T_u16 | uint16 | In | FULL | FULL |  |
| **Return Value** | None |  |  |  |  |  |

##### Description

#### Setup Write - Register

| **Function Name** | SetupWriteRegister | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | Register_Cnt_T_u08 | uint8 | In | 0 | 127 |  |
| **Return Value** | None |  |  |  |  |  |

##### Description

#### Setup Read

| **Function Name** | SetupRead | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | None |  |  |  |  |  |
| **Return Value** | None |  |  |  |  |  |

##### Description

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

#### None

### Serial Communication Functions

None

## Execution Requirements

### Execution Sequence of the Module

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
| DigColPsInt_Init | N/A |
| DigColPsInt_GetData | N/A |
| DigColPsInt_StartRequest | N/A |
| DigColPsInt_InterruptNotification | N/A |
| DigColPsInt_GetCustData | N/A |

### Local Functions

This table identifies the software segments for local functions identified in this module.

| Name of Sub Module | Software Segment |
| --- | --- |
| None |  |

## Known Issues / Limitations With Design

1. INLINE functions in GlobalMacro.h are not unit tested
## Revision Control Log

| **Item #** | **Rev #** | **Change Description** | **Date ** | **Author Initials** |
| --- | --- | --- | --- | --- |
| 1 | 1 | Initial component creation | 21-Aug-13 | Jared |
| 2 | 2 | Implemented the FDD rev.003: | 27-Feb-14 | Rijvi |
| 3 | 3 | Implemented the FDD rev.005. | 20-Mar-14 | Rijvi |
| 4 | 4 | Implemented the FDD rev.006 | 26-Mar-14 | Rijvi |
| 5 | 5 | Implemented the FDD rev 007 | 11-May-14 | Selva |
| 6 | 6 | Updated to FDD ver 008 | 27-Jun-14 | Jared |
| 7 | 7 | Updated to FDD ver12 compatibility with DSS | 05-Sep-14 | Vishnu |
| 8 | 8 | Unit Testing Finding Fixes | 13-Oct-14 | KPIT-PM |
| 9 | 9 | Updated to FDD ver 015 | 13-May-16 | JK |
