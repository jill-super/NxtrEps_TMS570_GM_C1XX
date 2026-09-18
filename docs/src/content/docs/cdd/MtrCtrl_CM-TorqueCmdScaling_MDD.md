---
title: "MtrCtrl_CM — TorqueCmdScaling_MDD"
description: "Converted .doc document from MtrCtrl_CM/doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/MtrCtrl_CM/doc/TorqueCmdScaling_MDD.doc`.

- Module -- Torque Command Scaling

- DOCVARIABLE "MDDRevNum" \* MERGEFORMAT

- High-Level Description

- The Torque Command Scale module multiplies the Torque_Command_MRF input signal by a calibration which is set during a manufacturing EOL calibration process. This calibration is provided to reduce overall system output torque variation. This scaled version of the torque command is used by all other sub functions within motor control which have a torque dependent component.

- Function Data Sharing

- This diagram shows all data that is shared between functions within the module.

- Function (Name)

- This diagram describes the functional characteristics and data flow of a given function.

- This is not mandatory, only used where a graphical representation helps explain the function. It is left to the author

- s discretion. New headers of this level (Level 3) should be created for each function.

- Variable Data Dictionary

- For details on module input / output variable, refer to the Data Dictionary for the application. Input / output variable names are listed here for reference.

- (Note: Full variable names required in table.)

- (Note: All global variables including End Of Line data used should be shown here)

- Module Inputs (Global Variable Name)

- Module Outputs (Global Variable Name)

- MRFMtrTrqCmd_MtrNm_f32

- MRFMtrTrqCmdScl_MtrNm_f32

- Module Internal Variables

- This section identifies the name, range and resolutions for module specific data created by this module. If there are no range restrictions on the variable, the term

- is placed into the table for legal range.

- Variable Name

- Software Segment

- User defined typedef definition/declaration

- This section documents any user types uniquely used for the module.

- Typedef Name

- Element Name

- User Defined Type

- Constant Data Dictionary

- Calibration Constants

- This section lists the calibrations used by the module. For details on calibration constants, refer to the Data Dictionary for the application.

- Constant Name

- k_MinTrqCmdScl_Uls_f32

- k_MaxTrqCmdScl_Uls_f32

- TorqueCmdSF_Uls_f32 (NVM)

- Program(fixed) Constants

- Embedded Constants

- All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

- This section lists the global constants used by the module. For details on global constants, refer to the Data Dictionary for the application.

- Module specific Lookup Tables Constants

- (This is for lookup tables (arrays) with fixed values, same name as other tables)

- Functions/Macros used by the Sub-Modules

- Library Functions / Macros

- The library functions / Macros that are called by the various sub modules are identified below,

- Data Hiding Functions

- The data hiding functions / macros used in this module are identified below,

- Rte_Call_TrqCmdScl_WriteBlock()

- Rte_Pim_TorqueCmdSF_Uls_f32()

- Local Functions/Macros Used by this MDD only

- (Note if they are defined in another source file, then reference the appropriate header file)

- The local functions/macros in this module are identified below,

- Software Module Implementation

- Periodic Functions

- Per: TrqCmdScl_Per1

- Design Rationale

- Program Flow Start

- Rte_Call_TrqCmdScl_Per1_CP0_CheckpointReached()

- Store Module Inputs to Local copies

- MRFMtrTrqCmd_MtrNm_T_f32 = Rte_IRead_TrqCmdScl_Per1_MRFMtrTrqCmd_MtrNm_f32()

- TorqueCmdSF_Uls_T_f32 = *Rte_Pim_TorqueCmdSF_Uls_f32()

- Apply Torque Command Scaling

- EMBED Visio.Drawing.11

- Store Local copy of outputs into Module Outputs

- Rte_IWrite_TrqCmdScl_Per1_MRFMtrTrqCmdScl_MtrNm_f32(MRFMtrTrqCmdScl_MtrNm_T_f32)

- Program Flow End

- Rte_Call_TrqCmdScl_Per1_CP1_CheckpointReached()

- Scomm: TrqCmdScl_SCom_Get

- Get Torque Command Scaling

- Scomm: TrqCmdScl_SCom_Set

- Set Torque Command Scaling

- Local Function/Macro Definitions

- If these are numerous and defined in a separate source file then reference the source file only.

- Function Name

- Arguments Passed

- Return Value

- Execution Requirements

- Execution Sequence of the Module

- TrqCmdScl_Per1 must be executed in the forward path before quadrant detection, the voltage command numerator, phase advance, voltage command denominator, and Modulation Index.

- Execution Rates for sub-modules called by the Scheduler

- This table serves as reference for the Scheduler design

- Calling Frequency

- System State(s)

- TrqCmdScl_Per1

- Execution Requirements for Serial Communication Functions

- Sub-Module called by (Serial Comm Function Name)

- TrqCmdScl_Scom_Get()

- TrqCmdScl_Scom_Set()

- Memory Map Definition Requirements

- Sub Modules (Functions)

- This table identifies the software segments for functions identified in this module.

- Name of Sub Module

- Local Functions

- This table identifies the software segments for local functions identified in this module.

- Known Issues / Limitations With Design

- Revision Control Log

- Change Description

- Author Initials

- Document creation and initial release for the component

- Corrections to assign EOL scaling factor to temporary variable

- Added checkpoints and memmap software segment is updated for static variables

- Heading and format corrected

- SOFTWARE MODULE DESIGN SPECIFICATION

- Hand Wheel Torque

- DOCPROPERTY "Product Line" \* MERGEFORMAT

- 2620-SepNov-2012

- Selva Sengottaiyan

- DOCPROPERTY "Company" \* MERGEFORMAT

- CONFIDENTIAL

- S/W module design template, Rev 2.2b
