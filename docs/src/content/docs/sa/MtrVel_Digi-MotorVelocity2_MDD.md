---
title: "MtrVel_Digi — MotorVelocity2_MDD"
description: "Converted .doc document from MtrVel_Digi/doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/MtrVel_Digi/doc/MotorVelocity2_MDD.doc`.

- Module -- Motor Velocity

- High-Level Description

- Function Data Sharing

- This diagram shows all data that is shared between functions within the module.

- No Shared Data

- This diagram describes the functional characteristics and data flow of a given function.

- Variable Data Dictionary

- For details on module input / output variable, refer to the Data Dictionary for the application. Input / output variable names are listed here for reference.

- (Note: Full variable names required in table.)

- (Note: All global variables including End Of Line data used should be shown here)

- Module Inputs (Global Variable Name)

- Module Outputs (Global Variable Name)

- AsstAssemblyPolarity _Cnt_s08

- SysCDiagMtrVelMRF_MtrRadpS_f32

- HandwheelVel_HwRadpS_f32

- SysCDiagHwVel_HwRadpS_f32

- MotorVelMRF_MtrRadpS_f32

- CumMechMtrPosMRF_Deg_f32

- MechMtrPos1Timestamp _uS_u32

- Module Internal Variables

- This section identifies the name, range and resolutions for module specific data created by this module. If there are no range restrictions on the variable, the term

- is placed into the table for legal range.

- Variable Name

- Software Segment

- MtrVel2_SysCMtrVelMRF_MtrRadpS_M_f32

- Single Precision Floating Point

- MTRVEL2_START_SEC_VAR_CLEARED_32

- MtrVel2_SysCHwVelCRF_HwRadpS_M_f32

- MtrVel2_SysCMtrVelDiffAcc_Cnt_M_u16

- MTRVEL2_START_SEC_VAR_CLEARED_16

- MtrVel2_SysCHwVelDiffAcc_Cnt_M_u16

- MtrVel2_SysCMtrVelCorrLimDiff_MtrRadpS_D_f32

- MtrVel2_SysCHwVelCorrLimDiff_HwRadpS_D_f32

- * Note: These ranges are based on the range of the normalized sine and cosine global inputs, which in turn are based on the maximum amount of signal variation that can be caused by temperature changes on the MSB signals.

- User defined typedef definition/declaration

- This section documents any user types uniquely used for the module.

- Typedef Name

- Element Name

- User Defined Type

- (Name given for the user defined typdef of type struct/union)

- (Variable name qualified similar to all other variables)

- as other variables

- Constant Data Dictionary

- Calibration Constants

- This section lists the calibrations used by the module. For details on calibration constants, refer to the Data Dictionary for the application.

- Constant Name

- k_GearRatio_Uls_f32

- k_MtrVelCorrLim_Cnt_Str

- k_HwVelCorrLim_Cnt_Str

- k_MtrVelCorrLim_MtrRadpS_f32

- k_HwVelCorrLim_HwRadpS_f32

- Program(fixed) Constants

- Embedded Constants

- All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

- D_MICROSECTOSEC_f32

- Single Precision float

- D_MAXHANDWHEELVEL_HWRADPS_F32

- D_MINHANDWHEELVEL_HWRADPS_F32

- This section lists the global constants used by the module. For details on global constants, refer to the Data Dictionary for the application.

- D_MSECPERSEC_ULS_F32

- D_RADPERREV_ULS_F32

- Module specific Lookup Tables Constants

- (This is for lookup tables (arrays) with fixed values, same name as other tables)

- Functions/Macros used by the Sub-Modules

- Library Functions / Macros

- The library functions / Macros that are called by the various sub modules are identified below,

- LPF_OpUpdate_f32_m ()

- LPF_KUpdate_f32_m

- Data Hiding Functions

- The data hiding functions / macros used in this module are identified below,

- Local Functions/Macros Used by this MDD only

- (Note if they are defined in another source file, then reference the appropriate header file)

- The local functions/macros in this module are identified below,

- Software Module Implementation

- Initialization Functions

- Init: MtrVel2_Init1

- Design Rationale

- Module Outputs

