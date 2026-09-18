---
title: "DampingFirewall — Damping_Firewall_MDD"
description: "Converted .doc document from DampingFirewall/doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/DampingFirewall/doc/Damping_Firewall_MDD.doc`.

- DOCPROPERTY "Document Title" \* MERGEFORMAT

- Damping Firewall

- High-Level Description

- This module regulates the damping command according to safety specifications.

- Component Diagram

- Variable Data Dictionary

- For details on module input / output variable, refer to the Data Dictionary for the application. Input / output variable names are listed here for reference.

- Module Inputs

- Module Outputs

- AsstFirewallActive_Uls_f32

- CombinedDamping_MtrNm_f32

- DampingCmd_MtrNm_f32

- HwTorque_HwNm_f32

- InertiaComp_MtrNm_f32

- MtrVelCRF_MtrRadpS_f32

- VehicleSpeed_Kph_f32

- BaseAssistCmd_MtrNm_f32

- WIRCmdAmpBlnd_MtrNm_f32

- FreqDepDmpSrlComSvcDft_Cnt_lgc

- VehicleLonAccel_KphpS_f32

- Defeat_Damping_Svc_Cnt_lgc

- MEC_Counter_Cnt_enum

- Module Internal Variables

- This section identifies the name, range and resolutions for module specific data created by this module. If there are no range restrictions on the variable, the term

- is placed into the table for legal range.

- Variable Name

- Software Segment

- DampFWVBICErrFiltSv_M_str

- LPF32KSV_Str

- see Data Dictionary

- DAMPINGFIREWALL_START_SEC_VAR_CLEARED_UNSPECIFIED

- DampFWActiveKSV_M_str

- DampFWUprBoundKSV_M_str

- DampFWLwrBoundKSV_M_str

- DampFWUprBoundFilt_MtrNm_D_f32

- Single Precision Float

- DAMPINGFIREWALL_START_SEC_VAR_CLEARED_32

- DampFWLwrBoundFilt_MtrNm_D_f32

- DampFWUprBound_MtrNm_D_f32

- DampFWLwrBound_MtrNm_D_f32

- DampFWAddedDamp_MtrNm_D_f32

- DampFWAddedDampAFW_MtrNm_D_f32

- DampFWAddedDampDFW_MtrNm_D_f32

- DampFWTbarVelFiltSv_M_str

- DampFWSatDamp_MtrNm_D_f32

- Single Precision Floating Point

- DampFWPrevTbarAng_HwDeg_M_s6p9

- DAMPINGFIREWALL_START_SEC_VAR_CLEARED_16

- DampFWPrev1SclDrvVel_MtrRadpS_M_s14p1

- DampFWPrev2SclDrvVel_MtrRadpS_M_s14p1

- DampFWPrev1PreAttnComp_MtrNm_M_s9p6

- DampFWPrev2PreAttnComp_MtrNm_M_s9p6

- DampFWOverBound_Uls_D_lgc

- DAMPINGFIREWALL_START_SEC_VAR_CLEARED_BOOLEAN

- ReducedPerfSV_Cnt_M_lgc

- DampFWVBICOverThresh_Cnt_D_lgc

- DampFWVBICReducedPerfSV_Cnt_M_lgc

- DampFWDiverseVBIC_MtrNm_D_f32

- DampFWDefltDamp_MtrNm_D_f32

- DampFWDampActive_Uls_D_f32

- DampFWLimitedVBIC_MtrNm_D_f32

- DampFWInrtCmpPNStatus_Cnt_M_lgc

- DampFWPNCountStatus_Cnt_M_lgc

- InrtCmpPNAccum_Cnt_M_u16

- DampPNAcc_Cnt_M_u16

- PNAcc_Cnt_M_u16

- DampFWOverBound_Cnt_D_lgc

- LimitedDamp_MtrNm_D_f32

- DriverVel_MtrRadpSec_D_s24p7

- PrevDecelGain_Uls_M_u5p11

- FiltFreq_RadpS_D_s10p5

- ScaledDriverVel_MtrRadpS_D_s14p1

- OutputAtten_Uls_D_u8p8

