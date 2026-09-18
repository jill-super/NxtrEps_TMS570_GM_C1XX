---
title: "MtrCtrl_CM — CurrCmd_MDD"
description: "Converted .doc document from MtrCtrl_CM/doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/MtrCtrl_CM/doc/CurrCmd_MDD.doc`.

- Module -- CurrCmd

- High-Level Description

- This Module generates the current command and the voltage reference for the current control.

- Function Data Sharing

- Function (Name)

- Variable Data Dictionary

- For details on module input / output variable, refer to the Data Dictionary for the application. Input / output variable names are listed here for reference.

- Module Inputs

- Module Outputs

- Refer Data Dictionary

- Module Internal Variables

- This section identifies the name, range and resolutions for module specific data created by this module. If there are no range restrictions on the variable, the term

- is placed into the table for legal range.

- Variable Name

- Software Segment

- For all information regarding Module level/Display variable refer Data Dictionary

- User defined typedef definition/declaration

- This section documents any user types uniquely used for the module.

- Typedef Name

- Element Name

- User Defined Type

- LowPassFiltBilinear_Str

- PrevInput_Uls_f32

- Single precision float

- PrevOutput_Uls_f32

- TermN_Uls_f32

- TermD_Uls_f32

- Constant Data Dictionary

- Calibration Constants

- This section lists the calibrations used by the module. For details on calibration constants, refer to the Data Dictionary for the application.

- Constant Name

- Program(fixed) Constants

- Embedded Constants

- All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

- D_SQRT3OVR2_ULS_F32

- Single Precision Float

- D_MTRPOLESDIV2_CNT_F32

- D_2OVRSQRT3_ULS_F32

- D_NEG2OVRSQRT3_ULS_F32

- -1.15470053837925F

- D_ROUND_ULS_F32

- D_NEGROUND_ULS_F32

- D_NEG_ULS_F32

- D_MAXCURRENT_AMP_F32

- D_SIZERDLTAPOINTS_CNT_U16

- TableSize_m(t_RefDeltaPoints_Rad_f32)

- D_MAXDELTAPOINTSSIZE_CNT_U16

- D_PIPLUSPIOVER4_ULS_F32

- D_PI_ULS_F32+( D_2PI_ULS_F32/4)

- D_VECUMAX_VOLTS_F32

- D_2PISQRT3OVR2_ULS_F32

- (D_2PI_ULS_F32*D_SQRT3OVR2_ULS_F32)

- D_FOUROVRSQRT3_ULS_F32

- ( D_2OVRSQRT3_ULS_F32* 2.0F)

- D_BANDWIDTHLOLIM_HZ_F32

- D_BANDWIDTHHILIM_HZ_F32

- D_NATFREQLOLIM_HZ_F32

- D_NATFREQHILIM_HZ_F32

- D_VECUDEFAULT_VOLT_F32

- This section lists the global constants used by the module. For details on global constants, refer to the Data Dictionary for the application.

- D_ZERO_ULS_F32

- D_180OVRPI_ULS_F32

- D_ONE_ULS_F32

- D_QUADRANT3_CNT_U8

- D_QUADRANT1_CNT_U8

- D_2PI_ULS_F32

- D_ZERO_CNT_U16

- D_VECUMIN_VOLTS_F32

- Module specific Lookup Tables Constants

- (This is for lookup tables (arrays) with fixed values, same name as other tables)

- Functions/Macros used by the Sub-Modules

- Library Functions / Macros

- The library and functions / Macros that are called by the various sub modules are identified below,

- FPM_FloatToFixed_m

- LPF_SvUpdate_s16InFixKTrunc_m

- LPF_OpUpdate_s16InFixKTrunc_m

- FPM_FixedToFloat_m

- IntplVarXY_u16_u16Xu16Y_Cnt

- Data Hiding Functions

- Global Functions/Macros Defined by this Module

- Local Functions/Macros Used by this MDD only

- Local Function #1

- Function Name

- ParabolicInterpolation

- Arguments Passed

- IntpolPoints_Uls_T_f32[6]

- HYPERLINK "tel:2147483648" \t "_blank"

- HYPERLINK "tel:2147483647" \t "_blank"

- Return Value

- ParaIntpol_Uls_T_f32

- EMBED Visio.Drawing.11

- Local Function #2

- CalculateImVSIdq

- IdRef_Amp_T_f32

- IqRef_Amp_T_f32

- ImVSIdq_AmpSq_T_f32

- Local Function #3

- Torquecmd_MtrNm_T_f32

- IqRefTmp_Amp_T_f32

- Local Function #4

- CurrtoVoltTest

- *VqR_Amp_T_f32

- *VdR_Amp_T_f32

- VoltTest_Uls_T_lgc

- Local Function #5

- CosDelta_Cnt_T_f32

- SinDelta_Cnt_T_f32

- *IdMax_Amp_T_f32

- TorqueCalc_MtrNm_T_f32

- Local Function #6

- LocateTrqExtremese

