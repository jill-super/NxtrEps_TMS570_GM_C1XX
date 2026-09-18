---
title: "MtrCtrl_CM — TrqCanc_MDD"
description: "Converted .docx document from MtrCtrl_CM/doc."
---

> **Converted document.** Source: `MtrCtrl_CM/doc/TrqCanc_MDD.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

## Module -- TrqCanc

## High-Level Description

## Figures

### Component Diagram

![figure](../../../assets/converted/MtrCtrl_CM/TrqCanc_MDD-fig11.png)

## Variable Data Dictionary

For details on module input / output variable, refer to the Data Dictionary for the application.  Input / output variable names are listed here for reference.

| Module Inputs | Module Outputs | Module Outputs |
| --- | --- | --- |
| Refer the Data dictionary | Refer the Data dictionary | Refer the Data dictionary |

### Module Internal Variables

This section identifies the name, range and resolutions for module specific data created by this module.  If there are no range restrictions on the variable, the term “FULL” is placed into the table for legal range.

| Variable Name | Resolution | Legal Range | Legal Range | Software Segment |
| --- | --- | --- | --- | --- |
| Refer the Data dictionary | Refer the Data dictionary | Refer the Data dictionary | Refer the Data dictionary | Refer the Data dictionary |

#### User defined typedef definition/declaration

This section documents any user types uniquely used for the module.

| Typedef Name | Element Name | User Defined Type | Legal Range | Legal Range |
| --- | --- | --- | --- | --- |
| CoggingM_Amp_Str | CoggingMX_MtrNm_s2p13 | sint16 | FULL | FULL |
|  | CoggingMY_MtrNm_s2p13 | sint16 | FULL | FULL |
| CogTrqCalPtr | Rte_Pim_CogTrqCal()[512] | Uint16 | -1 | 1 |
| CogTrqCalRplCompPtr | Rte_Pim_CogTrqRplComp()[9] | Uint16 | -1 | 1 |

## Constant Data Dictionary

### Calibration Constants

This section lists the calibrations used by the module.  For details on calibration constants, refer to the Data Dictionary for the application.

| Constant Name |
| --- |
| k_Harmonic6thElec_Uls_f32 |
| k_Harmonic12thElec_Uls_f32 |
| k_Harmonic18thElec_Uls_f32 |
| t_MtrCurrQaxRpl_Amp_u9p7[] |
| t_MtrCurrDaxRpl_Amp_u9p7[] |
| t2_MtrTrqRpl6X_MtrNm_s2p13 |
| t2_MtrTrqRpl6Y_MtrNm_s2p13 |
| t2_MtrTrqRpl12X_MtrNm_s2p13 |
| t2_MtrTrqRpl12Y_MtrNm_s2p13 |
| t2_MtrTrqRpl18X_MtrNm_s2p13 |
| t2_MtrTrqRpl18Y_MtrNm_s2p13 |
| t_MtrVelX_MtrRadpS_T_u14p2[10] |
| t_MtrTrqCancPIMagRP_Uls_u6p10[10] |
| t_MtrTrqCancPIPhRP_Rev_u0p16[10] |
| t_MtrTrqCmdPIY_MtrNm_u5p11 [] |
| t2_MtrTrqCancPIMagRP_Uls_u6p10[] |
| t2_MtrTrqCancPIPhRP_Rev_u0p16[] |

### Program(fixed) Constants

#### Embedded Constants

All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

##### Local

| Constant Name | Resolution | Units | Value |
| --- | --- | --- | --- |
| D_SQRT3OVR2_ULS_F32 | Single precision float | Unit less | 0.866025403784 |
| D_6HARMONICNO_F32 | Single precision float | Unit less | 6 |
| D_12HARMONICNO_F32 | Single precision float | Unit less | 12 |
| D_COGGINGTBLRES_F32 | Single precision float | Counts | 81.48733 |
| D_MAXTBLVALUE_CNT_u16 | 1 | Counts | 511 |
| D_SCALERADTOCNTS_ULS_F32 | Single precision float | Unit less | 10430.3783505 |
| D_30DEGREES_CNT_U16 | 1 | Counts | 5461 |
| D_DEG2RAD_ULS_F32 | Singles precision float | Unit less | 0.0174532925199 |
| D_REVWITHROUND_ULS_F32 | Singles precision float | Unit less | 65536.5 |
| D_ONEHALF_ULS_F32 | Singles precision float | Unit less | 0.5 |
| D_POSITIVEONE_CNT_S8 | 1 | Counts | 1 |
| D_COGTRQ_LOOPLMT | 1 | Unit less | 128 |
| D_DAXRPLTBLSZ_CNT_U8 | 1 | Counts | TableSize_m(t_MtrCurrDaxRpl_Amp_u9p7) |
| D_QAXRPLTBLSZ_CNT_U8 | 1 | Counts | TableSize_m(t_MtrCurrQaxRpl_Amp_u9p7) |
| D_COGTRQRPL_LOOPLMT | 1 | Counts | 3U |
| D_NOOFHARMONIC_CNT_U8 | 1 | Counts | 9U |
| D_MINCOGRANGE_NM_S5P10 | S5P10_T | Nm | -0.1 |
| D_MINCOGRANGE_NM_S5P10 | S5P10_T | Nm | 0.1 |
| D_MINCOGRANGE_NM_S2P13 | S2P13 | Nm | FPM_InitFixedPoint_m(-0.1,s2p13_T) |
| D_MAXCOGRANGE_NM_S2P13 | S2P13 | Nm | FPM_InitFixedPoint_m(0.1,s2p13_T) |
| D_MINTRQRANGE_NM_F32 | Single precision float | Nm | (-0.5F) |
| D_MAXTRQRANGE_NM_F32 | Single precision float | Nm | (-0.5F) |

##### Global

This section lists the global constants used by the module.  For details on global constants, refer to the Data Dictionary for the application.

| Constant Name |
| --- |
| D_2PI_ULS_F32 |
| D_ONE_ULS_F32 |
| D_ZERO_ULS_F32 |

#### Module specific Lookup Tables Constants

(This is for lookup tables (arrays) with fixed values, same name as other tables)

| Constant Name | Resolution | Value | Software Segment |
| --- | --- | --- | --- |
| t_SinTbl_Cnt_u16 | Uint16 |  | TRQCANC_START_SEC_CONST_16 |

## Functions/Macros used by the Sub-Modules

### Library Functions / Macros

The library and functions / Macros that are called by the various sub modules are identified below,

1. Abs_s16_m
2. FPM_FloatToFixed_m
3. TableSize_m
4. FPM_FixedToFloat_m
5. IntplVarXY_u16_u16Xu16Y_Cnt
6. BilinearXYM_s16_u16Xs16YM_Cnt
7. sqrtf
8. atan2f
9. sinf
10. Rte_Pim_CogTrqCal
11. Rte_Pim_CogTrqRplComp
### Data Hiding Functions

MtrCntrl_Read_MtrElecPol_Cnt_s8

MtrCntrl_Read_MtrPosElec_Rev_u0p16

MtrCntrl_Read_ReadFwdPthAccessBfr_Cnt_u16

### Global Functions/Macros Defined by this Module

None

### Local Functions/Macros Used by this MDD only

## Software Module Implementation

### Runtime Environment (RTE) Initial Values

This section lists the initial values of data written by this module but controlled by the RTE. After RTE initialization, the data in this table will contain these values.

| Data | Value |
| --- | --- |

### Initialization Functions

#### Per:  TrqCanc_Init

##### Design Rationale

Update the lookup table for ripple’s

##### Processing

### Periodic Functions

#### Per:  TrqCanc_Per1

##### Design Rationale

FastDataAccessBufIndex  allows  the buffer synchronization between data calculated on slower periodic loop time(2 milli seconds)  and are  read by faster periodic run time (ie 0.125ms)

##### Program Flow Start

Rte_Call_TrqCanc_Per1_CP0_CheckpointReached()

##### Store Module Inputs to Local copies

MRFMtrVel_MtrRadpS_T_f32=Rte_IRead_TrqCanc_Per1_MRFMtrVel_MtrRadpS_f32

DaxRef_Amp_T_f32=Rte_IRead_TrqCanc_Per1_MtrCurrDaxRef_Amp_f32

QaxRef_Amp_T_f32 =Rte_IRead_TrqCanc_Per1_MtrCurrQaxRef_Amp_f32

WriteAccessBufIndex_Cnt_T_u16= (FastDataAccessBufIndex_Cnt_M_u16&1)^1

EstLq_Henry_T_f32=Rte_IRead_TrqCanc_Per1_EstLq_Henry_f32()

MtrTrqCmdMRFScl_MtrNm_T_f32 =Rte_IRead_TrqCanc_Per1_MtrTrqCmdMRFScl_MtrNm_f32()

EstLd_Henry_T_f32=Rte_IRead_TrqCanc_Per1_EstLd_Henry_f32()

EstKe_VpRadpS_T_f32 = Rte_IRead_TrqCanc_Per1_EstKe_VpRadpS_f32()

##### Store Local copy of outputs into Module Outputs

MtrTrqRpl6Mag_MtrNm_M_f32[WriteAccessBufIndex_Cnt_T_u16] =  MtrTrq6thMag_MtrNm_T_f32

MtrTrqRpl12Mag_MtrNm_M_f32[WriteAccessBufIndex_Cnt_T_u16] = MtrTrq12thMag_MtrNm_T_f32

MtrTrq6Ph_Rad_M_f32[WriteAccessBufIndex_Cnt_T_u16] =     MtrTrqRip6thPhs_Rad_T_f32

MtrTrq12Ph_Rad_M_f32[WriteAccessBufIndex_Cnt_T_u16]  =   MtrTrqRip12thPhs_Rad_T_f32

MtrTrqRpl18Mag_MtrNm_M_f32[WriteAccessBufIndex_Cnt_T_u16] =MtrTrq18thMag_MtrNm_T_f32

MtrTrq18Ph_Rad_M_f32[WriteAccessBufIndex_Cnt_T_u16] =    MtrTrqRip18thPhs_Rad_T_f32

TrqCanc_IqtoTrqMulti_VpRadpS_M_f32[WriteAccessBufIndex_Cnt_T_u16] = IqtoTrqMulti_VpRadpS_T_f32

##### Program Flow End

Rte_Call_TrqCanc_Per1_CP1_CheckpointReached()

### Periodic Functions

#### Per:  TrqCogCancRefPer1

##### Design Rationale

FastDataAccessBufIndex  allows  the buffer synchronization between data calculated on slower periodic loop time(2 milli seconds)  and are  read by faster periodic run time. SlowDataAccessBufIndex  allows  the buffer synchronization between data calculated on faster periodic loop time(125 micro seconds)  and are  read by slower periodic run time (ie 2ms)

##### Program Flow Start

N/A

##### Store Module Inputs to Local copies

DataAccessBfr_Cnt_T_u16 =FastDataAccessBufIndex_Cnt_M_u16

MtrCntrl_Read_MtrElecPol_Cnt_s8(&MtrElecPol_Cnt_T_s8)

MtrCntrl_Read_MtrPosElec_Rev_u0p16(&MtrPosElec_Rev_T_u0p16)

MtrPosComputDelay_Rad_T_f32=MtrPosComputationDelay_Rad_M_f32[DataAccessBfr_Cnt_T_u16]

EstKe_VpRadpS_T_f32= MtrEstKe_VpRadpS_M_f32[DataAccessBfr_Cnt_T_u16]

MtrTrqRpl6Mag_MtrNm_T_f32 =MtrTrqRpl6Mag_MtrNm_M_f32[DataAccessBfr_Cnt_T_u16] MtrTrqRpl12Mag_MtrNm_T_f32=MtrTrqRpl12Mag_MtrNm_M_f32[DataAccessBfr_Cnt_T_u16]

MtrTrq6Ph_Rad_T_f32  =MtrTrq6Ph_Rad_M_f32[DataAccessBfr_Cnt_T_u16]

MtrTrq12Ph_Rad_T_f32 =MtrTrq12Ph_Rad_M_f32[DataAccessBfr_Cnt_T_u16]

MtrTrqRpl18Mag_MtrNm_T_f32=MtrTrqRpl18Mag_MtrNm_M_f32[DataAccessBfr_Cnt_T_u16]

MtrTrq18Ph_Rad_T_f32  =MtrTrq18Ph_Rad_M_f32[DataAccessBfr_Cnt_T_u16]

IqtoTrqMulti_VpRadpS_T_f32 = TrqCanc_IqtoTrqMulti_VpRadpS_M_f32[DataAccessBfr_Cnt_T_u16] ;

##### Store Local copy of outputs into Module Outputs

None

##### Program Flow End

None

### Fault Recovery Functions

None

### Shutdown Functions

None

### Interrupt Functions

None

### Serial Communication Functions

#### SComm: TrqCanc_Scom_ReadCogTrqCal

##### Design Rationale

#ifdef RTE_PTR2ARRAYBASETYPE_PASSING

FUNC(void, RTE_AP_TRQCANC_APPL_CODE) TrqCanc_Scom_ReadCogTrqCal(P2VAR(UInt16, AUTOMATIC, RTE_AP_TRQCANC_APPL_VAR) CogTrqCalPtr, UInt16 ID)

#else

FUNC(void, RTE_AP_TRQCANC_APPL_CODE) TrqCanc_Scom_ReadCogTrqCal(P2VAR(CoggingCancTrq, AUTOMATIC, RTE_AP_TRQCANC_APPL_VAR) CogTrqCalPtr, UInt16 ID)

#endif

##### Program Flow Start

None

##### Store Module Inputs to Local copies

None

##### Processing

##### Store Local copy of outputs into Module Outputs

None

**Program Flow End**

None

#### SComm: TrqCanc_Scom_SetCogTrqCal

##### Design Rationale

| **Function Name** | CoggingTrqTableUpdate | Type | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | *******CogTrqCalPtr** | Sint16 | -1 | 1 |  |
|  | **ID** | Unit16 | 0 | 4 |  |
| **Return Value** | None |  |  |  |  |

##### #ifdef RTE_PTR2ARRAYBASETYPE_PASSING

##### FUNC(void, RTE_AP_TRQCANC_APPL_CODE) TrqCanc_Scom_SetCogTrqCal(P2CONST(UInt16, AUTOMATIC, RTE_AP_TRQCANC_APPL_DATA) CogTrqCalPtr, UInt16 ID)

##### #else

##### FUNC(void, RTE_AP_TRQCANC_APPL_CODE) TrqCanc_Scom_SetCogTrqCal(P2CONST(CoggingCancTrq, AUTOMATIC, RTE_AP_TRQCANC_APPL_DATA) CogTrqCalPtr, UInt16 ID)

#endif

##### Program Flow Start

None

##### Store Module Inputs to Local copies

None

##### Processing

##### Store Local copy of outputs into Module Outputs

None

##### Program Flow End

None

### Local Function/Macro Definitions

#### CoggingTrqTableUpdate#1

| **Function Name** | CoggingTrqTableUpdate | Type | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | N/A | N/A | - | - |  |
| **Return Value** | N/A | N/A | N/A | N/A |  |

##### Description

#### SinLookup #2

| **Function Name** | SinLookup | Type | Min | Max | UTP Tol. |
| --- | --- | --- | --- | --- | --- |
| **Arguments Passed ** | Theta_Rad_T_f32 | Float32 | --2*pi | 2*pi |  |
| **Return Value** | Result_Uls_T_f32 | Float32 | -1 | 1 |  |

##### Description

## Execution Requirements

### Execution Sequence of the Module

(Describe in words relevant details about the execution sequence of the different sub modules.)

### Execution Rates for sub-modules called by the Scheduler

This table serves as reference for the Scheduler design

| Function Name | Calling Frequency | System State(s) in which the function is called |
| --- | --- | --- |
| TrqCanc_Per1 | 2ms | ALL |
| TrqCogCancRefPer1 | 125us | ALL |
| TrqCanc_Init | Init | At Startup |

### Execution Requirements for Serial Communication Functions

| Function Name | Sub-Module called by (Serial Comm Function Name) |
| --- | --- |
| TrqCanc_Scom_ReadCogTrqCal | EPS_DiagSrvc |
| TrqCanc_Scom_SetCogTrqCal | EPS_DiagSrvc |

## Memory Map Definition Requirements

### Sub Modules (Functions)

This table identifies the software segments for functions identified in this module.

| Name of Sub Module | Software Segment |
| --- | --- |
| TrqCanc_Per1 | RTE_START_SEC_AP_TRQCANC_APPL_CODE |
| TrqCanc_Init | RTE_START_SEC_AP_TRQCANC_APPL_CODE |

### Local Functions

This table identifies the software segments for local functions identified in this module.

| Name of Sub Module | Software Segment |
| --- | --- |
| CoggingTrqTableUpdate | RTE_START_SEC_AP_TRQCANC_APPL_CODE |
| SinLookup | RTE_START_SEC_AP_TRQCANC_APPL_CODE |

## Known Issues / Limitations With Design

Note for UNIT  TEST:

1. Rte_Pim_CogTrqCal  and CogTrqRplComp is declared as unit16 with size of 521  with 512 values are used in the look up and 9 values are used in the harmonic table compensation.
Eventhough the values are read as uint16 it will be used as sint16 ( s5p10 preciously) with the range of -1 to 1 .

## Revision Control Log

| **Rev #** | **Change Description** | **Date ** | **Author Initials** |
| --- | --- | --- | --- |
| 1.0 | Initial version (v8 FDD SF99B) | 23-Mar-13 | Selva |
| 2 | Updated to version 9 FDD SF99B | 5-June-13 | Selva |
| 3 | Updated to version 10 FDD SF99B | 21-Oct-13 | Selva |
| 4 | Updated to version 10 FDD SF99B | 23-Oct-13 | Selva |
| 5 | Updated to version 11 FDD SF99B | 7-Nov-13 | Selva |
| 6 | Updated to version 15 FDD SF99B | 23-Mar-15 | Selva |
| 7 | Updated to version 16 FDD SF99B | 23-Apr-15 | Selva |