- RawDecelGain_Uls_D_u5p11

- DecelGain_Uls_D_u5p11

- ADDCoefCalc_MtrNmSpRad_D_u0p16

- InertiaCompCalc_MtrNm_D_u9p7

- PreFiltVBICError_MtrNm_D_f32

- PostFiltVBICError_MtrNm_D_f32

- DampFWPrev1PreAttnComp_MtrNm_M_s20p11

- DampFWPrev2PreAttnComp_MtrNm_M_s20p11

- User defined typedef definition/declaration

- This section documents any user types uniquely used for the module.

- Typedef Name

- Element Name

- User Defined Type

- Constant Data Dictionary

- Calibration Constants

- This section lists the calibrations used by the module. For details on calibration constants, refer to the Data Dictionary for the application.

- Constant Name

- k_DampFWInpLimitDamp_MtrNm_f32

- k_DampFWVBICLPF_Hz_f32

- k_DampFWFWActiveLPF_Hz_f32

- k_DampFWTbarVelLPFKn_Hz_f32

- k_DmpBoundLPFKn_Hz_f32

- k_DampFWMtrVelScale_Uls_f32

- t_DampFWEstCompTblX_Kph_u9p7[]

- t_DampFWTbarVelScaleY_Uls_u2p14[]

- k_DampFWFilkKn_Hz_f32

- t_DampFWEstCompHPF_Hz_u7p9[]

- t_DampFWEstCompGain_MtrNmpMtrRadpS_u1p15[]

- t_DampFWVehSpd_Kph_u9p7[]

- t2_DampFWUprBoundX_MtrRadpS_s10p5[][]

- t2_DampFWUprBoundY_MtrNm_s4p11[][]

- t_DampFWAddDampX_MtrRadpS_u11p5[]

- t_DampFWAddDampY_MtrNm_u5p11[]

- t_DampFWDefltDampX_MtrRadpS_u11p5[]

- t_DampFWDefltDampY_MtrNm_u5p11[]

- k_DampFWErrThresh_MtrNm_f32

- t_DampFWDampInrtCmpPNThesh_Cnt_u16[]

- k_DampFWInCmpPStep_Cnt_u16

- k_DampFWInCmpNStep_Cnt_u16

- k_InrtCmp_TBarVelLPFKn_Hz_f32

- k_DampFWPstep_Cnt_u16

- k_DampFWNstep_Cnt_u16

- t_DampFWPNstepThresh_Cnt_u16[]

- k_InrtCmp_MtrInertia_KgmSq_f32

- t_InrtCmp_ScaleFactorTblY_Uls_u9p7[]

- t_InrtCmp_TBarVel_ScaleFactorTblY_Uls_u9p7[]

- k_InrtCmp_MtrVel_ScaleFactor_Uls_f32

- t_InrtCmp_VehSpdTblX_Kph_u15p1[]

- t_FDD_ADDStaticTblY_MtrNmpRadpS_um1p17[]

- t2_FDD_ADDRollingTblYM_MtrNmpRadpS_um1p17[][]

- t_FDD_BlendTblY_Uls_u8p8[]

- t_FDD_FreqTblYM_Hz_u12p4[]

- t_FDD_AttenTblX_MtrRadpS_u12p4[]

- t_FDD_AttenTblY_Uls_u8p8[]

- t_WIRBlndTblX_MtrNm_u8p8[]

- t_RIAstWIRBlndTblY_Uls_u2p14[]

- t_DmpFiltKpWIRBlndY_Uls_u2p14[]

- k_CmnTbarStiff_NmpDeg_f32

- t_DmpADDCoefX_MtrNm_u4p12[10]

- k_DmpGainOnThresh_KphpS_f32

- k_DmpGainOffThresh_KphpS_f32

- k_DmpDecelGain_Uls_f32

- k_DmpDecelGainFSlew_UlspS_f32

- t_DmpDecelGainSlewX_MtrRadpS_f32[]

- t_DmpDecelGainSlewY_UlspS_f32[]

- k_CmnSysKinRatio_MtrDegpHwDeg_f32

- Program (fixed) Constants

