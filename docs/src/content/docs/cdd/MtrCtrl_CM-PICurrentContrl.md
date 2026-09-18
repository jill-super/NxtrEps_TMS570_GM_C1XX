---
title: "MtrCtrl_CM — PICurrentContrl"
description: "Converted .doc document from MtrCtrl_CM/doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/MtrCtrl_CM/doc/PICurrentContrl.doc`.

- Module -- PICurrCntrl

- High-Level Description

- Non-AUTOSAR PI driver required to perform EPS motor control PWM profiles.

- Function Data Sharing

- This diagram shows all data that is shared between functions within the module.

- Module Inputs and Outputs

- For details on module input / output variable, refer to the Data Dictionary for the application. Input / output variable names are listed here for reference.

- (Note: Full variable names required in table.)

- (Note: All global variables including End Of Line data used should be shown here)

- Module Inputs (Global Variable Name)

- Module Outputs (Global Variable Name)

- Refer the Data Dictionary

- Module Internal Variables

- This section identifies the name, range and resolutions for module specific data created by this module. If there are no range restrictions on the variable, the term

- is placed into the table for legal range.

- (Note: If no module specific variables are used by the design, place the text

- in the first Variable Name cell in the table)

- Variable Name

- Software Segment

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

- (Note: If no calibrations are used by the design, place the text

- in the first location in the table)

- Constant Name

- Program(fixed) Constants

- Embedded Constants

- All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

- D_SCALERADTOCNTS_ULS_F32

- Single Precision Float

- 10430.3783505F

- D_REVWITHROUND_ULS_F32

- D_ROUND_ULS_F32

- D_DEG2RAD_ULS_F32

- 0.0174532925199F

- D_GAIN_ULS_F32

- D_VECUMAX_VOLTS_F32

- D_SQRT3OVR2_ULS_F32

- D_MTRCTRLISRRATE_MS_F32

- D_MTRCURRMIN_AMP_F32

- D_MTRCURRMAX_AMP_F32

- D_VECUDEFAULT_VOLT_F32

- This section lists the global constants used by the module. For details on global constants, refer to the Data Dictionary for the application.

- D_ZERO_ULS_F32

- D_VECUMIN_VOLTS_F32

- Module specific Lookup Tables Constants

- (This is for lookup tables (arrays) with fixed values, same name as other tables)

- Functions/Macros used by the Sub-Modules

- Library Functions / Macros

- The library functions / Macros that are called by the various sub modules are identified below,

- IntplVarXY_u16_u16Xu16Y_Cnt_m()

- FPM_FloatToFixed_m

- Data Hiding Functions

- The data hiding functions / macros used in this module are identified below,

- Rte_ModeType_StaMd_Mode

- MtrCntrl_Read_MtrCurrQax_Amp_f32

- MtrCntrl_Read_MtrCurrDax_Amp_f32

- MtrCntrl_Read_Vecu_Volt_f32

- MtrCntrl_Read_ModIdxSrlComSvcDft_Cnt_lgc

- MtrCntrl_Read_SysState_Cnt_Enum

- MtrCntrl_Read_MtrCurrOffComOffset_Cnt_u16

- MtrCntrl_Read_MtrElecPol_Cnt_s8

- MtrCntrl_Read_MtrPosElec_Rev_u0p16

- MtrCntrl_Write_MtrCurrQaxFinalRef_Amp_f32

- MtrCntrl_Write_MtrDaxVoltage_Volt_f32

- MtrCntrl_Write_MtrQaxVoltage_Volt_f32

- MtrCntrl_Write_ModIdx_Uls_u16p16

- MtrCntrl_Write_PhaseAdvanceFinal_Rev_u0p16

- MtrCntrl_Write_CommOffset_Cnt_u16

- Local Functions/Macros Used by this MDD only

- Header file: Ap_MtrCntrl_Cfg.h

- Software Module Implementation

- Initialization Functions

- PICurrCntrl_MtrCurrDaxSatFluxRatio_Uls_M_f32 =D_ONE_ULS_F32

- PICurrCntrl_MtrCurrQaxSatFluxRatio_Uls_M_f32 =D_ONE_ULS_F32

- Initialise the output for State variables for Vecu filter:

- PICurrCntrl_MtrVecuFilt_M_str.PrevOutput_Uls_f32 = D_VECUDEFAULT_VOLT_F32

- PICurrCntrl_MtrVecuFilt_M_str.PrevInput_Uls_f32 = D_VECUDEFAULT_VOLT_F32

- Initialise the Bilinear Filter:

- CalLowPassFiltBilinearTerm(k_MtrVoltVecuFiltKn_Hz_f32, k_PiSamplingTs_Sec_f32 ,&PICurrCntrl_MtrVecuFilt_M_str)

- CalLowPassFiltBilinearTerm(k_MtrVoltQaxFiltFFKn_Hz_f32, k_PiSamplingTs_Sec_f32 ,&PICurrCntrl_MtrVoltQaxFFFilt_M_str)

