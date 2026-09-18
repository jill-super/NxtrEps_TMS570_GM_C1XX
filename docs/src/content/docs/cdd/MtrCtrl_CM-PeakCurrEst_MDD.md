---
title: "MtrCtrl_CM — PeakCurrEst_MDD"
description: "Converted .docx document from MtrCtrl_CM/doc."
---

> **Converted document.** Source: `MtrCtrl_CM/doc/PeakCurrEst_MDD.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

## Module – PeakCurrEst

## High-Level Description

## Figures

### Component Diagram

![figure](../../../assets/converted/MtrCtrl_CM/PeakCurrEst_MDD-fig4.png)

![figure](../../../assets/converted/MtrCtrl_CM/PeakCurrEst_MDD-fig3.png)

### Variable Data Dictionary

For details on module input / output variable, refer to the Data Dictionary for the application.  Input / output variable names are listed here for reference.

| Module Inputs | Module Outputs | Module Outputs |
| --- | --- | --- |

### Module Internal Variables

This section identifies the name, range and resolutions for module specific data created by this module.  If there are no range restrictions on the variable, the term “FULL” is placed into the table for legal range.

| Variable Name | Resolution | Legal Range | Legal Range | Software Segment |
| --- | --- | --- | --- | --- |

#### User defined typedef definition/declaration

This section documents any user types uniquely used for the module.

| Typedef Name | Element Name | User Defined Type | Legal Range | Legal Range |
| --- | --- | --- | --- | --- |
| None |  |  |  |  |

## Constant Data Dictionary

### Calibration Constants

This section lists the calibrations used by the module.  For details on calibration constants, refer to the Data Dictionary for the application.

| Constant Name |
| --- |
| k_EstPkCurr2msLPFKn_Uls_u16 |
| k_EstPkCurrSlowLoopLPFKn_Uls_u16 |

### Program(fixed) Constants

#### Embedded Constants

All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

##### Local

| Constant Name | Resolution | Units | Value |
| --- | --- | --- | --- |
| None |  |  |  |

##### Global

This section lists the global constants used by the module.  For details on global constants, refer to the Data Dictionary for the application.

| Constant Name |
| --- |
| D_ESTPKCURRLOLMT_AMPSQ_F32 |
| D_ESTPKCURRHILMT_AMPSQ_F32 |

#### Module specific Lookup Tables Constants

| Constant Name | Resolution | Value | Software Segment |
| --- | --- | --- | --- |
| None |  |  |  |

## Functions/Macros used by the Sub-Modules

### Library Functions / Macros

The library and functions / Macros that are called by the various sub modules are identified below,

1. LPF_SvUpdate_u16InFixKTrunc_m
2. LPF_OpUpdate_u16InFixKTrunc_m
3. LPF_SvUpdate_s16InFixKTrunc_m
4. LPF_OpUpdate_s16InFixKTrunc_m
5. FPM_FloatToFixed_m
6. FPM_FixedToFloat_m
7. Limit_m
### Data Hiding Functions

1. None
### Global Functions/Macros Defined by this Module

None

### Local Functions/Macros Used by this MDD only

None

## Software Module Implementation

### Runtime Environment (RTE) Initial Values

None

### Initialization Functions

None

### Periodic Functions

#### Per: PeakCurrEst_Per1

##### Design Rationale

None

##### Program Flow Start

Rte_Call_PeakCurrEst_Per1_CP0_CheckpointReached

##### Store Module Inputs to Local copies

##### Module Design

##### Store Local copy of outputs into Module Outputs

Rte_IWrite_PeakCurrEst_Per1_EstPkCurr_AmpSq_f32(EstPkCurr_AmpSq_T_f32)

##### Program Flow End

Rte_Call_PeakCurrEst_Per1_CP1_CheckpointReached

#### Per: PeakCurrEst_Per2

##### Design Rationale

##### Program Flow Start

Rte_Call_PeakCurrEst_Per2_CP0_CheckpointReached()

##### Module Design

##### Store Local copy of outputs into Module Outputs

Rte_IWrite_PeakCurrEst_Per2_FiltEstPkCurr_AmpSq_f32(FiltEstPkCurr_AmpSq_T_f32)

##### Program Flow End

##### Rte_Call_PeakCurrEst_Per2_CP1_CheckpointReached()

### Fault Recovery Functions

None

### Shutdown Functions

None

### Interrupt Functions

None

### Serial Communication Functions

None

## Execution Requirements

### Execution Sequence of the Module

### Execution Rates for sub-modules called by the Scheduler

This table serves as reference for the Scheduler design

| Function Name | Calling Frequency | System State(s) in which the function is called |
| --- | --- | --- |
| PeakCurrEst_Per1 | 2ms | OFF,DISABLE,OPERATE |
| PeakCurrEst_Per2 | 100ms | OFF,DISABLE,OPERATE |

### Execution Requirements for Serial Communication Functions

| Function Name | Sub-Module called by (Serial Comm Function Name) |
| --- | --- |

## Memory Map Definition Requirements

### Sub Modules (Functions)

This table identifies the software segments for functions identified in this module.

| Name of Sub Module | Software Segment |
| --- | --- |
| PeakCurrEst_Per1 | RTE_AP_PEAKCURREST_APPL_CODE |
| PeakCurrEst_Per2 | RTE_AP_PEAKCURREST_APPL_CODE |

### Local Functions

This table identifies the software segments for local functions identified in this module.

| Name of Sub Module | Software Segment |
| --- | --- |

## Known Issues / Limitations With Design

1. INLINE functions defined in GlobalMacro.h are not unit tested.
## Revision Control Log

| **Item #** | **Rev #** | **Change Description** | **Date ** | **Author Initials** |
| --- | --- | --- | --- | --- |
| 1 | 1.0 | Initial Version | 5/15/2012 | KPIT-RD |
| 2 | 2.0 | Addition of checkpoints and memmap statements | 20-Nov-12 | Selva |
| 3 | 3.0 | Updated to version 8 FDD SF99 B | 20-Mar-1 | Selva |