- Embedded Constants

- All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

- D_ONEOVR2MS_SEC_U9P7

- D_2MS_SEC_U0P16

- D_2MS_SEC_U2P14

- D_PIOVR180_ULS_S4P11

- D_ONE_ULS_U2P14

- D_ONE_ULS_U8P8

- D_ONE_ULS_U5P11

- D_TWO_ULS_S2P13

- D_2PI_ULS_U2P13

- D_TBARVELFILTVAL_HWDEGPSEC_S15P16

- D_TERMA_MTRRADPSEC_S20P11

- D_EIGHT_ULS_U10P6

- D_SCALEDDRIVERVEL_MTRRADPS_S17P14

- D_COMPENSATIONLIMIT_MTRNM_S11P20

- D_INERTIACOMPCALCLIMIT_MTRNM_U15P1

- D_FOUR_ULS_S3P12

- D_ADDCOEFCALCHILIMIT_MTRNMSPRAD_U1P15

- D_ADDCOEFCALCHILIMIT_MTRNMSPRAD_U3P13

- D_ABSSCALEDRIVERVELHI_MTRRADPS_U15P1

- VEHICLELONACCEL_MIN_F32

- VEHICLELONACCEL_MAX_F32

- D_ONE_ULS_U11P21

- This section lists the global constants used by the module. For details on global constants, refer to the Data Dictionary for the application.

- D_2MS_SEC_F32

- D_PIOVR180_ULS_F32

- D_ZERO_ULS_F32

- D_FALSE_CNT_LGC

- D_2PI_ULS_F32

- D_MTRTRQCMDHILMT_MTRNM_F32

- D_ONE_ULS_F32

- Module specific Lookup Tables Constants

- Functions/Macros Used By the Sub-Modules

- Library Functions / Macros

- The library and functions / Macros that are called by the various sub modules are identified below,

- LPF_KUpdate_f32_m

- LPF_OpUpdate_f32_m

- HPF_KUpdate_f32_m

- HPF_OpUpdate_f32_m

- FPM_FloatToFixed_m

- FPM_FixedToFloat_m

- IntplVarXY_u16_u16Xu16Y_Cnt

- BilinearXYM_s16_s16Xs16YM_Cnt

- Rte_Call_NxtrDiagMgr_SetNTCStatus

- Data Hiding Functions

- Global Functions/Macros Defined by this Module

- Local Functions/Macros Used by this MDD only

- Local Function #1

- Function Name

- DriverVelCalc

- Arguments Passed

- HwTorque_HwNm_T_f32

- CRFMotorVel_MtrRadpS_T_f32

- VehicleSpeed_Kph_T_f32

- Return Value

- ScaledDriverVel_MtrRadpS_T_s14p1

- EMBED Visio.Drawing.11

- Calculate ADD Coefficient

- BaseAssistCmd_MtrNm_T_f32

- WIRCmdAmpBlnd_MtrNm_T_f32

- VehicleLonAccel_KphpS_T_f32

- ADDCoefCalc_MtrNmSpRad_T_u0p16

- Calculate Filter Coefficients

- FilterCoefCalc

- filtCoef_Uls_T_Str

- filterCoef_T*

- N/A (address)

- Outputs Returned (by reference)

- filtCoef_Uls_T_Str->b0_Uls_ s0p15

- filtCoef_Uls_T_Str->b1_Uls_ u0p16

- filtCoef_Uls_T_Str->b2_Uls_ s0p15

- filtCoef_Uls_T_Str->a0_Uls_ u2p14

- filtCoef_Uls_T_Str->a1_Uls_s4p11

- filtCoef_Uls_T_Str->a2_Uls_u5p11

- Generate Command

- *filtCoef_Uls_Str

- b0_Uls_ s0p15

- b1_Uls_ u0p16

- b2_Uls_ s0p15

- a0_Uls_ u2p14

- a1_Uls_s4p11

- a2_Uls_u5p11

- Compenstation_MtrNm_T_ s11p20

- Unit Testing Considerations

