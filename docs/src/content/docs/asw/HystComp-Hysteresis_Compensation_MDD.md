---
title: "HystComp — Hysteresis_Compensation_MDD"
description: "Converted .doc document from HystComp/doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/HystComp/doc/Hysteresis_Compensation_MDD.doc`.

- Module -- Hysteresis Compensation

- High-Level Description

- This module will calculate a motor torque command to add into the low pass assist torque that will compensate for the hysteresis present in the system.

- Function Data Sharing

- This diagram shows all data that is shared between functions within the module.

- HystComp_Per1

- This diagram describes the functional characteristics and data flow of a given function.

- EMBED Visio.Drawing.11

- Variable Data Dictionary

- For details on module input / output variable, refer to the Data Dictionary for the application. Input / output variable names are listed here for reference.

- (Note: Full variable names required in table.)

- (Note: All global variables including End Of Line data used should be shown here)

- Module Inputs (Global Variable Name)

- Module Outputs (Global Variable Name)

- HwTorque_HwNm_f32

- HysteresisComp_MtrNm_f32

- BaseAssistCmd_MtrNm_f32

- DefeatHystService_Cnt_lgc

- VehicleSpeed_Kph_f32

- WIRCmdAmpBlnd_MtrNm_f32

- AssistMechTempEst_DegC_f32

- FricOffset_HwNm_f32

- Module Internal Variables

- This section identifies the name, range and resolutions for module specific data created by this module. If there are no range restrictions on the variable, the term

- is placed into the table for legal range.

- Variable Name

- Software Segment

- * AssistCmdLPFiltSV_HwNm_M_str

- HYSTCOMP_START_SEC_VAR_CLEARED_UNSPECIFIED

- Single Precision Float

- * HwTrqLPFiltSV_HwNm_M_str

- * RawHystCompLPFiltSV_HwNm_M_str

- HwTrqLastUsed_HwNm_M_f32

- HYSTCOMP_START_SEC_VAR_CLEARED_32

- Fraction_Uls_M_f32

- RawCalc_HwNm_M_f32

- RiseX_HwNm_M_s1p14f32

- Single Precision Float2-14

- HYSTCOMP_START_SEC_VAR_CLEARED_16

- AstCmdLastUsed_HwNm_ M_s8p7

- CompAvail_HwNm_D_f32

- HwTrqFilt_HwNm_D_f32

- CoulFric_HwNm_D_f32

- PosAvail_HwNm_D_f32

- NegAvail_HwNm_D_f32

- EffCompTrq_HwNm_D_f32

- AssistCmdFilt_HwNm_D_s8p7

- User defined typedef definition/declaration

- This section documents any user types uniquely used for the module.

- Typedef Name

- Element Name

- User Defined Type

- Constant Data Dictionary

- Calibration Constants

- This section lists the calibrations used by the module. For details on calibration constants, refer to the Data Dictionary for the application.

- Constant Name

- k_MtrNmPerHwNm_Uls_f32

- k_CmnSysTrqRatio_HwNmpMtrNm_f32

- k_HysCmpLPAstLPFKn_Hz_f32

- k_HysCmpHwTrqLPFKn_Hz_f32

- k_HysFinalOutLPFKn_Hz_f32

- k_LpFricIpLim_HwNm_u9p7

- k_HysRevGain_InvHwNm_f32

- k_HysOutLIm_HwNm_f32

- t_HysRiseTblX_HwNm_u2p14

- t_HysRiseTblY_Uls_u2p14

- t_HysSpdTblX_Kph_u9p7

- t_CmnVehSpd_Kph_u9p7

- t_EffOffTblY_HwNm_u9p7

- t_EffLossTblY_Uls_u4p12

- t2_HysHwTrqBlndTblX_HwNm_u9p7

- t2_HysHwTrqBlndTblY_Uls_u4p12

- t_HysCompCoulFricY_HwNm_u9p7

- t_HysCompCoulFricTempScaleX_DegC_s14p1

- t_HysCompCoulFricTempScaleY_HwNm_u9p7

- t_HysCompHysSatY_HwNm_u9p7

- t_HysCompCoulFricWIRBlendX_MtrNm_u8p8

- t_HysCompCoulFricWIRBlendY_Uls_u2p14

- t_HysCompNegHysCompX_MtrNm_u8p8

- t_HysCompNegHysCompY_HwNm_u9p7

- t_HysCompNegHysBlendX_HwNm_u9p7

- t_HysCompNegHysBlendY_Uls_u2p14

- Program(fixed) Constants

- Embedded Constants

- All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

- D_HYSPOSLMT_ULS_F32

- Single Precision Floating Point

- D_WIROFF_IDX_U16

- D_WIRON_IDX_U16

- D_WIRCMDBLNDFRC_ULS_F32

- D_HYSSATLOWLMT_HWNM_F32

- D_HYSOUTLMT_MTRNM_F32

