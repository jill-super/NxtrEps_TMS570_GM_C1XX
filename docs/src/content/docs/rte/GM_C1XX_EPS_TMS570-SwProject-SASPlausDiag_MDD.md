---
title: "Integration — doc/SASPlausDiag_MDD"
description: "Converted document SASPlausDiag_MDD.docx."
---

> **Converted document.** Source: `GM_C1XX_EPS_TMS570/SwProject/SASPlausDiag/doc/SASPlausDiag_MDD.docx`.

## Module – SASPlausDiag

## High-Level Description

This module performs a cross check of Digital Column Position’s output handwheel position to Vehicle Dynamics’ output handwheel position one time after both signals become valid.

## Figures

### Component Diagram

## Variable Data Dictionary

For details on module input / output variable, refer to the Data Dictionary for the application.  Input / output variable names are listed here for reference.

### Module Internal Variables

This section identifies the name, range and resolutions for module specific data created by this module.  If there are no range restrictions on the variable, the term “FULL” is placed into the table for legal range.

#### User defined typedef definition/declaration

This section documents any user types uniquely used for the module.

## Constant Data Dictionary

### Calibration Constants

This section lists the calibrations used by the module.  For details on calibration constants, refer to the Data Dictionary for the application.

### Program(fixed) Constants

#### Embedded Constants

All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

##### Local

##### Global

This section lists the global constants used by the module.  For details on global constants, refer to the Data Dictionary for the application.

#### Module specific Lookup Tables Constants

## Functions/Macros used by the Sub-Modules

### Library Functions / Macros

The library and functions / Macros that are called by the various sub modules are identified below,

Abs_f32_m

### Data Hiding Functions

None

### Global Functions/Macros Defined by this Module

None

### Local Functions/Macros Used by this MDD only

None

## Software Module Implementation

### Runtime Environment (RTE) Initial Values

This section lists the initial values of data written by this module but controlled by the RTE. After RTE initialization, the data in this table will contain these values.

### Initialization Functions

None

### Periodic Functions

#### Per: SASPlausDiag_Per1

##### Design Rationale

None

##### Program Flow Start

None

##### Store Module Inputs to Local copies

I2CHwPosValid_Cnt_T_lgc = Rte_IRead_SASPlausDiag_Per1_I2CHwAbsPosValid_Cnt_lgc()

I2CHwPos_HwDeg_T_f32 = Rte_IRead_SASPlausDiag_Per1_I2CHwAbsPos_HwDeg_f32()

VdAuthority_Uls_T_f32 = Rte_IRead_SASPlausDiag_Per1_VdAuthority_Uls_f32()

VdHwPos_HwDeg_T_f32 = Rte_IRead_SASPlausDiag_Per1_VdHwPos_HwDeg_f32()

##### Description

##### Store Local copy of outputs into Module Outputs

None

##### Program Flow End

None

### Shutdown Functions

None

### Interrupt Functions

None

### Serial Communication Functions

None

## Execution Requirements

### Execution Rates for sub-modules called by the Scheduler

This table serves as reference for the Scheduler design

### Execution Requirements for Serial Communication Functions

## Memory Map Definition Requirements

### Sub Modules (Functions)

This table identifies the software segments for functions identified in this module.

### Local Functions

This table identifies the software segments for local functions identified in this module.

## Known Issues / Limitations With Design

INLINE functions defined in GlobalMacro.h are not unit tested.Revision Control Log



| Module Inputs | Module Outputs | Module Outputs |

| --- | --- | --- |

| I2CHwAbsPosValid_Cnt_lgc | I2CHwAbsPosValid_Cnt_lgc | None |

| I2CHwAbsPos_HwDeg_f32 | I2CHwAbsPos_HwDeg_f32 |  |

| VdAuthority_Uls_f32 | VdAuthority_Uls_f32 |  |

| VdHwPos_HwDeg_f32 | VdHwPos_HwDeg_f32 |  |





| Variable Name | Resolution | Legal Range<br/>(min) | Legal Range<br/>(max) | Software Segment |

| --- | --- | --- | --- | --- |

| SASPlausDiag_TestExecuted_Cnt_M_lgc | 1 | FALSE | TRUE | SASPLAUSDIAG_START_VAR_CLEARED_BOOLEAN |





| Typedef Name | Element Name | User Defined Type | Legal Range<br/>(min) | Legal Range<br/>(max) |

| --- | --- | --- | --- | --- |

| None |  |  |  |  |





| Constant Name |

| --- |

| k_SASPlausDiagMaxDelta_HwDeg_f32 |





| Constant Name | Resolution | Units | Value |

| --- | --- | --- | --- |

| None |  |  |  |





| Constant Name |

| --- |

| None |





| Constant Name | Resolution | Value | Software Segment |

| --- | --- | --- | --- |

| None |  |  |  |





| Data | Value |

| --- | --- |

| Rte_InitValue_I2CHwAbsPos_HwDeg_f32 | 0 |

| Rte_InitValue_I2CHwAbsPosValid_Cnt_lgc | FALSE |

| Rte_InitValue_VdAuthority_Uls_f32 | 0 |

| Rte_InitValue_VdHwPos_HwDeg_f32 | 0 |





| Function Name | Calling Frequency | System State(s) in which the function is called |

| --- | --- | --- |

| SASPlausDiag_Per1 | 2 ms | ALL |





| Function Name | Sub-Module called by (Serial Comm Function Name) |

| --- | --- |

| None |  |





| Name of Sub Module | Software Segment |

| --- | --- |

| VehDyn_Per1 | RTE_START_SEC_AP_VEHDYN_APPL_CODE |





| Name of Sub Module | Software Segment |

| --- | --- |

| None |  |





| Rev # | Change Description | Date | Author Initials |

| --- | --- | --- | --- |

| 1.0 | Initial Version | 31-Mar-15 | JWJ |



> Figures not embeddable on the web (word/media/image1.emf (.emf)) are preserved in the original document.