- This function is designed to work with argument values from the calling function as used with the other functions in the module, and outputs may be out of the expected range if tested with arbitrary combinations of input values. Unit testing of this function should use only passed argument value combinations coming from the calling function.

- Software Module Implementation

- Runtime Environment (RTE) Initial Values

- This section lists the initial values of data written by this module but controlled by the RTE. After RTE initialization, the data in this table will contain these values.

- Rte_InitValue_AsstFirewallActive_Uls_f32

- Rte_InitValue_CombinedDamping_MtrNm_f32

- Rte_InitValue_DampingCmd_MtrNm_f32

- Rte_InitValue_HwTorque_HwNm_f32

- Rte_InitValue_InertiaComp_MtrNm_f32

- Rte_InitValue_MtrVelCRF_MtrRadpS_f32

- Rte_InitValue_VehicleSpeed_Kph_f32

- Rte_InitValue_ BaseAssistCmd_MtrNm_f32

- Rte_InitValue _WIRCmdAmpBlnd_MtrNm_f32

- Rte_InitValue _ VehicleLonAccel_KphpS_f32

- Rte_InitValue _ FreqDepDmpSrlComSvcDft_Cnt_lgc

- Initialization Functions

- DOCPROPERTY "Module Name" \* MERGEFORMAT

- DampingFirewall

- Design Rationale

- Module Internal

- Initialize Filters

- Periodic Functions

- Program Flow Start

- Rte_Call_ActivePull_Per1_CP0_CheckpointReached()

- Store Module Inputs to Local copies

- DefeatDampingSvc_Cnt_T_lgc = Rte_IRead_DampingFirewall_Per1_Defeat_Damping_Svc_Cnt_lgc()

- MECCounter_Cnt_T_enum = Rte_IRead_DampingFirewall_Per1_MEC_Counter_Cnt_enum()

- AsstFirewallActive_Uls_T_f32 = Rte_IRead_DampingFirewall_Per1_AsstFirewallActive_Uls_f32()

- DampingCmd_MtrNm_T_f32 = Rte_IRead_DampingFirewall_Per1_DampingCmd_MtrNm_f32()

- HwTorque_HwNm_T_f32 = Rte_IRead_DampingFirewall_Per1_HwTorque_HwNm_f32()

- InertiaComp_MtrNm_T_f32 = Rte_IRead_DampingFirewall_Per1_InertiaComp_MtrNm_f32()

- MtrVelCRF_MtrRadpS_T_f32 = Rte_IRead_DampingFirewall_Per1_MtrVelCRF_MtrRadpS_f32()

- VehicleSpeed_Kph_T_f32 = Rte_IRead_DampingFirewall_Per1_VehicleSpeed_Kph_f32()

- BaseAsstCmd_MtrNm_T_f32 = Rte_IRead_DampingFirewall_Per1_BaseAssistCmd_MtrNm_f32()

- WIRCmdAmpBlnd_MtrNm_T_f32 = Rte_IRead_DampingFirewall_Per1_WIRCmdAmpBlnd_MtrNm_f32()

- FDDDefSrvFlg_Cnt_T_lgc = Rte_IRead_DampingFirewall_Per1_FreqDepDmpSrlComSvcDft_Cnt_lgc()

- VehicleLonAccel_KphpS_T_f32 = Rte_IRead_DampingFirewall_Per1_VehicleLonAccel_KphpS_f32()

- DampFWPstepNstep_Cnt_T_str.PStep = k_DampFWPstep_Cnt_u16

- DampFWPstepNstep_Cnt_T_str.NStep = k_DampFWNstep_Cnt_u16

- DampFWPstepNstep_Cnt_T_str.Threshold = t_DampFWPNstepThresh_Cnt_u16[1]

- DampFWInrtCmpPstepNstep_Cnt_T_str.PStep = k_DampFWInCmpPStep_Cnt_u16

- DampFWInrtCmpPstepNstep_Cnt_T_str.NStep = k_DampFWInCmpNStep_Cnt_u16

- DampFWInrtCmpPstepNstep_Cnt_T_str.Threshold = t_DampFWDampInrtCmpPNThesh_Cnt_u16[1]

- Damping Limiter