- MtrTrqCmd_MtrNm_T_f32

- *PhsAdvPeak_Rad_T_f32

- LimitedMRFMtrTrqCmd_MtrNm_T_f32

- Local Function #7

- LocateMinimumIm

- * IdMin_Amp_T_f32

- * IqMin_Amp_T_f32

- ImSqrMin_AmpSq_T_f32

- Local Function #8

- CalLowPassFiltBilinearOut

- Input_Uls_T_f32

- *LowPassFiltBilinear_T_Str

- Output_Uls_T_f32

- Local Function #9 CalLowPassFiltBilinearTerm

- CalLowPassFiltBilinearTerm

- Freq_Hz_T_f32

- TimeCons_Sec_T_f32

- LowPassFiltBilinear_T_Str

- Local Function #10

- MtrCurrAngle_Rev_T_f32

- Local Function #11

- CalculateIdBoost

- *IqMin_Amp_T_f32

- *IdMin_Amp_T_f32

- IdMax_Amp_T_f32

- Software Module Implementation

- Runtime Environment (RTE) Initial Values

- This section lists the initial values of data written by this module but controlled by the RTE. After RTE initialization, the data in this table will contain these values.

- Rte_InitValue_DaxIntegralGain_Uls_f32

- Rte_InitValue_DaxPropotionalGain_Uls_f32

- Rte_InitValue_EstKe_VpRadpS_f32

- Rte_InitValue_EstLd_Henry_f32

- Rte_InitValue_EstLq_Henry_f32

- Rte_InitValue_EstR_Ohm_f32

- Rte_InitValue_MRFMtrVel_MtrRadpS_f32

- Rte_InitValue_MRFTrqCmdScl_MtrNm_f32

- Rte_InitValue_MtrCurrAngle_Rev_f32

- Rte_InitValue_MtrCurrDaxRef_Amp_f32

- Rte_InitValue_MtrCurrQaxRef_Amp_f32

- Rte_InitValue_MtrPosComputationDelay_Deg_f32

- Rte_InitValue_MtrTrqCmdSign_Cnt_s16

- Rte_InitValue_MtrVoltDaxFF_Volt_f32

- Rte_InitValue_MtrVoltQaxFF_Volt_f32

- Rte_InitValue_QaxIntegralGain_Uls_f32

- Rte_InitValue_QaxPropotionalGain_Uls_f32

- Rte_InitValue_VehSpd_Kph_f32

- FastDataAccessBufIndex

- Initialization Functions

- CurrCmd_Init

- Program Flow Start

- Rte_Call_CurrCmd_Per1_CP0_CheckpointReached()

- Periodic Functions

- Per: CurrCmd_Per1

- Design Rationale

- Store Module Inputs to Local copies

- WriteAccessBufIndex_Cnt_T_u16= (FastDataAccessBufIndex_Cnt_M_u16&1)^1;

- MRFMtrTrqCmd_MtrNm_T_f32=Rte_Iread_CurrCmd_Per1_MRFTrqCmdScl_MtrNm_f32

- MRFMtrVel_MtrRadpS_T_f32=Rte_Iread_CurrCmd_Per1_MRFMtrVel_MtrRadpS_f32

- EstKe_VpRadpS_T_f32=Rte_Iread_CurrCmd_Per1_EstKe_VpRadpS_f32

- EstR_Ohm_T_f32=Rte_Iread_CurrCmd_Per1_EstR_Ohm_f32

- EstLd_Henry_T_f32=Rte_Iread_CurrCmd_Per1_EstLd_Henry_f32

- EstLq_Henry_T_f32=Rte_Iread_CurrCmd_Per1_EstLq_Henry_f32

- VehSpd_Kph_T_f32=Rte_Iread_CurrCmd_Per1_VehSpd_Kph_f32

- MtrQuad_Cnt_T_u8 = Rte_Iread_CurrCmd_Per1_MtrQuad_Cnt_u08

- CurrentGainSvc_Cnt_T_lgc = Rte_IRead_CurrCmd_Per1_CurrentGainSvc_Cnt_lgc()

- Vecu_Volt_T_f32 = Limit_m(Vecu_Volt_T_f32, D_VECUMIN_VOLTS_F32, D_VECUMAX_VOLTS_F32)

- IvtrLoaMtgtnEn_Cnt_T_lgc = Rte_IRead_CurrCmd_Per1_IvtrLoaMtgtnEn_Cnt_lgc()

- MotCurrLoaMtgtnEn_Cnt_T_lgc= Rte_IRead_CurrCmd_Per1_MotCurrLoaMtgtnEn_Cnt_lgc()

- Store Local copy of outputs into Module Outputs

- MtrCurrQaxRef_Amp_M_f32[WriteAccessBufIndex_Cnt_T_u16] = MtrCurrQaxRef_Amp_T_f32;

- MtrCurrDaxRef_Amp_M_f32[WriteAccessBufIndex_Cnt_T_u16] = MtrCurrDaxRef_Amp_T_f32;