- Periodic Functions

- Per: PICurrCntrl_Per1

- Design Rationale

- This function is responsible for calculating the amount of current to be supplied to the motor. To control the PWM profiles generated for the motor. FastDataAccessBufIndex allows the buffer synchronization between data calculated on slower periodic loop time(2 milli seconds) and are read by faster periodic run time (ie 0.125ms)

- Store Module Inputs to Local copies

- MtrCntrl_Read_MtrCurrQax_Amp_f32(&MtrCurrQax_Amp_T_f32);

- MtrCntrl_Read_MtrCurrDax_Amp_f32(&MtrCurrDax_Amp_T_f32);

- MtrCntrl_Read_Vecu_Volt_f32(&Vecu_Volt_T_f32);

- MtrCntrl_Read_ModIdxSrlComSvcDft_Cnt_lgc(&ModIdxSrlComSvcDft_Cnt_T_lgc);

- MtrCntrl_Read_SysState_Cnt_Enum(&SysState_Cnt_T_Enum);

- FwdDataAcessBuffer_Cnt_T_u16= (ActWriteAccBufIndex_Cnt_T_u16)

- MtrCurrQaxRef_Amp_T_f32=MtrCurrQaxRef_Amp_M_f32[FwdDataAcessBuffer_Cnt_T_u16];

- MtrCurrDaxRef_Amp_T_f32=MtrCurrDaxRef_Amp_M_f32[FwdDataAcessBuffer_Cnt_T_u16];

- PIDaxIntegralGain_Uls_T_f32=MtrDaxIntegralGain_Uls_M_f32[FwdDataAcessBuffer_Cnt_T_u16];

- PIDaxPropotionalGain_Uls_T_f32=MtrDaxPropotionalGain_Uls_M_f32[FwdDataAcessBuffer_Cnt_T_u16]

- PIQaxIntegralGain_Uls_T_f32=MtrQaxIntegralGain_Uls_M_f32[FwdDataAcessBuffer_Cnt_T_u16];

- PIQaxPropotionalGain_Uls_T_f32=MtrQaxPropotionalGain_Uls_M_f32[FwdDataAcessBuffer_Cnt_T_u16]

- ElecPosDelayComp_Rad_T_f32=MtrPosComputationDelay_Rad_M_f32[FwdDataAcessBuffer_Cnt_T_u16]

- MtrVoltDaxFF_Volt_T_f32=MtrVoltDaxFF_Volt_M_f32[FwdDataAcessBuffer_Cnt_T_u16]MtrVoltQaxFF_Volt_T_f32=MtrVoltQaxFF_Volt_M_f32[FwdDataAcessBuffer_Cnt_T_u16];

- Program Flow Start

- Refer FDD for flowcharts

- Store Local copy of outputs into Module Outputs

- MtrCntrl_Write_MtrCurrQaxFinalRef_Amp_f32(MtrCurrQaxFinalRef_Amp_T_f32)

- MtrCntrl_Write_MtrDaxVoltage_Volt_f32(MtrDaxVoltage_Volt_T_f32)

- MtrCntrl_Write_MtrQaxVoltage_Volt_f32(MtrQaxVoltage_Volt_T_f32)

- MtrCntrl_Write_ModIdx_Uls_u16p16(FPM_FloatToFixed_m(ModIdx_Uls_T_u16p16))

- MtrCntrl_Write_PhaseAdvanceFinal_Rev_u0p16(PhaseAdvanceFinal_Rev_T_u0p16)

- MtrCntrl_Write_CommOffset_Cnt_u16(CommOffset_Cnt_T_u16)

- MtrCntrl_Write_MtrVolt_Volt_f32(MtrVoltCmdFinal_Volt_T_f32)

- MtrCntrl_Write_MtrCurrDaxIntg_Volt_f32(MtrCurrDaxIntg_Volt_T_f32)

- MtrCntrl_Write_MtrCurrQaxIntg_Volt_f32(MtrCurrQaxIntg_Volt_T_f32)

- MtrCurrQaxFinalRef_Amp_M_f32[SlowDataAccessBufIndex_Cnt_M_u16]= MtrCurrQaxFinalRef_Amp_T_f32;

- MtrVoltDax_Volt_M_f32[SlowDataAccessBufIndex_Cnt_M_u16] = MtrDaxVoltage_Volt_T_f32;

- MtrVoltQax_Volt_M_f32[SlowDataAccessBufIndex_Cnt_M_u16] = MtrQaxVoltage_Volt_T_f32

- Program Flow End

- Per: PICurrCntrl_Per2

- This function is responsible for calculating the amount of current to be supplied to the motor. To control the PWM profiles generated for the motor.

- SlowDataAccessBufIndex allows the buffer synchronization between data calculated on faster periodic loop time(125 micro seconds) and are read by slower periodic run time (ie 2ms)

