---
title: "Integration — doc/Vehicle_Power_Mode_MDD"
description: "Converted document Vehicle_Power_Mode_MDD.docx."
---

> **Converted document.** Source: `GM_C1XX_EPS_TMS570/SwProject/VehPwrMd/doc/Vehicle_Power_Mode_MDD.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

## Module –

## High-Level Description

## Figures

### Component Diagram

![figure](../../../assets/converted/VehPwrMd/Vehicle_Power_Mode_MDD-fig2.png)

## Variable Data Dictionary

For details on module input / output variable, refer to the Data Dictionary for the application.  Input / output variable names are listed here for reference.

| Module Inputs | Module Outputs | Module Outputs |
| --- | --- | --- |
| EngONSrlComSvcDft_Cnt_lgc | EngONSrlComSvcDft_Cnt_lgc | OperRampRate_XpmS_f32 |
| SrlComEngOn_Cnt_lgc | SrlComEngOn_Cnt_lgc | OperRampValue_Uls_f32 |
| SrlComSPMOn_Cnt_lgc | SrlComSPMOn_Cnt_lgc | ATermActive_Cnt_lgc |
| VehSpdValid_Cnt_lgc | VehSpdValid_Cnt_lgc | CTermActive_Cnt_lgc |
| VehSpd_Kph_f32 | VehSpd_Kph_f32 |  |

### Module Internal Variables

This section identifies the name, range and resolutions for module specific data created by this module.  If there are no range restrictions on the variable, the term “FULL” is placed into the table for legal range.

| Variable Name | Resolution | Legal Range | Legal Range | Software Segment |
| --- | --- | --- | --- | --- |
| IGNDiagStartTime_mS_M_u32p0 | 1 | FULL | FULL | VEHPWRMD_START_SEC_VAR_CLEARED_32 |

#### User defined typedef definition/declaration

This section documents any user types uniquely used for the module.

| Typedef Name | Element Name | User Defined Type | Legal Range | Legal Range |
| --- | --- | --- | --- | --- |
| <None> |  |  |  |  |

## Constant Data Dictionary

### Calibration Constants

This section lists the calibrations used by the module.  For details on calibration constants, refer to the Data Dictionary for the application.

| Constant Name |
| --- |
| k_RampUpRtLoSpd_UlspmS_f32 |
| k_RampDnRt_UlspmS_f32 |
| k_RmpDnAsstVehSpdLimit_Kph_f32 |
| k_IGNDiagTime_mS_u16p0 |

### Program(fixed) Constants

#### Embedded Constants

All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

##### Local

| Constant Name | Resolution | Units | Value |
| --- | --- | --- | --- |
| <None> |  |  |  |

##### Global

This section lists the global constants used by the module.  For details on global constants, refer to the Data Dictionary for the application.

| Constant Name |
| --- |
| D_ZERO_ULS_F32 |

#### Module specific Lookup Tables Constants

| Constant Name | Resolution | Value | Software Segment |
| --- | --- | --- | --- |
| <None> |  |  |  |

## Functions/Macros used by the Sub-Modules

### Library Functions / Macros

The library and functions / Macros that are called by the various sub modules are identified below,

1. Rte_Call_EpsEn_OP_GET
2. Rte_Call_NxtrDiagMgr_GetNTCFailed
3. NtWrapC_CanStart
4. NtWrapC_CanStop
5. NtWrapC_SrlComInput_SCom_ResetBus1Timers
6. NtWrapC_SrlComInput_SCom_ResetBus2Timers
### Data Hiding Functions

1. Rte_Mode_SystemState_Mode
### Global Functions/Macros Defined by this Module

#### Global Function #1

| **Function Name** | <None> | Type | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | <None> |  |  |  |  |
| **Return Value** | N/A |  |  |  |  |

##### Description

### Local Functions/Macros Used by this MDD only

#### Local Function #1

| **Function Name** | IgnFailureDiag | Type | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | SrlComEngOn_Cnt_T_lgc | boolean | FALSE | TRUE |  |
|  | SrlComSPMOn_Cnt_T_lgc | boolean | FALSE | TRUE |  |
|  | EPSEn_Cnt_T_lgc | boolean | FALSE | TRUE |  |
| **Return Value** | N/A |  |  |  |  |

##### Description

## Software Module Implementation

### Runtime Environment (RTE) Initial Values

This section lists the initial values of data written by this module but controlled by the RTE. After RTE initialization, the data in this table will contain these values.

| Data | Value |
| --- | --- |
| ATermActive_Cnt_lgc | TRUE |
| CTermActive_Cnt_lgc | FALSE |
| EngONSrlComSvcDft_Cnt_lgc | FALSE |
| OperRampRate_XpmS_f32 | 0.0F |
| OperRampValue_Uls_f32 | 0.0F |
| SrlComEngOn_Cnt_lgc | FALSE |
| SrlComSPMOn_Cnt_lgc | FALSE |
| VehSpd_Kph_f32 | 0.0F |
| VehSpdValid_Cnt_lgc | FALSE |

### Initialization Functions

#### Init: _Init1(void)

##### Design Rationale

None

##### Module Outputs

Rte_IWrite_VehPwrMd_Init1_OperRampRate_XpmS_f32(k_RampDnRt_UlspmS_f32)

Rte_IWrite_VehPwrMd_Init1_OperRampValue_Uls_f32(D_ZERO_ULS_F32)

##### Module Internal

None

### Periodic Functions

#### Per: _Per1()

##### Design Rationale

None

##### Program Flow Start

Rte_Call_VehPwrMd_Per1_CP0_CheckpointReached()

##### Store Module Inputs to Local copies

EngONSrlComSvcDft_Cnt_T_lgc = Rte_IRead_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc()

Rte_Call_EpsEn_OP_GET(&EPSEn_Cnt_T_lgc)

SrlComEngOn_Cnt_T_lgc = Rte_IRead_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc()

SrlComSPMOn_Cnt_T_lgc = Rte_IRead_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc()

VehSpdValid_Cnt_T_lgc = Rte_IRead_VehPwrMd_Per1_VehSpdValid_Cnt_lgc()

VehSpd_Kph_T_f32 = Rte_IRead_VehPwrMd_Per1_VehSpd_Kph_f32()

Rte_Call_NxtrDiagMgr_GetNTCFailed(NTC_Num_MissingMsg_N, &EngMissingFlt_Cnt_T_lgc)

SystemState_Cnt_T_enum = Rte_Mode_SystemState_Mode()

##### Processing of function

##### Store Local copy of outputs into Module Outputs

Rte_IWrite_VehPwrMd_Per1_OperRampRate_XpmS_f32(OperRampRate_XpmS_T_f32)

Rte_IWrite_VehPwrMd_Per1_OperRampValue_Uls_f32(OperRampValue_Uls_T_f32)

Rte_IWrite_VehPwrMd_Per1_ATermActive_Cnt_lgc(ATermActive_Cnt_T_lgc)

Rte_IWrite_VehPwrMd_Per1_CTermActive_Cnt_lgc(CTermActive_Cnt_T_lgc)

##### Program Flow End

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached()

#### Per: _trns1()

##### Design Rationale

None

##### Program Flow Start

N/A

##### Store Module Inputs to Local copies

None

##### Processing of function

NtWrapC_CanStop()

##### Store Local copy of outputs into Module Outputs

None

##### Program Flow End

N/A

#### Per: _trns2()

##### Design Rationale

None

##### Program Flow Start

N/A

##### Store Module Inputs to Local copies

None

##### Processing of function

NtWrapC_SrlComInput_SCom_ResetBus1Timers()

NtWrapC_SrlComInput_SCom_ResetBus2Timers()

NtWrapC_CanStart()

##### Store Local copy of outputs into Module Outputs

None

##### Program Flow End

N/A

### Fault Recovery Functions

None

### Shutdown Functions

None

### Interrupt Functions

None

### Serial Communication Functions

#### SCom: VehPwrMd_SCom_

##### Design Rationale

None

##### Program Flow Start

N/A

##### Store Module Inputs to Local copies

None

##### Processing of function

##### Store Local copy of outputs into Module Outputs

None

##### Program Flow End

N/A

## Execution Requirements

### Execution Sequence of the Module

### Execution Rates for sub-modules called by the Scheduler

This table serves as reference for the Scheduler design

| Function Name | Calling Frequency | System State(s) in which the function is called |
| --- | --- | --- |
| VehPwrMd_Per1 | 2ms | OFF, DISABLE, WARMINIT, OPERATE |
| VehPwrMd_Trns1 | On Event | On transition to OFF |
| VehPwrMd_Trns2 | On Event | On transition from OFF |

### Execution Requirements for Serial Communication Functions

| Function Name | Sub-Module called by (Serial Comm Function Name) |
| --- | --- |
| <None> |  |

## Memory Map Definition Requirements

### Sub Modules (Functions)

This table identifies the software segments for functions identified in this module.

| Name of Sub Module | Software Segment |
| --- | --- |
| VehPwrMd_Per1 | RTE_START_SEC_AP_VEHPWRMD_APPL_CODE |
| VehPwrMd_Trns1 | RTE_START_SEC_AP_VEHPWRMD_APPL_CODE |
| VehPwrMd_Trns2 | RTE_START_SEC_AP_VEHPWRMD_APPL_CODE |

### Local Functions

This table identifies the software segments for local functions identified in this module.

| Name of Sub Module | Software Segment |
| --- | --- |
| IgnFailureDiag |  |

## Known Issues / Limitations With Design

1. INLINE functions defined in GlobalMacro.h are not unit tested.
## Revision Control Log

| **Item #** | **Rev #** | **Change Description** | **Date ** | **Author Initials** |
| --- | --- | --- | --- | --- |
| 1 | 1.0 | Initial Version | 29-July-13 | LWW |
