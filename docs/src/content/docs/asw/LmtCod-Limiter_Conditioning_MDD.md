---
title: "LmtCod — Limiter_Conditioning_MDD"
description: "Converted .doc document from LmtCod/doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/LmtCod/doc/Limiter_Conditioning_MDD.doc`.

- Limiter Conditioning

- High-Level Description

- This MDD describes the summation of all assist and limit terms used in an Electric Power Steering application.

- Component Diagram

- Variable Data Dictionary

- For details on module input / output variable, refer to the Data Dictionary for the application. Input / output variable names are listed here for reference.

- Module Inputs

- Module Outputs

- AssistEOTGain_Uls_f32

- EOTGainLtd_Uls_f32

- AssistEOTLimit_MtrNm_f32

- EOTLimitLtd_MtrNm_f32

- AssistStallLimit_MtrNm_f32

- OutputRampMultLtd_Uls_f32

- AssistVehSpdLimit_MtrNm_f32

- StallLimitLtd_MtrNm_f32

- OutputRampMult_Uls_f32

- ThermalLimitLtd_MtrNm_f32

- ThermalLimit_MtrNm_f32

- VehSpdLimitLtd_MtrNm_f32

- VehicleSpeed_Kph_f32

- CCLTrqRamp_Uls_f32

- Module Internal Variables

- This section identifies the name, range and resolutions for module specific data created by this module. If there are no range restrictions on the variable, the term

- is placed into the table for legal range.

- Variable Name

- Software Segment

- CurrAssistEOTGain_Uls_M_f32

- Single Precision Float

- LMTCOD_START_SEC_VAR_CLEARED_32

- CurrOutputRampMult_Uls_M_f32

- CurrAssistEOTLimit_MtrNm_M_f32

- CurrAssistStallLimit_MtrNm_M_f32

- Single Precision Floating Point

- CurrAssistVehSpdLimit_MtrNm_M_f32

- CurrThermalLimit_MtrNm_M_f32

- CCLTrqRamp_Uls_M_f32

- User defined typedef definition/declaration

- This section documents any user types uniquely used for the module.

- Typedef Name

- Element Name

- User Defined Type

- Constant Data Dictionary

- Calibration Constants

- This section lists the calibrations used by the module. For details on calibration constants, refer to the Data Dictionary for the application.

- Constant Name

- k_GainDecSlew_UlspS_f32

- k_TorqueDecSlew_MtrNmpS_f32

- t_GainIncSlewTblX_Kph_u9p7[2]

- t_GainIncSlewTblY_UlspS_u9p7[2]

- t_TorqueIncSlewTblX_Kph_u9p7[2]

- t_TorqueIncSlewTblY_MtrNmpS_u13p3[2]

- k_CCLTrqRampIncSlew_UlspS_f32

- Program(fixed) Constants

- Embedded Constants

- All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

- This section lists the global constants used by the module. For details on global constants, refer to the Data Dictionary for the application.

- D_2MS_SEC_F32

- FLTINJ_ASSTEOTGAIN_LMTCOD

- FLTINJ_OUTPUTRAMPMULT_LMTCOD

- FLTINJ_ASSTEOTLIMIT_LMTCOD

- BC_LMTRCONDN_FAULTINJECTIONPOINT

- Module specific Lookup Tables Constants

- (This is for lookup tables (arrays) with fixed values, same name as other tables)

- Functions/Macros used by the Sub-Modules

- Library Functions / Macros

- The library and functions / Macros that are called by the various sub modules are identified below,

- Sign_f32_m()

- IntplVarXY_u16_u16Xu16Y_Cnt()

- FPM_FloatToFixed_m()

- FPM_FixedToFloat_m()

- Data Hiding Functions

- Global Functions/Macros Defined by this Module

- Local Functions/Macros Used by this MDD only

- Software Module Implementation

- Runtime Environment (RTE) Initial Values

- This section lists the initial values of data written by this module but controlled by the RTE. After RTE initialization, the data in this table will contain these values.

- Rte_InitValue_AssistEOTGain_Uls_f32

- Rte_InitValue_AssistEOTLimit_MtrNm_f32

- Rte_InitValue_AssistStallLimit_MtrNm_f32

- Rte_InitValue_AssistVehSpdLimit_MtrNm_f32

- Rte_InitValue_OutputRampMult_Uls_f32

- Rte_InitValue_ThermalLimit_MtrNm_f32

- Rte_InitValue_EOTGainLtd_Uls_f32

- Rte_InitValue_EOTLimitLtd_MtrNm_f32

- Rte_InitValue_OutputRampMultLtd_Uls_f32