- Module Internal

- CumMtrPosMRF_Deg_T_f32= Rte_IRead_MtrVel2_Init_CumMechMtrPosMRF_Deg_f32()

- SysCDiagCumMtrPos_Rad_T_f32 = (CumMtrPosMRF_Deg_T_f32) * D_PIOVR180_ULS_F32;

- PrevSysCDiagCumMtrPos_Rad_M_f32 = SysCDiagCumMtrPos_Rad_T_f32;

- Periodic Functions

- Per: MtrVel2_Per1

- Program Flow Start

- Rte_Call_MtrVel2_Per1_CP0_CheckpointReached()

- Store Module Inputs to Local copies

- AsstAssemPol_Cnt_T_s8 = Rte_IRead_MtrVel2_Per1_AsstAssemblyPolarity_Cnt_s08();

- MechMtrPosTimeStamp_uSec_T_u32 = Rte_IRead_MtrVel2_Per1_MechMtrPos1Timestamp_USec_u32();

- CumMtrPosMRF_Deg_T_f32 = Rte_IRead_MtrVel2_Per1_CumMechMtrPosMRF_Deg_f32();

- Calculate SysC Motor Velocity

- EMBED Visio.Drawing.11

- Store Local copy of outputs into Module Outputs

- Rte_IWrite_MtrVel2_Per1_SysCDiagHandwheelVel_HwRadpS_f32 (SysCHwVelCRF_HwRadpS_M_f32)

- Rte_IWrite_MtrVel2_Per1_SysCDiagMtrVelMRF_MtrRadpS_f32(SysCMtrVelRawMRF_MtrRadpS_T_f32)

- MtrVel2_SysCMtrVelMRF_MtrRadpS_M_f32 = SysCMtrVelRawMRF_MtrRadpS_T_f32 ;

- Program Flow End

- Rte_Call_MtrVel2_Per1_CP1_CheckpointReached()

- Per: MtrVel2_Per2

- Rte_Call_MtrVel2_Per2_CP0_CheckpointReached()

- HandwheelVel_HwRadpS_T_f32 = Rte_IRead_MtrVel2_Per2_HandwheelVel_HwRadpS_f32 ()

- MRFMotorVel_MtrRadpS_T_f32 = Rte_IRead_MtrVel2_Per2_MotorVelMRF_MtrRadpS_f32 ()

- Calculate Raw Motor Velocity

- Rte_Call_MtrVel2_Per2_CP1_CheckpointReached()

- Fault Recovery Functions

- Shutdown Functions

- Interrupt Functions

- Serial Communication Functions

- Local Function/Macro Definitions

- Execution Requirements

- Execution Sequence of the Module

- (Describe in words relevant details about the execution sequence of the different sub modules.)

- Execution Rates for sub-modules called by the Scheduler

- This table serves as reference for the Scheduler design

- Function Name

- Calling Frequency

- System State(s) in which the function is called

- MtrVel2_Init1

- MtrVel2_Per1

- MtrVel2_Per2

- Execution Requirements for Serial Communication Functions

- Sub-Module called by (Serial Comm Function Name)

- Memory Map Definition Requirements

- Sub Modules (Functions)

- This table identifies the software segments for functions identified in this module.

- Name of Sub Module

- RTE_START_SEC_SA_MTRVEL2_APPL_CODE

- Local Functions

- Known Issues / Limitations With Design

- Revision Control Log

- Change Description

- Author Initials

- Initial AutoSAR release.

- Update the Input and output ports of Motor Velocity

- Updated Port interface name to match the FDD

- A-5749 fixes ie replacing MtrVel with raw cal values

- Update Motor Velocity for A7136, A7138, A7385 (Section 6.2.4 , section 6.8.3 flow chart)

- SOFTWARE MODULE DESIGN SPECIFICATION

- Motor Velocity

- DOCPROPERTY "Product Line" \* MERGEFORMAT

- 0612-OctDec- -13

- Selva Sengottaiyan

- NEXTEER CONFIDENTIAL

- S/W module design template, Rev 2.2b

- }qbSqbSq}q}OHD

- {w{w{w{wrnjnbnb^bn
