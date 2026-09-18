---
title: "MtrVel_Digi — MotorVelocity_MDD"
description: "Converted .doc document from MtrVel_Digi/doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/MtrVel_Digi/doc/MotorVelocity_MDD.doc`.

- tored in the associated index of MtrVel3_OsBufPos_Cnt_M_u08[] . The design requires monotonically increasing timestamps relative to the starting index value in MtrVel3_OsBufPos_Cnt_M_u08[]. Due to the modulo 65536 behavior of the timestamp, a single timestamp rollover within the active sample set pair is correctly handled by the design. Simultaneous sample points (e.g.

- t = 0 for consecutive timestamps) are invalid and will result in a divide by zero in the current design. Unit Test vectors for functions which have MtrVel3_TimeBuffer_uS_M_u16p0[4][8] as an input (MtrVel_Per1 and RegressionFit) must provide an input vector value set which conforms to the set of rules in the following table:

- Buffer consecutive timestamp value

- twice the nominal execution rate for MtrCtrl ISR. This is to account for a worst case delay scenario.

- Cross buffer set timestamp pair

- between the oldest samples in each buffer, the

- between the second oldest oldest samples in each buffer, etc)

- i.e. MtrVel3_TimeBuffer_uS_M_u16p0 [MtrVel_OsBufSelect_M_u08][i] - MtrVel3_TimeBuffer_uS_M_u16p0 [MtrVel_OldPosBuf_M_u08][k]

- where k = i + (MtrVel3_OsBufPos_Cnt_M_u08[MtrVel_OldPosBuf_M_u08] - MtrVel3_OsBufPos_Cnt_M_u08[MtrVel_OsBufSelect_M_u08]) modul

- MtrVel_OsBufSelect_Cnt_M_u08. Failure to do so will result in a divide by 0 exception.

- D_MTRVELOSBUFSZ_CNT_U08

- is defined as Cal

- k_BufferSize

- in SF40AB. Since the size of the array is based on the Calibration, the calibration is changed to configurable constant.

- This allow s integrater to modify the constant before compilation. This saves memory wastage.

- Revision Control Log

- Change Description

- Author Initials

- Initial AutoSAR release.

- Updated the input and the output through RTE ports

- Updated the Ports names to match the FDD

- Updated the Buffer Index in Regression fit A-5803

- Update Motor Velocity for A7136, A7138, A7385 (Section 6.2.4 , section 6.8.3 flow chart)

- SOFTWARE MODULE DESIGN SPECIFICATION

- Motor Velocity

- DOCPROPERTY "Product Line" \* MERGEFORMAT

- 06-Oct-1312- Dec- 14

- NeXTEER CONFIDENTIAL

- S/W module design template, Rev 2.2b

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

- AsstAssemblyPolarity_Cnt_s08

- SysCMotorVelMRF_MtrRadpS_f32

- SysCDiagHandwheelVel_HwRadpS_f32

- SysCHandwheelVel_HwRadpS_f32

- SysCDiagMtrVelMRF_MtrRadpS_f32

- MotorVelCRF_MtrRadpS_f32

- MechMtrPos2_Rev_u0p16

- MotorVelMRF_MtrRadpS_f32

- MechMtrPos1Timestamp_USec_u32

- HandWheelVel_HwRadpS_f32

- HwVelValid_Cnt_lgc

- MechMtrPos1_Rev_u0p16

- MechMtrPos2Timestamp_USec_u32

- SysCDiagHwVel_HwRadpS_f32

- Module Internal Variables

- This section identifies the name, range and resolutions for module specific data created by this module. If there are no range restrictions on the variable, the term

- is placed into the table for legal range.

- Variable Name

- Software Segment

- MtrVel_WestBlendedMtrVel_MtrRadpS_D_f32

- Single Precision Floating Point

- MTRVEL_START_SEC_VAR_CLEARED_32

- MtrVel_PrevMtrPosMechMtrPos2_Rad_M_f32

- MtrVel_CrsMtrVel_MtrRadpS_D_f32

- MtrVel_PriMtrVel_MtrRadpS_D_f32

- MtrVel_HwVel_HwRadpS_M_f32

- MtrVel_MtrVelCorrLimDiff_MtrRadpS_D_f32

- MtrVel_HwVelCorrLimDiff_HwRadpS_D_f32

- MtrVel_DiffAcc_Cnt_M_u16

- MTRVEL_START_SEC_VAR_CLEARED_16

- MtrVel_HwVelDiffAcc_Cnt_M_u16

- MtrVel_OsBufSelect_Cnt_M_u08

- MTRVEL_START_SEC_VAR_CLEARED_8

- MtrVel_OldPosBuf_Cnt_M_u08

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