- Rte_InitValue_StallLimitLtd_MtrNm_f32

- Rte_InitValue_ThermalLimitLtd_MtrNm_f32

- Rte_InitValue_VehSpdLimitLtd_MtrNm_f32

- Rte_InitValue_VehicleSpeed_Kph_f32

- Rte_InitValue_CCLTrqRamp_Uls _f32

- Initialization Functions

- Periodic Functions

- Per: LmtCod_Per1

- Design Rationale

- This function provides a layer of protection from erroneous signals feeding into SF-04 Sum & Limit. It is applied primarily to

- signals that serve to reduce motor torque command under certain operating conditions. This function can prevent step response or

- behavior that might cause undesirable vehicle feel. It includes capability of fault injection at some inputs to facilate tuning. See FDD SF-38 for more details.

- Program Flow Start

- Rte_Call_LmtCod_Per1_CP0_CheckpointReached()

- Store Module Inputs to Local copies

- Module Input Name

- AssistEOTGain_Uls_T_f32

- Rte_IRead_LmtCod_Per1_AssistEOTGain_Uls_f32

- AssistEOTLimit_MtrNm_T_f32

- Rte_IRead_LmtCod_Per1_AssistEOTLimit_MtrNm_f32

- AssistStallLimit_MtrNm_T_f32

- Rte_IRead_LmtCod_Per1_AssistStallLimit_MtrNm_f32

- AssistVehSpdLimit_MtrNm_T_f32

- Rte_IRead_LmtCod_Per1_AssistVehSpdLimit_MtrNm_f32

- OutputRampMult_Uls_T_f32

- Rte_IRead_LmtCod_Per1_OutputRampMult_Uls_f32

- ThermalLimit_MtrNm_T_f32

- Rte_IRead_LmtCod_Per1_ThermalLimit_MtrNm_f32

- VehicleSpeed_Kph_T_f32

- Rte_IRead_LmtCod_Per1_VehicleSpeed_Kph_f32

- _CCLTrqRamp_Uls _T_f32

- Rte_IRead_LmtCod_Per1_CCLTrqRamp_Uls _f32

- (Processing of function)

- EMBED Visio.Drawing.11

- Store Local copy of outputs into Module Outputs

- Module Output Name

- Rte_IWrite_LmtCod_Per1_EOTGainLtd_Uls_f32

- Rte_IWrite_LmtCod_Per1_EOTLimitLtd_MtrNm_f32

- FinalCurrOutputRampMult_Uls_T_f32CurrOutputRampMult_Uls_M_f32

- Rte_IWrite_LmtCod_Per1_OutputRampMultLtd_Uls_f32

- Rte_IWrite_LmtCod_Per1_StallLimitLtd_MtrNm_f32

- Rte_IWrite_LmtCod_Per1_ThermalLimitLtd_MtrNm_f32

- Rte_IWrite_LmtCod_Per1_VehSpdLimitLtd_MtrNm_f32

- Program Flow End

- Rte_Call_LmtCod_Per1_CP1_CheckpointReached()

- Fault Recovery Functions

- Shutdown Functions

- Interrupt Functions

- Serial Communication Functions

- Execution Requirements

- Execution Sequence of the Module

- Execution Rates for sub-modules called by the Scheduler

- This table serves as reference for the Scheduler design

- Function Name

- Calling Frequency

- System State(s) in which the function is called

- Execution Requirements for Serial Communication Functions

- Sub-Module called by (Serial Comm Function Name)

- Memory Map Definition Requirements

- Sub Modules (Functions)

- This table identifies the software segments for functions identified in this module.

- Name of Sub Module

- LmtCod_Per1()

- RTE_START_SEC_AP_LMTCOD_APPL_CODE

- Local Functions

- This table identifies the software segments for local functions identified in this module.

- Known Issues / Limitations With Design

- INLINE functions defined in globalmacro.h are not unittested.

- Revision Control Log

- Change Description

- Author Initials

- Document creation for component based design process

- Check points corrected

- Update to FDD SF38 v002

- Update to FDD SF38 v003

- Changed the init value of

- SOFTWARE MODULE DESIGN SPECIFICATION

- DOCPROPERTY "Product Line" \* MERGEFORMAT

- SAVEDATE \@ "d-MMM-yy" \* MERGEFORMAT

- Selva Sengottaiyan(rz3h1n)

- DOCPROPERTY "Company" \* MERGEFORMAT

- CONFIDENTIAL

- S/W module design template, Rev 2.2b+

- |pl]pQpEpEp]

- }yuyuynjnyfb^bfbfyWSWyI

- ~zvrv~hbhWhbhbhWh~Q~
