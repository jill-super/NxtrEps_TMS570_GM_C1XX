---
title: "BatteryVoltage — Battery_Voltage_MDD"
description: "Converted .doc document from BatteryVoltage/doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/BatteryVoltage/doc/Battery_Voltage_MDD.doc`.

- Module -- Battery Voltage

- DOCVARIABLE "MDDRevNum" \* MERGEFORMAT

- High-Level Description

- This module is responsible for applying voltage and time based hysteresis to the battery voltage to determine over voltage and low voltage faults.

- Function Data Sharing

- This diagram shows all data that is shared between functions within the module.

- Variable Data Dictionary

- For details on module input / output variable, refer to the Data Dictionary for the application. Input / output variable names are listed here for reference.

- (Note: Full variable names required in table.)

- (Note: All global variables including End Of Line data used should be shown here)

- Module Inputs (Global Variable Name)

- Module Outputs (Global Variable Name)

- Batt_Volt_f32

- VswitchClosed_Cnt_lgc

- BattSwitched_Volt_f32

- Vecu_Volts_f32

- SysCVSwitch_Volt_f32

- SysC_Vecu_Volt_f32

- Module Internal Variables

- This section identifies the name, range and resolutions for module specific data created by this module. If there are no range restrictions on the variable, the term

- is placed into the table for legal range.

- Variable Name

- User Defined Type

- Software Segment

- Vecu_Volts_M_f32

- BATTERYVOLTAGE_START_SEC_VAR_CLEARED_32

- VswitchClosed_Cnt_M_lgc

- BATTERYVOLTAGE_START_SEC_VAR_CLEARED_BOOLEAN

- VswitchCorrLimDiff_Volts_D_f32

- VecuVbatCorrLimDiff_Volts_D_f32

- VswitchCorrErrAcc_Cnt_M_u16

- BATTERYVOLTAGE_START_SEC_VAR_CLEARED_16

- VecuVbatCorrErrAcc_Cnt_M_u16

- Vbatt_Volts_M_f32

- OvervoltageFaultSet_Cnt_M_lgc

- User defined typedef definition/declaration

- This section documents any user types uniquely used for the module.

- Typedef Name

- Element Name

- Constant Data Dictionary

- Calibration Constants

- This section lists the calibrations used by the module. For details on calibration constants, refer to the Data Dictionary for the application.

- Constant Name

- k_MaxSwitchedVolt_Volts_f32

- k_MaxBattVoltDiff_Volts_f32

- k_VswitchCorrLim_Cnt_Str

- k_VecuCorrLim_Cnt_Str

- k_VecuVbatCorrLim_Volts_f32

- k_VswitchCorrLim_Volts_f32

- Program(fixed) Constants

- Embedded Constants

- All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

- D_VSWITCHEDTHRESH_ULS_F32

- Single precision floating point

- D_VECUMAX_VOLTS_F32

- This section lists the global constants used by the module. For details on global constants, refer to the Data Dictionary for the application.

- D_VECUMIN_VOLTS_F32

- BC_BATTERYVOLTAGE_FAULTINJECTIONPOINT

- FLTINJ_VECU_BATTERYVOLTAGE

- Module specific Lookup Tables Constants

- (This is for lookup tables (arrays) with fixed values, same name as other tables)

- Functions/Macros used by the Sub-Modules

- Library Functions / Macros

- The library functions / Macros that are called by the various sub modules are identified below,

- FPM_FloatToFixed_m()

- Data Hiding Functions

- The data hiding functions / macros used in this module are identified below,

- Rte_Call_NxtrDiagMgr_SetNTCStatus()

- Rte_Call_Batt_Batt_V_f32()

- Rte_Call_BattSwitched_BattSwitched_V_f32

- Rte_Call_SysC_Vswitch_BattSwitched_V_f32

- Rte_Call_BatteryVoltage_Per1_CP0_CheckpointReached

- Rte_Call_BatteryVoltage_Per1_CP1_CheckpointReached

- Rte_Call_BatteryVoltage_Per2_CP0_CheckpointReached

- Rte_Call_BatteryVoltage_Per2_CP1_CheckpointReached

- Rte_Pim_OvervoltageData()

- Rte_Call_OvervoltageData_SetRamBlockStatus()

- Local Functions/Macros Used by this MDD only

- (Note if they are defined in another source file, then reference the appropriate header file)

- The local functions/macros in this module are identified below,

- Software Module Implementation

- Initialization Functions

- Module state variables are initialized to 0 at start-up by RAM init.

- Init: BatteryVoltage_Init1

- Design Rationale

- Program Flow Start

- Store Module Inputs to Local copies

- EMBED Visio.Drawing.11

- Store Local copy of outputs into Module Outputs

- Program Flow End

- Periodic Functions

- Per: BatteryVoltage_Per1

- See FDD 08B.