- t_MtrVelBlendTblX_MtrRadpS_u12p4

- k_GearRatio_Uls_f32

- k_MtrVelCorrLim_Cnt_Str

- k_HwVelCorrLim_Cnt_Str

- k_MtrVelCorrLim_MtrRadpS_f32

- k_HwVelCorrLim_HwRadpS_f32

- Program(fixed) Constants

- Embedded Constants

- All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

- D_USECPERSEC_ULS_F32

- D_MTRVELOSBUFNUM_CNT_U08

- D_SNAPSHOTBUF_CNT_U08

- D_MTRVELLOLMT_MTRRADPS_F32

- T_MtrVelBlendTblY_Uls_u2p14[2]

- D_MAXHANDWHEELVEL_HWPADPS_F32

- D_MINHANDWHEELVEL_HWPADPS_F32

- This section lists the global constants used by the module. For details on global constants, refer to the Data Dictionary for the application.

- D_RADPERREV_ULS_F32

- D_ZERO_CNT_U8

- D_MTRVELOSBUFSZ_CNT_U08 (from MtrVel_Cfg.h)

- Module specific Lookup Tables Constants

- (This is for lookup tables (arrays) with fixed values, same name as other tables)

- T_MtrVelBlendTblY_Uls_u2p14

- Functions/Macros used by the Sub-Modules

- Library Functions / Macros

- The library functions / Macros that are called by the various sub modules are identified below,

- FPM_FixedToFloat_m()

- FPM_FloatToFixed_m()

- IntplVarXY_u16_u16Xu16Y_Cnt()

- LPF_SvUpdate_s16InFixKTrunc_m()

- LPF_OpUpdate_s16InFixKTrunc_m()

- Rte_Call_NxtrDiagMgr_GetNTCFailed

- Rte_Call_NxtrDiagMgr_SetNTCStatus

- TableSize_m()

- Data Hiding Functions

- The data hiding functions / macros used in this module are identified below,

- Local Functions/Macros Used by this MDD only

- (Note if they are defined in another source file, then reference the appropriate header file)

- The local functions/macros in this module are identified below,

- CalcCoarseVel()

- MtrVelBlend()

- RegressionFit()

- Software Module Implementation

- Initialization Functions

- Init: MtrVel_Init1

- Design Rationale

- Module Outputs

- Module Internal

- EMBED Visio.Drawing.11

- Periodic Functions

- Per: MtrVel_Per1

- Program Flow Start

- Rte_Call_MtrVel_Per1_CP0_CheckpointReached()

- Store Module Inputs to Local copies

- AsstAssemPol_Cnt_T_s8 = Rte_IRead_MtrVel_Per1_AsstAssemblyPolarity_Cnt_s08();

- MtrPos_SampleTime2_uS_T_u32= Rte_IRead_MtrVel_Per1_MechMtrPos2Timestamp_USec_u32()

- MtrPos_MechMtrPos2_Rev_T_u0p16 = Rte_IRead_MtrVel_Per1_MechMtrPos2_Rev_u0p16();

- Calculate Raw Motor Velocity

- Store Local copy of outputs into Module Outputs

- (void)Rte_IWrite_MtrVel_Per1_SysCMotorVelMRF_MtrRadpS_f32(MtrVel_MtrVelMRF_MtrRadpS_M_f32);

- (void)Rte_IWrite_MtrVel_Per1_SysCHandwheelVel_HwRadpS_f32(MtrVel_HwVel_HwRadpS_M_f32);

- (void)Rte_IWrite_MtrVel_Per1_MotorVelCRF_MtrRadpS_f32(MtrVelCRF_MtrRadpS_T_f32);

- (void)Rte_IWrite_MtrVel_Per1_MotorVelMRF_MtrRadpS_f32(MtrVel_MtrVelMRF_MtrRadpS_M_f32);

- (void)Rte_IWrite_MtrVel_Per1_HandwheelVel_HwRadpS_f32(MtrVel_HwVel_HwRadpS_M_f32);

- Program Flow End

- Rte_Call_MtrVel_Per1_CP1_CheckpointReached()

- Per: MtrVel_Per2

- Rte_Call_MtrVel_Per2_CP0_CheckpointReached()

- SysCDiagMtrVelMRF_MtrRadpS_T_f32 = Rte_IRead_MtrVel_Per2_SysCDiagMtrVelMRF_MtrRadpS_f32();

- SysCDiagHandWheelVel_HwRadpS_T_f32 = Rte_IRead_MtrVel_Per2_SysCDiagHwVel_HwRadpS_f32();

- (void)Rte_Call_NxtrDiagMgr_GetNTCFailed(NTC_Num_PriMSB_SinCosCorr,&MtrPosFault1_Cnt_T_lgc)

