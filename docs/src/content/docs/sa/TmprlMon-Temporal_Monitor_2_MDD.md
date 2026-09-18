---
title: "TmprlMon — Temporal_Monitor_2_MDD"
description: "Converted .docx document from TmprlMon/doc."
---

> **Converted document.** Source: `TmprlMon/doc/Temporal_Monitor_2_MDD.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

## Module --

## High-Level Description

This module helps ensure valid execution time for the forward path.  It generates the falling edge of the monitor signal used by an external processor to determine execution time.

## Figures

### Component Diagram

> **Figure not rendered:** `Temporal_Monitor_2_MDD-fig1.emf` is a Windows vector image (EMF/WMF) embedded in the original Word document and cannot be displayed in a browser. See the source `.docx` file for the diagram.

## Variable Data Dictionary

For details on module input / output variable, refer to the Data Dictionary for the application.  Input / output variable names are listed here for reference.

| Module Inputs | Module Outputs | Module Outputs |
| --- | --- | --- |
| <None> | <None> |  |

### Module Internal Variables

This section identifies the name, range and resolutions for module specific data created by this module.  If there are no range restrictions on the variable, the term “FULL” is placed into the table for legal range.

| Variable Name | Resolution | Legal Range | Legal Range | Software Segment |
| --- | --- | --- | --- | --- |
| <None> |  |  |  |  |

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
| <None> |

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
| STD_LOW |
| STD_HIGH |

#### Module specific Lookup Tables Constants

| Constant Name | Value | Software Segment |
| --- | --- | --- |
| <None> |  |  |

## Functions/Macros used by the Sub-Modules

### Library Functions / Macros

The library and functions / Macros that are called by the various sub modules are identified below,

1. <None>
### Data Hiding Functions

1. <None>
### Global Functions/Macros Defined by this Module

None

### Local Functions/Macros Used by this MDD only

None

## Software Module Implementation

### Runtime Environment (RTE) Initial Values

This section lists the initial values of data written by this module but controlled by the RTE. After RTE initialization, the data in this table will contain these values.

| Data | Value |
| --- | --- |
| <None> |  |

### Initialization Functions

None

### Periodic Functions

#### Per: _Per1

##### Design Rationale

This function generates the falling edge of the WdMonitor signal.  ***It must be mapped ******at the end of****** the forward path***.

##### Program Flow Start

Rte_Call_TmprlMon2_Per1_CP0_CheckpointReached()

##### Store Module Inputs to Local copies

None

##### Set WdMonitor Low

##### Store Local copy of outputs into Module Outputs

None

##### Program Flow End

Rte_Call_TmprlMon2_Per1_CP1_CheckpointReached()

## Execution Requirements

### Execution Sequence of the Module

_Per1 is executed at the end of the forward path.

### Execution Rates for sub-modules called by the Scheduler

This table serves as reference for the Scheduler design

| Function Name | Calling Frequency | System State(s) in which the function is called |
| --- | --- | --- |
| _Per1 | 2 ms | ALL |

### Execution Requirements for Serial Communication Functions

| Function Name | Sub-Module called by (Serial Comm Function Name) |
| --- | --- |
| <None> |  |

## Memory Map Definition Requirements

### Sub Modules (Functions)

This table identifies the software segments for functions identified in this module.

| Name of Sub Module | Software Segment |
| --- | --- |
| _Per1 | RTE_START_SEC_SA_TMPRLMON_APPL_CODE |

### Local Functions

This table identifies the software segments for local functions identified in this module.

| Name of Sub Module | Software Segment |
| --- | --- |

## Known Issues / Limitations With Design

1. None
## Revision Control Log

| **Item #** | **Rev #** | **Change Description** | **Date ** | **Author Initials** |
| --- | --- | --- | --- | --- |
| 1 | 1.0 | Initial MDD | 12-Nov-12 | JJW |