- Rte_Call_BatteryVoltage_Per1_CP0_CheckpointReached()

- Vbatt_Volts_T_f32 = Rte_IRead_BatteryVoltage_Per2_Batt_Volt_f32()

- Vswitched_Volts_T_f32 = Rte_IRead_BatteryVoltage_Per1_BattSwitched_Volt_f32()

- Perform Over and Low Voltage Diagnostics

- Vecu_Volts_M_f32 = Vecu_Volts_T_f32

- Vbatt_Volts_M_f32 = Vbatt_Volts_T_f32

- Rte_IWrite_BatteryVoltage_Per1_ VswitchClosed _Cnt_lgc(VswitchClosed_Cnt_T_lgc)

- Rte_IWrite_BatteryVoltage_Per1_ Vecu _Volts_f32(Vecu_Volts_T_f32)

- Rte_IWrite_BatteryVoltage_Per1_SysC_Vecu_Volt_f32(Vecu_Volts_M_f32)

- Rte_Call_BatteryVoltage_Per1_CP1_CheckpointReached()

- Per: BatteryVoltage_Per2

- Rte_Call_BatteryVoltage_Per2_CP0_CheckpointReached()

- VecuVbatCorrLimDiff_Volts_T_f32 =0

- NTCSysFailCtrlV_T_lgc = FALSE

- Vswitched_Volts_T_f32 = Rte_IRead_BatteryVoltage_Per2_BattSwitched_Volt_f32()

- SysCVswitch_Volts_T_f32 = Rte_IRead_BatteryVoltage_Per2_SysCVSwitch_Volt_f32()

- VSwitch and Vecu cross correlation diagnostics

- VswitchCorrLimDiff_Volts_D_f32 = VswitchCorrLimDiff_Volts_T_f32

- VecuVbatCorrLimDiff_Volts_D_f32 = VecuVbatCorrLimDiff_Volts_T_f32

- Rte_Call_BatteryVoltage_Per2_CP1_CheckpointReached()

- Fault Recovery Functions

- Shutdown Functions

- Interrupt Functions

- NoneIsr: Isr_OvervoltThresh

- Serial Communication Functions

- SCom: BatteryVoltage_SCom_ClearTransOvData

- Function Name

- BatteryVoltage_SCom_ClearTransOvData

- Arguments Passed

- Return Value

- Store Module Inputs to Local Copies

- Clear Transient Overvoltage Data Service

- Store Local Copy of outputs into Module Outputs

- BatteryVoltage_SCom_ReadTransOvData

- *OvervoltageCounter_Cnt_u16

- *MaxBattVoltage_Volts_f32

- Read Transient Overvoltage Data Service

- Local Function/Macro Definitions

- If these are numerous and defined in a separate source file then reference the source file only.

- Execution Requirements

- Execution Sequence of the Module

- (Describe in words relevant details about the execution sequence of the different sub modules.)

- Execution Rates for sub-modules called by the Scheduler

- This table serves as reference for the Scheduler design

- Calling Frequency

- System State(s) in which the function is called

- BatteryVoltage_Init1

- BatteryVoltage_Per1

- BatteryVoltage_Per2

- Isr_OvervoltThresh

- Execution Requirements for Serial Communication Functions

- Sub-Module called by (Serial Comm Function Name)

- EPS_DiagSrvc

- Memory Map Definition Requirements

- Sub Modules (Functions)

- This table identifies the software segments for functions identified in this module.

- Name of Sub Module

- RTE_AP_BATTERYVOLTAGE_APPL_CODE

- BatteryVoltage_Per1()

- BatteryVoltage_Per2()

- BatteryVoltage_SCom_ClearTransOvData()

- BatteryVoltage_SCom_ReadTransOvData()

- Local Functions

- This table identifies the software segments for local functions identified in this module.

- Known Issues / Limitations With Design

- Revision Control Log

- Change Description

- Author Initials

- Initial AutoSAR release.

- Updated to meet FDD 08B rev 02 Ecu Voltage

- Corrected execution states for periodic

- s to global constants

- s global constants names per latest NTC definitions

- Updated as per FDD Ver 004

- changed from client server port type to Sender/Receiver port

- MDD updates for UTP catchups

- Checked in the right version of the MDD into synergy

- Updated to FDD Ver 005

- Updated to FDD Ver 006 and anomaly 5138 correction

- Added missing ISR function for overvoltage diagnostic (A5789)

- Add BATTERYVOLTAGE_REPORTERRORSTATUS for program specific integration.

- SOFTWARE MODULE DESIGN SPECIFICATION

- Battery Voltage

- DOCPROPERTY "Product Line" \* MERGEFORMAT

- 83-Jan-1426-Jun-13

- Jared Julien

- Nexteer CONFIDENTIAL

- S/W module design template, Rev 3.0a

- rngncn\XnQMQ