- This section lists the global constants used by the module. For details on global constants, refer to the Data Dictionary for the application.

- BC_HYSTCOMP_FAULTINJECTIONPOINT

- FLTINJ_HYSTCOMP

- D_2MS_SEC_F32

- Module specific Lookup Tables Constants

- (This is for lookup tables (arrays) with fixed values, same name as other tables)

- Functions/Macros used by the Sub-Modules

- Library Functions / Macros

- The library functions / Macros that are called by the various sub modules are identified below,

- FPM_FloatToFixed_m()

- FPM_FixedToFloat_m()

- LPF_OpUpdate_f32_m ()

- IntplVarXY_u16_u16Xu16Y_Cnt()

- IntplVarXY_u16_s16Xu16Y_Cnt()

- TableSize_m()

- Sign_s16_m()

- Sign_f32_m()

- BilinearXMYM_u16_u16XMu16YM_Cnt

- Data Hiding Functions

- The data hiding functions / macros used in this module are identified below,

- Local Functions/Macros Used by this MDD only

- (Note if they are defined in another source file, then reference the appropriate header file)

- The local functions/macros in this module are identified below,

- MoreCompensation()

- LessCompensation()

- CalcAvailComp()

- Software Module Implementation

- Initialization Functions

- (Note: For multiple init functions, insert new headers at the

- 5.1 Initialization Functions

- and follow the same sub-section design shown below)

- Init: HystComp_Init1()

- Design Rationale

- LPF_KUpdate_f32 is used to initialize the LPF filter instead of the full LPF_Init_f32 macro as an optimization since the required initial state of the filter is 0, which is the initialized value of the RAM, so there is no need to explicitly initialize the state variables in this init function.

- Module Outputs

- Module Internal

- Initialize Low Pass Filters

- Periodic Functions

- Per: HystComp_Per1

- Program Flow Start

- Rte_Call_HystComp_Per1_CP0_CheckpointReached()Store Module Inputs to Local copies

- DefeatHystService_Cnt_lgc as Boolean

- VehSpd_Kph_T_f32 of type float32

- AssistCmd_MtrNm_T_f32 as float32

- HwTrq_HwNm_T_f32 of type float32

- AssistCmd_HwNm_T_f32 of type float32

- AssistCmdFilt_HwNm_T_s8p7 of type s8p7_T

- AssistCmdFilt_HwNm_T_f32 of type float32

- HwTrqFilt_HwNm_T_f32 of type float32

- RawHysComp_HwNm_St_f32 of type float32

- HysComp_HwNm_T_f32 as float32

- HysComp_MtrNm_T_f32 as float32

- Fraction_Uls_T_f32 as float32

- CompAvail_HwNm_T_f32 as float32

- TrqChange_HwNm_T_f32 as type float32

- HwNmPerMtrNm_Uls_T_f32 as float32

- PrevRiseY_Uls_T_f32 as float32

- RawHysCompZm1_HwNm_T_f32 as float32

- PrevRiseY_Uls_T_f32 = Fraction_Uls_M_f32

- RawHysCompZm1_HwNm_T_f32 = RawCalc_HwNm_M_f32

- DefeatHystService_Cnt_lgc = Rte_IRead_HystComp_Per1_DefeatHystService_Cnt_lgc();

- VehSpd_Kph_T_u9p7 = FPM_FloatToFixed_m(Rte_Iread_HystComp_Per1_VehicleSpeed_Kph_f32(), u9p7_T)

- AssistCmd_MtrNm_T_f32 = Rte_Iread_HystComp_Per1_ BaseAssistCmd_MtrNm_f32 ()

- HwTrq_HwNm_T_f32 =Rte_Iread_HystComp_Per1_HwTorque_HwNm_f32()

- HwNmPerMtrNm_Uls_T_f32 = 1.0F / k_MtrNmPerHwNm_Uls_f32;

- Convert Low Pass Assist Command to HwNm

- Apply Filtering to Torque Inputs

- Freeze Input Values if LP Assist Exceeds Threshold

- Calculate Hysteresis Loop Position Based on Quadrant

- Calculate Hysteresis and Limit Rate of Change

- Store Local copy of outputs into Module Outputs

- Rte_Iwrite_HystComp_Per1_HysteresisComp_MtrNm_f32(HysComp_MtrNm_T_f32)

- AstCmdLastUsed_HwNm_M_s8p7 = AssistCmdFilt_HwNm_T_s8p7;

- HwTrqLastUsed_HwNm_M_f32 = HwTrqFilt_HwNm_T_f32;

- Fraction_Uls_M_f32 = Fraction_Uls_T_f32;/*HysComp_Fraction*/

- RawCalc_HwNm_M_f32 = RawHysComp_HwNm_T_f32;/*HysComp_RawCalc*/

- CompAvail_HwNm_D_f32 = CompAvail_HwNm_T_f32

- ;/*HysComp_Avail*/

- Program Flow End

