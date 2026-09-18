---
title: "EtDmpFw — EOTDampingFirewall_MDD"
description: "Converted .doc document from EtDmpFw/doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/EtDmpFw/doc/EOTDampingFirewall_MDD.doc`.

- EOTDampingFirewall

- High-Level Description

- This MDD describes the summation of all assist and limit terms used in an Electric Power Steering application.

- Component Diagram

- Variable Data Dictionary

- For details on module input / output variable, refer to the Data Dictionary for the application. Input / output variable names are listed here for reference.

- Module Inputs

- Module Outputs

- AssistEOTDamping_MtrNm_f32

- EOTDampingLtd_MtrNm_f32

- CRFMtrVel_MtrRadpS_f32

- HandwheelAuthority_Uls_f32

- HandwheelPosition_HwDeg_f32

- Vehicle_Speed_Kph_f32

- EOTDisable_Cnt_lgc

- MEC_Counter_Cnt_enum

- Module Internal Variables

- This section identifies the name, range and resolutions for module specific data created by this module. If there are no range restrictions on the variable, the term

- is placed into the table for legal range.

- Variable Name

- Software Segment

- EOTDmpFWActvLtd_MtrNm_D_f32

- Single Precision Float

- ETDMPFW_START_SEC_VAR_CLEARED_32

- EOTDmpFWInActvLtd_MtrNm_D_f32

- UprBndActive_MtrNm_D_f32

- LwrBndActive_MtrNm_D_f32

- Single Precision Floating Point

- EOTDmpFWActvRegion_Cnt_D_lgc

- ETDMPFW_START_SEC_VAR_CLEARED_BOOLEAN

- EOTDmpFWHWAuth_Cnt_D_lgc

- EOTDmpFWMode_Cnt_M_u08

- ETDMPFW_START_SEC_VAR_CLEARED_08

- User defined typedef definition/declaration

- This section documents any user types uniquely used for the module.

- Typedef Name

- Element Name

- User Defined Type

- Constant Data Dictionary

- Calibration Constants

- This section lists the calibrations used by the module. For details on calibration constants, refer to the Data Dictionary for the application.

- Constant Name

- k_EOTDmpFWInputLim_MtrNm_f32

- k_MinRackTrvl_HwDeg_u12p4

- t2_EOTPosDepDmpTblX_HwDeg_u12p4

- k_EOTDynConf_Uls_u8p8

- t_EOTDmpFWActiveBoundX_MtrRadpS_s11p4t_EOTDmpFWActUprBndX_MtrRadpS_s11p4

- t2_EOTDmpFWActiveBoundY_MtrNm_s7p8t_EOTDmpFWActUprBndY_MtrNm_s7p8

- k_EOTDmpFWInactiveLim_MtrNm_f32

- t_EOTDmpFWActLwrBndX_MtrRadpS_s11p4

- t_EOTDmpFWActLwrBndY_MtrNm_s7p8

- t_EOTDmpFWVehSpd_Kph_u9p7

- Program(fixed) Constants

- Embedded Constants

- All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

- D_INACTIVEREGION_ULS_U08

- D_ACTIVEREGION_ULS_U08

- D_FIREWALLLDISABLED_ULS_U08

- This section lists the global constants used by the module. For details on global constants, refer to the Data Dictionary for the application.

- D_ZERO_ULS_F32

- D_ONE_ULS_F32

- D_MTRTRQCMDHILMT_MTRNM_F32

- D_MTRTRQCMDLOLMT_MTRNM_F32

- BC_ETDMPFW_FAULTINJECTIONPOINT

- FLTINJ_EOTDAMPING_ETDMPFW

- D_NEGONE_CNT_S16

- D_FALSE_CNT_LGC

- Module specific Lookup Tables Constants

- (This is for lookup tables (arrays) with fixed values, same name as other tables)

- Functions/Macros used by the Sub-Modules

- Library Functions / Macros

- The library and functions / Macros that are called by the various sub modules are identified below,