- ReadBuffer_Cnt_T_u16 = SlowDataAccessBufIndex_Cnt_M_u16

- WriteBuffer_Cnt_T_u16 = (ReadBuffer_Cnt_T_u16 & 1U) ^ 1U

- SlowDataAccessBufIndex_Cnt_M_u16 = WriteBuffer_Cnt_T_u16

- EstKe_VpRadpS_T_f32= Rte_IRead_PICurrCntrl_Per2_EstKe_VpRadpS_f32();

- EstR_Ohm_T_f32 = Rte_IRead_PICurrCntrl_Per2_EstR_Ohm_f32();

- MRFMtrVel_MtrRadpS_T_f32 = Rte_IRead_PICurrCntrl_Per2_MRFMtrVel_MtrRadpS_f32();

- CorrMtrPosElec_Rev_T_f32 = Rte_IRead_PICurrCntrl_Per2_CorrMtrPosElec_Rev_f32();

- MtrCurrDaxRef_Amp_T_f32 = Rte_IRead_PICurrCntrl_Per2_MtrCurrDaxRef_Amp_f32();

- MtrVoltDax_Volt_T_f32 = MtrVoltDax_Volt_M_f32[ReadBuffer_Cnt_T_u16];

- MtrVoltQax_Volt_T_f32 = MtrVoltQax_Volt_M_f32[ReadBuffer_Cnt_T_u16];

- MtrCurrQaxFinalRef_Amp_T_f32 = MtrCurrQaxFinalRef_Amp_M_f32[ReadBuffer_Cnt_T_u16];

- Rte_Call_PICurrCntrl_Per2_CP0_CheckpointReached()

- EMBED Visio.Drawing.11

- Rte_IWrite_PICurrCntrl_Per2_DervLambdaAlphaDiag_Volt_f32(DervLambdaAlphaDiag_Volt_T_f32);

- Rte_IWrite_PICurrCntrl_Per2_DervLambdaBetaDiag_Volt_f32(DervLambdaBetaDiag_Volt_T_f32);

- Rte_Call_PICurrCntrl_Per2_CP1_CheckpointReached()

- Local Functions

- Local Function #1

- Function Name

- CalLowPassFiltBilinearOut

- Arguments Passed

- Input_Uls_T_f32

- *LowPassFiltBilinear_T_Str

- Return Value

- Output_Uls_T_f32

- Local Function #2 CalLowPassFiltBilinearTerm

- CalLowPassFiltBilinearTerm

- Freq_Hz_T_f32

- TimeCons_Sec_T_f32

- LowPassFiltBilinear_T_Str

- Local Function #3 IntegralStateVarNonOperState

- IntegralStateVarNonOperState

- SysState_Cnt_T_Enum

- Local Function #4 CalLowPassFiltVecuOut

- CalLowPassFiltVecuOut

- *Vecu_Volt_T_f32

- Local Function #5 LoaMtgtnSclFac

- LoaMtgtnSclFac

- MotCurrLoaMtgtnEn_Cnt_T_lgc

- IvtrLoaMtgtnEn_Cnt_T_lgc

- Execution Requirements

- Execution Sequence of the Module

- Execution Rates for sub-modules called by the Scheduler

- This table serves as reference for the Scheduler design

- Calling Frequency

- System State(s) in which the function is called

- PICurrCntrl_Per1

- PICurrCntrl_Per2

- Execution Requirements for Serial Communication Functions

- Sub-Module called by (Serial Comm Function Name)

- Memory Map Definition Requirements

- Sub Modules (Functions)

- This table identifies the software segments for functions identified in this module.

- Name of Sub Module

- PICurrCntrl_CODE

- RTE_START_SEC_AP_PICURRCNTRL_APPL_CODE

- This table identifies the software segments for local functions identified in this module.

- - Denotes functions that are vector call-backs only included to avoid compiler errors.

- Known Issues / Limitations With Design

- The computation of commoffset and ModIndex service defeat part of FDD15D is implemented in this component inaddition to 99B requirements

- The reason for the implementation is to keep the sine voltage driver common across components

- Revision Control Log

- Change Description

- Author Initials

- Initial release with changes for IPM

- Changes for memap statements added

- Updated for SF99B

- v8 with only changes needed for voltage command

- integrity check for torque reasonableness

- Corrected for SF99B

- Updated for V12 of FDD SF99

- Updated for V15 of FDD SF99

- Updated for V17 of FDD SF99 EA3#A283,EA3#1777 fixed

- Updated as per unit test findings

- Updated for V18 of FDD SF99

- NEXT GENERATION SOFTWARE DESIGN

- MODULE DESIGN SPECIFICATION

- Gen II Plus - EA3.0

- 20-Aug-1518-March-2016

- Selva Sengottaiyan

- DELPHI CONFIDENTIAL

- S/W module design template, Rev 2.2

- sfVfVFfVFfVFfV