- Rte_Call_HystComp_Per1_CP1_CheckpointReached()

- Fault Recovery Functions

- Shutdown Functions

- Interrupt Functions

- Serial Communication Functions

- Local Function/Macro Definitions

- If these are numerous and defined in a separate source file then reference the source file only.

- MoreCompensation Calculation

- Function Name

- MoreCompensation

- UTP Tolerance

- Arguments Passed

- TrqChange_HwNm_T_f32

- RiseXPtr_HwNm_T_s1p14f32

- s1p14_Tfloat32*

- Return Value

- RiseY_Uls_T_s1p14

- LessCompensation Calculation

- LessCompensation

- PrevRiseY_Uls_T_f32

- RiseY_Uls_T_f32

- Two saturation blocks from the partial reversal block were omitted from the design as they were redundant. The limiting of the RiseY happens after the merge block and is redundant and the RiseX is implicitly limited by the interpolation lookup.

- Calculate Available Compensation

- CalcAvailComp

- HwTrqFilt_HwNm_T_f32

- AssistCmdFilt_HwNm_T_s8p7

- VehSpd_Kph_T_u9p7

- CompAvail_HwNm_T_f32

- The limit function that bounds HysTrq_HwNm_T_f32 between ZERO and FPSATHILMT was used to match the design in the FDD, however, the HIGH bound of the limit is unreachable as the maximum possible value for the input does not cause a limiting condition. An alternate design choice would have been to use a max() function between HysTrq_HwNm_T_f32 and ZERO as the only limiting factor is the LOWER bound.

- Localvariables:

- EffOff_HwNm_T_f32

- EffLoss_Uls_T_f32

- HysTrq_HwNm_T_f32

- HysBlend_Uls_T_f32

- WIROffFric_HwNm_T_f32

- WIROnFric_HwNm_T_f32

- CoulFricHysBlend_T_f32

- HysNegBlend_Uls_T_f32

- WIRFric_HwNm_T_f32

- TempScale_HwNm_T_f32

- CoulFric_HwNm_T_f32

- HwTrqFilt_HwNm_T_s7p8

- HysSat_HwNm_T_f32

- HysNegBlndCmp_T_f32

- WIRCmdAmpBlnd_MtrNm_u8p8

- WIRCmdBlnd_Uls_T_f32

- HysNegComp_Uls_T_f32

- AssistMechTempEst_DegC_T_s14p1

- AbsCombinedTrq_HwNm_T_f32

- Execution Requirements

- Execution Sequence of the Module

- (Describe in words relevant details about the execution sequence of the different sub modules.)

- Execution Rates for sub-modules called by the Scheduler

- This table serves as reference for the Scheduler design

- Calling Frequency

- System State(s) in which the function is called

- HystComp_Per1()

- Execution Requirements for Serial Communication Functions

- Sub-Module called by (Serial Comm Function Name)

- Memory Map Definition Requirements

- Sub Modules (Functions)

- This table identifies the software segments for functions identified in this module.

- Name of Sub Module

- HystComp_Init1()

- RTE_AP_HYSTCOMP_APPL_CODE

- Local Functions

- This table identifies the software segments for local functions identified in this module.

- AP_HYSTCOMP_CODE

- LowCompensation()

- Known Issues / Limitations With Design

- INLINE Functions defined in globalmacro.h are not unittested

- Revision Control Log

- Change Description

- Author Initials

- Initial AutoSAR version.

- Added negative hysteresis and ConstFric Blending interface

- Added ball screw temperature compensation

- Update section9 for INLINE functions

- Removed Per1 no longer used

- Corrections per SWC interface requirements

- Corrected initialization of HwNmPerMtrNm_Uls_T_f32

- Anomaly Fixes and removed unused Module level variable PrevRiseX_Uls_M_s8p7

- Changes done as per FaultInjectionTechnique

- Changed component over to floating point

- Added design rationale to CalcAvailComp to document unit test limit path failure

- Updated to new Average Friction Learninput requirements

- Removed SlewRate limit in 6.2.1.7 section

- Replaced Limit with Max and removed D_FPSATHILMT_ULS_F32 in sec 6.7.3.2

- Added checkpoints and memmap software segment is updated for static variables

- Replaced 1-D AsstMagBlndTbl with 2D HwTrqBlnd Table.Six more Display variables added

- Changed precision of t_HysRiseTblY & t_HysRiseTblX per Anom 6855.

- Anomaly 4110 correction

- Anom 4937 correction

- Update to FDD ver 007

- SOFTWARE MODULE DESIGN SPECIFICATION

- Hysteresis Compensation

- DOCPROPERTY "Product Line" \* MERGEFORMAT

- DATE \@ "d-MMM-yy"

- 2-May-131-May-13

- Blake Latchford (zz4r1x)Niveditha Reddy

- Nexteer CONFIDENTIAL

- S/W module design template, Rev 3.0a

- yunduyu`Y`yuyu