- Sign_f32_m()

- BilinearXYM_s16_s16Xs16YM_Cnt()

- FPM_FloatToFixed_m()

- Data Hiding Functions

- Global Functions/Macros Defined by this Module

- Local Functions/Macros Used by this MDD only

- Software Module Implementation

- Runtime Environment (RTE) Initial Values

- This section lists the initial values of data written by this module but controlled by the RTE. After RTE initialization, the data in this table will contain these values.

- Rte_InitValue_AssistEOTDamping_MtrNm_f32

- Rte_InitValue_CRFMtrVel_MtrRadpS_f32

- Rte_InitValue_EOTDampingLtd_MtrNm_f32

- Rte_InitValue_HandwheelAuthority_Uls_f32

- Rte_InitValue_HandwheelPosition_HwDeg_f32

- Initialization Functions

- Periodic Functions

- Per: EtDmpFw_Per1

- Design Rationale

- Program Flow Start

- Rte_Call_EtDmpFw_Per1_CP0_CheckpointReached()

- Store Module Inputs to Local copies

- Module Input Name

- AsstEOTDamping_MtrNm_T_f32

- Rte_IRead_EtDmpFw_Per1_AssistEOTDamping_MtrNm_f32

- HandwheelPosition_HwDeg_T_f32

- Rte_IRead_EtDmpFw_Per1_HandwheelPosition_HwDeg_f32

- HandwheelAuthority_Uls_T_f32

- Rte_IRead_EtDmpFw_Per1_HandwheelAuthority_Uls_f32

- CRFMtrVel_MtrRadpS_T_f32

- Rte_IRead_EtDmpFw_Per1_CRFMtrVel_MtrRadpS_f32

- VehicleSpeed_Kph_T_f32

- Rte_IRead_EtDmpFw_Per1_Vehicle_Speed_Kph_f32

- EOTDisable_Cnt_T_lgc

- Rte_IRead_EtDmpFw_Per1_EOTDisable_Cnt_lgc

- MECCounter_Cnt_T_enum

- Rte_IRead_EtDmpFw_Per1_MEC_Counter_Cnt_enum

- VehicleSpeed_Kph_T_u9p7

- FPM_FloatToFixed_m(VehicleSpeed_Kph_T_f32, u9p7_T)

- (Processing of function)

- EMBED Visio.Drawing.11

- Store Local copy of outputs into Module Outputs

- Module Output Name

- LimitedEOTDamping_MtrNm_T_f32

- Rte_IWrite_EtDmpFw_Per1_EOTDampingLtd_MtrNm_f32

- Program Flow End

- Rte_Call_EtDmpFw_Per1_CP1_CheckpointReached()

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

- EtDmpFw_Per1

- Execution Requirements for Serial Communication Functions

- Sub-Module called by (Serial Comm Function Name)

- Memory Map Definition Requirements

- Sub Modules (Functions)

- This table identifies the software segments for functions identified in this module.

- Name of Sub Module

- RTE_START_SEC_AP_ETDMPFW_APPL_CODE

- Local Functions

- This table identifies the software segments for local functions identified in this module.

- Known Issues / Limitations With Design

- INLINE functions defined in globalmacro.h are not unittested.

- Revision Control Log

- Change Description

- Author Initials

- Document creation for component based design process

- Added watchdog checkpoints

- Corrected for static variable software section

- Updated as per FDDVer002, FaultInjectionPoint added to AsstEOTDamping_MtrNm_T_f32 signal

- Updated to SF-27 v003

- SOFTWARE MODULE DESIGN SPECIFICATION

- EOTDamping Firewall

- DOCPROPERTY "Product Line" \* MERGEFORMAT

- SAVEDATE \@ "d-MMM-yy" \* MERGEFORMAT

- 16-May-1329-Jan-13

- Selva Sengottaiyan

- DOCPROPERTY "Company" \* MERGEFORMAT

- CONFIDENTIAL

- S/W module design template, Rev 2.2b+