- MtrCtrl_MtrDaxIntegralGain_Ohm_M_f32[WriteAccessBufIndex_Cnt_T_u16] = KidGain_Ohm_T_f32

- MtrCtrl_MtrDaxPropotionalGain_Ohm_M_f32[WriteAccessBufIndex_Cnt_T_u16] = KpdGain_Ohm_T_f32

- MtrCtrl_MtrQaxIntegralGain_Ohm_M_f32[WriteAccessBufIndex_Cnt_T_u16] = KiqGain_Ohm_T_f32

- MtrCtrl_MtrQaxPropotionalGain_Ohm_M_f32[WriteAccessBufIndex_Cnt_T_u16] = KpqGain_Ohm_T_f32

- Rte_IWrite_CurrCmd_Per1_MtrCurrDaxRef_Amp_f32(MtrCurrDaxRef_Amp_T_f32)

- Rte_IWrite_CurrCmd_Per1_MtrCurrQaxRef_Amp_f32(MtrCurrQaxRef_Amp_T_f32)

- Rte_IWrite_CurrCmd_Per1_MtrCurrAngle_Rev_f32(MtrCurrAngle_Rev_T_f32)

- MtrCtrl_MtrVoltDaxFF_Volt_M_f32[WriteAccessBufIndex_Cnt_T_u16] = MtrVoltDaxFF_Volt_T_f32

- MtrCtrl_MtrVoltQaxFF_Volt_M_f32[WriteAccessBufIndex_Cnt_T_u16] = MtrVoltQaxFF_Volt_T_f32

- MtrPosComputationDelay_Rad_M_f32[WriteAccessBufIndex_Cnt_T_u16] = ElecPosDelayComp_Rad_T_f32

- MtrCtrl_MtrDampTermDax_Ohm_M_f32[WriteAccessBufIndex_Cnt_T_u16] = MtrDampTermDax_Ohm_T_f32

- MtrCtrl_MtrDampTermQax_Ohm_M_f32[WriteAccessBufIndex_Cnt_T_u16] = MtrDampTermQax_Ohm_T_f32

- MtrCtrl_MtrImpedDax_Ohm_M_f32[WriteAccessBufIndex_Cnt_T_u16] = MtrImpedDax_Ohm_T_f32

- MtrCtrl_MtrImpedQax_Ohm_M_f32[WriteAccessBufIndex_Cnt_T_u16] = MtrImpedQax_Ohm_T_f32

- MtrCtrl_MtrCurrDaxMaxVal_Amp_M_f32[WriteAccessBufIndex_Cnt_T_u16]=MtrCurrDaxMaxVal_Amp_T_f32

- MtrCtrl_MtrPosComputationDelayRpl_Rad_M_f32[WriteAccessBufIndex_Cnt_T_u16] = ElecPosDelayCompRpl_Rad_T_f32

- MtrCtrl_Vecu_Volt_M_f32[WriteAccessBufIndex_Cnt_T_u16] = Vecu_Volt_T_f32

- Program Flow End

- Rte_Call_CurrCmd_Per1_CP1_CheckpointReached()

- Fault Recovery Functions

- Shutdown Functions

- Interrupt Functions

- Serial Communication Functions

- Execution Requirements

- Execution Sequence of the Module

- (Describe in words relevant details about the execution sequence of the different sub modules.)

- Execution Rates for sub-modules called by the Scheduler

- This table serves as reference for the Scheduler design

- Calling Frequency

- System State(s) in which the function is called

- CurrCmd_Per1

- Execution Requirements for Serial Communication Functions

- Sub-Module called by (Serial Comm Function Name)

- Memory Map Definition Requirements

- Sub Modules (Functions)

- This table identifies the software segments for functions identified in this module.

- Name of Sub Module

- RTE_START_SEC_AP_CURRCMD_APPL_CODE

- Local Functions

- This table identifies the software segments for local functions identified in this module.

- LocateTrqExtremes

- Known Issues / Limitations With Design

- Global Macro

- s are not unit tested.

- Revision Control Log

- Change Description

- Author Initials

- Initial version

- Partial implementation of SF-99B v004

- Checkpoints and memmap statements added

- Implementation of SF99 v8

- Corrected for A5883. Corrected LocateMinimumIm

- Updated for v11 FDD99B

- Corrected for NewDelta calculation / Updated for v11 FDD99B UTP fixes

- Updated for V12 of FDD SF99

- Updated for v15 of FDD SF99B

- Updated for V17 of FDD SF99 EA3#A283,EA3#1777 fixed

- Unit Testing finding fixes

- Updated for V18 of FDD SF99

- SOFTWARE MODULE DESIGN SPECIFICATION

- DOCPROPERTY "Product Line" \* MERGEFORMAT

- Gen II+ EPS EA3

- DATE \@ "d-MMM-yy"

- Selva Sengottaiyan

- DOCPROPERTY "Company" \* MERGEFORMAT

- CONFIDENTIAL

- MDD Template EA3, Rev 1.1