- Interpolate and Filter Boundaries

- Additional Damping

- Store Local copy of outputs into Module Outputs

- DampFWUprBound_MtrNm_D_f32 = UprBoundRaw_MtrNm_T_f32

- Rte_IWrite_DampingFirewall_Per1_CombinedDamping_MtrNm_f32(CombinedDamping_MtrNm_T_f32)

- Program Flow End

- Rte_Call_ActivePull_Per1_CP1_CheckpointReached()

- Fault Recovery Functions

- Shutdown Functions

- Interrupt Functions

- Serial Communication Functions

- Execution Requirements

- Execution Sequence of the Module

- DampingFirewall_Per1 is called at a rate of 2 ms.

- Execution Rates for sub-modules called by the Scheduler

- This table serves as reference for the Scheduler design

- Calling Frequency

- System State(s) in which the function is called

- DampingFirewall_Init1

- DampingFirewall_Per1

- OPERATE, DISABLE

- Execution Requirements for Serial Communication Functions

- Sub-Module called by (Serial Comm Function Name)

- Memory Map Definition Requirements

- Sub Modules (Functions)

- This table identifies the software segments for functions identified in this module.

- Name of Sub Module

- RTE_START_SEC_AP_DAMPINGFIREWALL_APPL_CODE

- Local Functions

- This table identifies the software segments for local functions identified in this module.

- AP_DAMPINGFIREWALL_CODE

- Known Issues / Limitations With Design

- INLINE functions defined in GlobalMacro.h are not unit tested.

- Due to the requirement to use fixed point arithmetic in the

- diverse implementation

- of SF-14 (VBIC), precision of some calculations, especially of the filter coefficients and especially at the extremes of the input ranges, is significantly less than the resolution of the data types of the variables. For example, the a0 coefficient is stored in a variable with 2^-14 resolution, but the a0 min value is accurate to approximately 2^-6 as compared to the expected results of the same c

- Agreed with the FDD owner Scott Millsap to leave the resolutions of calconstants as they are in v11.2 of implementation.

- Revision Control Log

- Change Description

- Author Initials

- Initial Version

- Fixed UTP Issues (naming consistency)

- Fixed calibration naming conflict

- Anomaly 3324 (using wrong value for boundary calc), fixed units in names

- Updated to SF-35 v002 (anomaly 3325)

- Updated to SF-35 v003

- Updated to SF-35 v004

- Updated to SF-35 V005

- Updated to SF-35 V006. Removed input limit on inertia comp input for VBIC limiter. Added multiple display variables. Variable name changes for state variables for filter.

- Added watchdog checkpoints

- Corrected software segments of internal variables

- MDD updates based on UTP catch up

- Anom 3957- VBICFaultmode is not set

- Updates as per the implementation of v007 of the FDD

- Updates for anomaly 4407

- Updates for anomaly 4809

- Anomaly 4913 fixes

- VBIC Error filter robustness change

- Updated to SF-35 Ver 008, Generate Cmd calculations changed to fixed point

- Updated to SF-35 Ver 009, undone Generate Cmd fixed point changes and merged 14.1.1 changes

- Updated to SF-35 Ver 010

- add filtering on LwrBound and UprBound

- A5206 anomaly fix

- Corrections for issues found in UTP

- Additional corrections for issues found in unit test

- Changed ranges of filter coefficients to account for fixed point math and worst case inputs, and added design limitation regarding resolution of filter coefficient calculations.

- A6259 anomaly fix

- Updated the Rates and State execution; QAC cleanup

- Fix for anomalies EA3#5983 and those associated with CompCR EA3#8741

- SOFTWARE MODULE DESIGN SPECIFICATION

- DOCPROPERTY "Product Line" \* MERGEFORMAT

- Gen II+ EPS EA3

- 14-Juan-20165

- Spandana BalaniKrishna Anne

- DOCPROPERTY "Company" \* MERGEFORMAT

- CONFIDENTIAL

- MDD Template EA3, Rev 1.1

- {wkw\kw\PL\L

- xtlhldl`t\t\t

- }y}u}u}u}q}y}

- wskgkgkgkgb^
