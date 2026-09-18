---
title: "MtrVel_Digi — MotorVelocity3_MDD"
description: "Converted .doc document from MtrVel_Digi/doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/MtrVel_Digi/doc/MotorVelocity3_MDD.doc`.

- Module -- Motor Velocity

- High-Level Description

- Function Data Sharing

- This diagram shows all data that is shared between functions within the module.

- No Shared Data

- Variable Data Dictionary

- For details on module input / output variable, refer to the Data Dictionary for the application. Input / output variable names are listed here for reference.

- (Note: Full variable names required in table.)

- (Note: All global variables including End Of Line data used should be shown here)

- Module Inputs (Global Variable Name)

- Module Outputs (Global Variable Name)

- MechMtrPos1_Rev_u0p16

- MechMtrPos1SampleTTimeStamp1_uS_u32

- Module Internal Variables

- This section identifies the name, range and resolutions for module specific data created by this module. If there are no range restrictions on the variable, the term

- is placed into the table for legal range.

- Variable Name

- Software Segment

- MtrVel3_PosBuffer_Rad_M_u0p16f32

- MTRVEL3_START_SEC_VAR_CLEARED_1632

- MtrVel3_TimeBuffer_uS_M_u16p0

- MTRVEL3_START_SEC_VAR_CLEARED_16

- MtrVel3_OsBufPos_Cnt_M_u08

- MTRVEL3_START_SEC_VAR_CLEARED_8

- * Note: These ranges are based on the range of the normalized sine and cosine global inputs, which in turn are based on the maximum amount of signal variation that can be caused by temperature changes on the MSB signals.

- User defined typedef definition/declaration

- This section documents any user types uniquely used for the module.

- Typedef Name

- Element Name

- User Defined Type

- Constant Data Dictionary

- Calibration Constants

- This section lists the calibrations used by the module. For details on calibration constants, refer to the Data Dictionary for the application.

- Constant Name

- Program(fixed) Constants

- Embedded Constants

- All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

- D_BUFFERMASK_CNT_U08

- D_MTRVELOSBUFSZ_CNT_U08 - 1

- This section lists the global constants used by the module. For details on global constants, refer to the Data Dictionary for the application.

- Module specific Lookup Tables Constants

- (This is for lookup tables (arrays) with fixed values, same name as other tables)

- Functions/Macros used by the Sub-Modules

- Library Functions / Macros

- The library functions / Macros that are called by the various sub modules are identified below,

- Data Hiding Functions

- The data hiding functions / macros used in this module are identified below,

- Local Functions/Macros Used by this MDD only

- (Note if they are defined in another source file, then reference the appropriate header file)

- The local functions/macros in this module are identified below,

- Software Module Implementation

- Initialization Functions

- Init: MtrVel3_Init1

- Design Rationale

- Module Outputs

- Module Internal

- MtrVel_Read_MechMtrPos1_Rev_u0p16(&MtrPos_MechMtrPos_Rev_T_u0p16)

- MtrVel_Read_MechMtrPos1SampleTime_uS_u32(&MtrPos_SampleTime_uS_T_u32) MtrVel_Read_SampleTime1_uS_u32(&MtrPos_SampleTime_uS_T_u32);

- MtrVel_PosBuffer_Rad_T_f32 =(FPM_FixedToFloat_m(MtrPos_MechMtrPos_Rev_T_u0p16, u0p16_T))*D_2PI_ULS_F32

- EMBED Visio.Drawing.11

- Periodic Functions

- Per: MtrVel3_Per1

- Program Flow Start

- Store Module Inputs to Local copies

- MtrVel_Read_MechMtrPos1_Rev_u0p16 MtrVel_Read_MechMtrPos1_Rev_u0p16(&MtrPos_MechMtrPos_Rev_T_u0p16);

- MtrVel_Read_MechMtrPos1TimeStamp_uS_u32 MtrVel_Read_SampleTime1_uS_u32(&MtrPos_SampleTime_uS_T_u32);

- Populate Sample Buffers

- Store Local copy of outputs into Module Outputs

- Program Flow End

- Fault Recovery Functions

- Shutdown Functions

- Interrupt Functions

- Serial Communication Functions

- Local Function/Macro Definitions

- If these are numerous and defined in a separate source file then reference the source file only.

- Execution Requirements

- Execution Sequence of the Module

- (Describe in words relevant details about the execution sequence of the different sub modules.)

- Execution Rates for sub-modules called by the Scheduler

- This table serves as reference for the Scheduler design

- Function Name

- Calling Frequency

- System State(s) in which the function is called

- MtrVel3_Init1

- MtrVel3_Per1

- Motor Control ISR

- Execution Requirements for Serial Communication Functions

- Sub-Module called by (Serial Comm Function Name)

- Memory Map Definition Requirements

- Sub Modules (Functions)

- This table identifies the software segments for functions identified in this module.

- Name of Sub Module

- RTE_SA_MTRVEL3_APPL_CODE

- Known Issues / Limitations With Design

- The range limits are not applied to task running at Motor Control ISR. As the limiting adds few more instruction cycles, the ranges for those variables should be applied at 2ms N/A

- Revision Control Log

- Change Description

- Author Initials

- Initial release for FDD v01

- Updated the Port name from Motor Pos to Motor Velocity

- Updated Port interface name to match the FDD

- SOFTWARE MODULE DESIGN SPECIFICATION

- Motor Velocity 3

- DOCPROPERTY "Product Line" \* MERGEFORMAT

- 223-JuneAug-13

- NEXTEER CONFIDENTIAL

- S/W module design template, Rev 3.1b

- {le]YNF]B;7;B7

- zvzvzvzvqmiem]m]Y]m