- (void)Rte_Call_NxtrDiagMgr_GetNTCFailed(NTC_Num_PriVsSec_SinCosCorr, &MtrPosFault2_Cnt_T_lgc);

- Rte_Call_MtrVel_Per2_CP1_CheckpointReached()

- Fault Recovery Functions

- Shutdown Functions

- Interrupt Functions

- Serial Communication Functions

- Local Function/Macro Definitions

- If these are numerous and defined in a separate source file then reference the source file only.

- Calculation Coarse Velocity

- Function Name

- CalcCoarseVel

- Arguments Passed

- DeltaPos_Rad_T_f32

- DeltaTime_uS_T_f32

- Return Value

- MtrVel_MtrRadpS_T_f32

- Motor Velocity Blend

- FinMtrVel_MtrRadpS_T_f32

- CrsMtrVel_MtrRadpS_T_f32

- Regression Fit

- Execution Requirements

- Execution Sequence of the Module

- (Describe in words relevant details about the execution sequence of the different sub modules.)

- Execution Rates for sub-modules called by the Scheduler

- This table serves as reference for the Scheduler design

- Calling Frequency

- System State(s) in which the function is called

- MtrVel_Init1

- Execution Requirements for Serial Communication Functions

- Sub-Module called by (Serial Comm Function Name)

- Memory Map Definition Requirements

- Sub Modules (Functions)

- This table identifies the software segments for functions identified in this module.

- Name of Sub Module

- RTE_SA_MTRVEL_APPL_CODE

- Local Functions

- This table identifies the software segments for local functions identified in this module.

- AP_MTRVEL_CODE

- RegressionFit

- Known Issues / Limitations With Design

- In this design, MtrVel3_TimeBuffer_uS_M_u16p0[][] represents a set of independent circular buffers. Each buffer contains a set of continuous timestamps with the most recent timestamp index of each sample set st

- MtrVel3_TimeBuffer_uS_M_u16p0 [i][k] - MtrVel3_TimeBuffer_uS_M_u16p0 [i][k+1]

- Monotonically increasing in a modulo 65536 fashion (e.g. testing of the 16 bit rollover point allows for a single rollover point within the data buffer that is not monotonically increasing).

- The UTP MUST provide at least 1 test vector that provides a data set with a time stamp rollover (See

- REF _Ref355689267 \h

- 10 uS is the worst case minimum sampling period based on the MtrCtrl ISR runtime.

- 250 uS is the minimum required time to guarantee 8 samples at a nominal 62.5 uS sample rate have been completed.

- 4000 uS is twice the execution rate for MtrVel_Per1. This is to account for a worst case delay scenario.

- When computing the delta it is necessary to perform modulo 65536 math compensation to account for rollover situations (e.g.

- [z-7] samples depict a rollover case where the natural delta is 1764

- 65300 = -63536, however this is not the correct delta result for the strictly increasing modulo 65536 accumulator. Since the natural result is negative, 65536 must be added to obtain the actual delta, -63536 + 65536 = 2000.

- for a complete example conforming to this rule.

- SEQ Table \* ARABIC

- : Time Buffer UTP Constraints

- The following *.bas is a VBA function to validate the timestamp data sets.

- EMBED Package

- EXAMPLE TimeStamp Buffer Data Set:

- The following buffer timestamp data set provides an example when buffers 0 and 1 are active. Values for buffers 2 and 3 are don

- t care values for this example and shown as

- . The samples within the buffers have subscripts which describe the samples order relative to the newest sample in the buffer (e.g. z-1 indicates that the sample is 1 sample period old, z-2 indicates the sample is 2 sample periods old, etc). Samples of the same relative order within each buffer have the same cell shading applied to aid the reader in locating cross buffer sample pairs.

- MtrVel_OldPosBuf_M_u08 = 0

- MtrVel_OsBufSelect_M_u08 = 1

- MtrVel3_OsBufPos_Cnt_M_u08[0] = 0

- MtrVel3_OsBufPos_Cnt_M_u08[1] = 2

- MtrVel3_OsBufPos_Cnt_M_u08[2] = Don

- MtrVel3_OsBufPos_Cnt_M_u08[3] = Don

- : Example UTP TimeBuffer Roll-Over Sample Set

- The state variables MtrVel_OldPosBuf_M_u08 and MtrVel_OsBufSelect_Cnt_M_u08 have a relationship that is maintained by logic that is executed after their use in RegressionFit(). The RegressionFit() function design requires a valid set of state variables to function properly. Therefore, it is possible to provide an illegal value set for the related state variables in a unit testing environment that 

- znznznbnbzbz

- ia]a]a]a]XTLTLTL
