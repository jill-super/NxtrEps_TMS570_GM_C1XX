---
title: "TrqArblim — TrqArblim_MDD"
description: "Converted .docx document from TrqArblim/doc."
---

> **Converted document.** Source: `TrqArblim/doc/TrqArblim_MDD.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

## Module  -- TrqArblim

## High-Level Description

This function determines the state, calculates, and slew limits the TrqArblim command.

This function is owned by Nexteer but designed and implemented to satisfy the requirements of a particular customer.  It is not intended for use on other customer programs.

## Figures

### Diagram – Function Data Sharing

#### Diagram – Function

![figure](../../../assets/converted/TrqArblim/TrqArblim_MDD-fig5.png)

![figure](../../../assets/converted/TrqArblim/TrqArblim_MDD-fig4.png)

![figure](../../../assets/converted/TrqArblim/TrqArblim_MDD-fig3.png)

## Variable Data Dictionary

For details on module input / output variable, refer to the Data Dictionary for the application.  Input / output variable names are listed here for reference.

| Module Inputs | Module Outputs | Module Outputs |
| --- | --- | --- |
| LKACmd_HwNm_f32 | LKACmd_HwNm_f32 | IqTrqOv_HwNm_f32 |
| LKAState_State_enum | LKAState_State_enum | LKATorqueDelivered_HwNm_f32 |
| MSecureVehicleSpeed_Kph_f32 | MSecureVehicleSpeed_Kph_f32 | AssistDDFactor_Uls_f32 |
| PosServEnable_Cnt_lgc | PosServEnable_Cnt_lgc | DampingDDFactor_Uls_f32 |
| PosSrvoCmd_MtrNm_f32 | PosSrvoCmd_MtrNm_f32 | OpTrqOv_MtrNm_f32 |
| HwTorque_HwNm_f32 | HwTorque_HwNm_f32 | ReturnDDFactor_Uls_f32 |
| TrqOscCmd_MtrNm_f32 | TrqOscCmd_MtrNm_f32 | ESCIsLimited_Cnt_lgc |
| GMOSHOscillate_State_enum | GMOSHOscillate_State_enum | ESCTorqueDelivered_HwNm_f32 |
| ESCCmd_HwNm_f32 | ESCCmd_HwNm_f32 |  |
| ESCState_State_enum | ESCState_State_enum |  |

### Module Internal Variables

This section identifies the name, range and resolutions for module specific data created by this module.  If there are no range restrictions on the variable, the term “FULL” is placed into the table for legal range.

| Variable Name | Resolution | Legal Range | Legal Range | Software Segment |
| --- | --- | --- | --- | --- |
| TrqArblim_LKADesired_HwNm_D_f32 | See Data Dictionary | See Data Dictionary | See Data Dictionary | TRQARBLIM_START_SEC_VAR_CLEARED_32 |
| TrqArblim_APASmoothing_Uls_D_f32 | See Data Dictionary | See Data Dictionary | See Data Dictionary | TRQARBLIM_START_SEC_VAR_CLEARED_32 |
| TrqArblim_APADisableRate_Uls_M_f32 | See Data Dictionary | See Data Dictionary | See Data Dictionary | TRQARBLIM_START_SEC_VAR_CLEARED_32 |
| TrqArblim_FinalSlew_NmpSec_D_f32 | See Data Dictionary | See Data Dictionary | See Data Dictionary | TRQARBLIM_START_SEC_VAR_CLEARED_32 |
| TrqArblim_PreLKATrqReq_HwNm_M_f32 | See Data Dictionary | See Data Dictionary | See Data Dictionary | TRQARBLIM_START_SEC_VAR_CLEARED_32 |
| TrqArblim_HwTorqueSV_HwNm_M_Str | See Data Dictionary | See Data Dictionary | See Data Dictionary | TRQARBLIM_START_SEC_VAR_CLEARED_UNSPECIFIED |
| TrqArblim_PosSrvoCmd_MtrNm_M_f32 | See Data Dictionary | See Data Dictionary | See Data Dictionary | TRQARBLIM_START_SEC_VAR_CLEARED_32 |
| TrqArblim_ESC_State_Cnt_M_enum | See Data Dictionary | See Data Dictionary | See Data Dictionary | TRQARBLIM_START_SEC_VAR_CLEARED_UNSPECIFIED |

#### User defined typedef definition/declaration

This section documents any user types uniquely used for the module.

| Typedef Name | Element Name | User Defined Type | Legal Range | Legal Range |
| --- | --- | --- | --- | --- |

## Constant Data Dictionary

### Calibration Constants

This section lists the calibrations used by the module.  For details on calibration constants, refer to the Data Dictionary for the application.

| Constant Name |
| --- |
| k_APASmoothHwTrqLPFKn_Hz_f32 |
| k_APAEnableRate_pSec_f32; |
| k_APAUseAsstScale_lgc |
| k_APAUseRetScale_lgc |
| k_APAUseADmpScale_lgc |
| k_LKAUseSlewCal_lgc |
| k_ESCMax_HwNm_f32 |
| t_LKASlewX_Kph_u8p8[6] |
| t_LKASlewY_NmpSec_u4p12[6] |
| t_APASmoothX_Uls_u2p14[10] |
| t_APASmoothY_Uls_u2p14[10] |
| t_APADisableRateX_HwNm_u4p12[6] |
| t_APADisableRateY_pSec_u7p9[6] |

### Program(fixed) Constants

#### Embedded Constants

All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

##### Local

| Constant Name | Resolution | Units | Value |
| --- | --- | --- | --- |
| D_DSRTRQLMT_HWNM_F32 | Single precision float | HwNm | 3.0 |
| D_OPTRQOVLMT_MTRNM_F32 | Single precision float | MtrNm | 8.8 |
| D_FINALSLEWLMT_NMPSEC_F32 | Single precision float | NmpSec | 3.0 |

##### Global

This section lists the global constants used by the module.  For details on global constants, refer to the Data Dictionary for the application.

| Constant Name |
| --- |
| D_FALSE_CNT_LGC |
| D_2MS_SEC_F32 |
| D_ZERO_ULS_F32 |
| D_ONE_ULS_F32 |

#### Module specific Lookup Tables Constants

(This is for lookup tables (arrays) with fixed values, same name as other tables)

| Constant Name | Resolution | Value | Software Segment |
| --- | --- | --- | --- |
| None |  |  |  |

## Functions/Macros used by the Sub-Modules

### Library Functions / Macros

The library and functions / Macros that are called by the various sub modules are identified below,

1. FPM_FloatToFixed_m
2. FPM_FixedToFloat_m
3. IntplVarXY_u16_u16Xu16Y_Cnt
4. Limit_m
5. Abs_f32_m
### Data Hiding Functions

1. TableSize_m
### Global Functions/Macros Defined by this Module

#### Global Function #1

| **Function Name** | None | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** |  |  |  |  |  |  |
| **Return Value** |  |  |  |  |  |  |

##### Description

None

### Local Functions/Macros Used by this MDD only

#### Local Function #1

| **Function Name** | None | Type | Dir. | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | None |  |  |  |  |  |
|  | None |  |  |  |  |  |
| **Return Value** | None |  |  |  |  |  |

##### Description

None

## Software Module Implementation

### Runtime Environment (RTE) Initial Values

This section lists the initial values of data written by this module but controlled by the RTE. After RTE initialization, the data in this table will contain these values.

| Data | Value |
| --- | --- |

### Initialization Functions

#### Init: TrqArblim_Init

##### Design Rationale

Initialize the state to Inactive at the start.

##### Module Outputs

##### Module Internal

### LPF_Init_f32_m(D_ZERO_ULS_F32, k_APASmoothHwTrqLPFKn_Hz_f32, D_2MS_SEC_F32, &TrqArblim_HwTorqueSV_HwNm_M_Str);

### Periodic Functions

#### Per: TrqArblim_Per1

##### Design Rationale

None

##### Program Flow Start

Rte_Call_TrqArblim_Per1_CP0_CheckpointReached()

##### Store Module Inputs to Local copies

LKACmd_HwNm_T_f32= Rte_IRead_TrqArblim_Per1_LKACmd_HwNm_f32()

LKA_State_T_enum = Rte_IRead_TrqArblim_Per1_LKAState_State_enum()

ESCCmd_HwNm_T_f32 = Rte_IRead_TrqArblim_Per1_ESCCmd_HwNm_f32()

ESC_State_T_enum = Rte_IRead_TrqArblim_Per1_ESCState_State_enum()

MSecVehSpd_Kph_T_f32 = Rte_IRead_TrqArblim_Per1_MSecureVehicleSpeed_Kph_f32()

PosServEnable_Cnt_T_lgc = Rte_IRead_TrqArblim_Per1_PosServEnable_Cnt_lgc()

PosSrvoCmd_MtrNm_T_f32 =Rte_IRead_TrqArblim_Per1_PosSrvoCmd_MtrNm_f32()

HwTorque_HwNm_T_f32 = Rte_IRead_TrqArblim_Per1_HwTorque_HwNm_f32()

TrqOscCmd_MtrNm_T_f32 = Rte_IRead_TrqArblim_Per1_TrqOscCmd_MtrNm_f32()

GMOSHOscillate_State_T_enum = Rte_IRead_TrqArblim_Per1_GMOSHOscillate_State_enum()

##### FLOW

##### Store Local copy of outputs into Module Outputs

(void) Rte_IWrite_TrqArblim_Per1_IqTrqOv_HwNm_f32 (IqTrqOv_HwNm_T_f32)

(void)Rte_IWrite_TrqArblim_Per1_LKATorqueDelivered_HwNm_f32(LKATrqDel_HwNm_T_f32)

(void) Rte_IWrite_TrqArblim_Per1_ESCTorqueDelivered_HwNm_f32(ESCTrqDel_HwNm_T_f32)

void) Rte_IWrite_TrqArblim_Per1_ESCIsLimited_Cnt_lgc(ESCIsLimited_Cnt_T_lgc)

(void) Rte_IWrite_TrqArblim_Per1_AssistDDFactor_Uls_f32(AssistDDFactor_Uls_T_f32)

(void) Rte_IWrite_TrqArblim_Per1_DampingDDFactor_Uls_f32(DampingDDFactor_Uls_T_f32)

(void) Rte_IWrite_TrqArblim_Per1_OpTrqOv_MtrNm_f32(OpTrqOv_MtrNm_T_f32)

(void) Rte_IWrite_TrqArblim_Per1_ReturnDDFactor_Uls_f32(ReturnDDFactor_Uls_T_f32)

##### Program Flow End

### Rte_Call_TrqArblim_Per1_CP1_CheckpointReached()Fault Recovery Functions

### Shutdown Functions

None

### Interrupt Functions

None

### Serial Communication Functions

None

## Execution Requirements

### Execution Sequence of the Module

(Describe in words relevant details about the execution sequence of the different sub modules.)

### Execution Rates for sub-modules called by the Scheduler

This table serves as reference for the Scheduler design

| Function Name | Calling Frequency | System State(s) in which the function is called |
| --- | --- | --- |
| TrqArblim_Per1 | 2ms | ALL |
| TrqArblim_Init | ECU startup | ALL |

### Execution Requirements for Serial Communication Functions

| Function Name | Sub-Module called by (Serial Comm Function Name) |
| --- | --- |
| <None> |  |

## Memory Map Definition Requirements

### Sub Modules (Functions)

This table identifies the software segments for functions identified in this module.

| Name of Sub Module | Software Segment |
| --- | --- |
| TrqArblim_Per1 | RTE_START_SEC_AP_TRQARBLIM_APPL_CODE |
| TrqArblim_Init | RTE_START_SEC_AP_TRQARBLIM_APPL_CODE |

### Local Functions

This table identifies the software segments for local functions identified in this module.

| Name of Sub Module | Software Segment |
| --- | --- |

## Known Issues / Limitations With Design

1. Global Macros are not unit tested.
## Revision Control Log

| **Item #** | **Rev #** | **Change Description** | **Date ** | **Author Initials** |
| --- | --- | --- | --- | --- |
| 1 | 1 | Initial revision | 23-Jan-14 | Selva |
| 2 | 2 | Unit Testing Finding Fixes | 27-Mar-2014 | KPIT-SSK |
| 3 | 3 | A6345 fixes + fixes for UTP | 21-Apr-14 | Selva |
| 4 | 4 | Change PosServoCommand input units from HwNm to MtrNm as per A6682 | 2-May-14 | JWJ |
| 5 | 5 | Implemented CF-10 GM Torque Arbitrator v002 – 12180 | 21-Jul-14 | SB |
| 6 | 6 | A7189 - Global output not range limited | 09-Sep-14 | SB |
