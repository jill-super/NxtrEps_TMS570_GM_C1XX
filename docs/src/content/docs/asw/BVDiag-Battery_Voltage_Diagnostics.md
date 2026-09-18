---
title: "BVDiag — Battery_Voltage_Diagnostics"
description: "Converted .doc document from BVDiag/doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/BVDiag/doc/Battery_Voltage_Diagnostics.doc`.

- Module -- Battery Voltage

- DOCVARIABLE "MDDRevNum" \* MERGEFORMAT

- High-Level Description

- This module is responsible for applying voltage and time based hysteresis to the battery voltage to determine over voltage(B5) and low voltage faults(B0). Requirements for all these faults are detailed in SER.

- Function Data Sharing

- This diagram shows all data that is shared between functions within the module.

- Variable Data Dictionary

- For details on module input / output variable, refer to the Data Dictionary for the application. Input / output variable names are listed here for reference.

- (Note: Full variable names required in table.)

- (Note: All global variables including End Of Line data used should be shown here)

- Module Inputs (Global Variable Name)

- Module Outputs (Global Variable Name)

- Batt_Batt_V_f32

- Module Internal Variables

- This section identifies the name, range and resolutions for module specific data created by this module. If there are no range restrictions on the variable, the term

- is placed into the table for legal range.

- Variable Name

- User Defined Type

- Software Segment

- LowSetInitBD_ms_M_u32p0

- LowClrInitBD_ms_M_u32p0

- OvSetInitBD_ms_M_u32p0

- OvClrInitBD_ms_M_u32p0

- User defined typedef definition/declaration

- This section documents any user types uniquely used for the module.

- Typedef Name

- Element Name

- Constant Data Dictionary

- Calibration Constants

- This section lists the calibrations used by the module. For details on calibration constants, refer to the Data Dictionary for the application.

- Constant Name

- k_OvDetect_Volts_u10p6

- k_OvNotDetect_Volts_u10p6

- k_OvDetect_ms_u16p0

- k_OvNotDetect_ms_u16p0

- k_LowNotDetect_Volts_u10p6

- k_LowDetect_Volts_u10p6

- k_LowDetect_ms_u16p0

- k_LowNotDetect_ms_u16p0

- Program(fixed) Constants

- Embedded Constants

- All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

- D_ABOVEMAX_CNT_U16

- D_BELOWMIN_CNT_U16

- D_INDEADBAND_CNT_U16

- D_DIAGOV_CNT_U16

- D_DIAGLOW_CNT_U16

- This section lists the global constants used by the module. For details on global constants, refer to the Data Dictionary for the application.

- NTC_Num_OpVoltage

- NTC_Num_OpVoltageOvrMax

- Module specific Lookup Tables Constants

- (This is for lookup tables (arrays) with fixed values, same name as other tables)

- Functions/Macros used by the Sub-Modules

- Library Functions / Macros

- The library functions / Macros that are called by the various sub modules are identified below,

- Data Hiding Functions

- The data hiding functions / macros used in this module are identified below,

- Rte_Call_NxtrDiagMgr_SetNTCStatus()

- Rte_Call_BVDiag_Per1_CP0_CheckpointReached

- Rte_Call_BVDiag_Per1_CP1_CheckpointReached

- Local Functions/Macros Used by this MDD only

- (Note if they are defined in another source file, then reference the appropriate header file)

- The local functions/macros in this module are identified below,

- ApplyHysteresis()

- ControlTimers()

- Software Module Implementation

- Initialization Functions

- Module state variables are initialized to 0 at start-up by RAM init.

- Periodic Functions

- Per: BVDiag_Per1

- Design Rationale

- Check BMW or K2XX SER. Both describes same functionality for B0,B5

- Program Flow Start

- Rte_Call_BVDiag_Per1_CP0_CheckpointReached()

- Store Module Inputs to Local copies

- BattVoltage_Volts_T_f32 = Rte_IRead_BVDiag_Per1_Batt_Volt_f32()

- Perform Over and Low Voltage Diagnostics

- EMBED Visio.Drawing.11

- Store Local copy of outputs into Module Outputs

- Program Flow End

- Fault Recovery Functions

- Shutdown Functions

- Interrupt Functions

- Serial Communication Functions

- Local Function/Macro Definitions

- If these are numerous and defined in a separate source file then reference the source file only.

- Control Timers

- Function Name

- ControlTimers

- Arguments Passed

- BattVoltage_Volts_T_u10p6

- CompareType_T_u16

- UpperCal_T_u10p6

- LowerCal_T_u10p6

- SetTimer_T_ptr

- ClrTimer_T_ptr

- SetTimer_ms_T_u16p0

- ClrTimer_ms_T_u16p0

- Option_T_u16

- Return Value

- See data dictionary for input which corresponds to a calibration or global variable

- This generic local function is used to control set and clear timers for the diagnostic functions as well as control flags used to indicate battery voltage is

- for the application. Data is passed to indicate the following:

- CompareType_T_u16:

- Passed data to indicate the type of comparison to be made internally to the function (Above Max or Below Min). Used in a decision block within the function. Essentially, reverses the logic between an over voltage test (where below min is a normal operating point) and low voltage test (where above max is a normal operating point)

- UpperCal_T_u10p6:

- Voltage level calibration of the hysteresis (upper threshold).

- LowerCal_T_u10p6:

- Voltage level calibration of the hysteresis (lower threshold). Note: Lower cal must be <= Upper Cal.

- SetTimer_T_ptr:

- Pointer to the appropriate module specific 32-bit set timer under test (examples are set timer for over voltage, low voltage, battery Ok, etc.)

- ClrTimer_T_ptr:

- Pointer to the appropriate module specific 32-bit clear timer under test (examples are set timer for over voltage, low voltage, battery Ok, etc.)

- SetTimer_ms_T_u16p0:

- Calibration used for the time based hysteresis to set the condition. Note that the calibrations will differ for set timers for over voltage, low voltage, etc.

- ClrTimer_ms_T_u16p0:

- Calibration used for the time based hysteresis to clear the condition. Note that the calibrations will differ for set timers for over voltage, low voltage, etc.

- Option_T_u16:

- Identifies which function is being used to identify which set fault, clear fault functions to call, which battery voltage OK state is being checked, etc.

- Apply Hysteresis

- ApplyHysteresis

- BattIn_T_u10p6

- HighCal_T_u10p6

- LowCal_T_u10p6

- OutputZone_T_u16

- This local function is used to determine the next state for a voltage based hysteresis as applied to the battery voltage level. Data is passed to include the battery voltage, upper calibration and a lower calibration. The function returns the state of the battery voltage relative to the cals (either

- ). Note that the design requires the upper cal to be larger than the lower cal for proper operation.

- Execution Requirements

- Execution Sequence of the Module

- (Describe in words relevant details about the execution sequence of the different sub modules.)

- Execution Rates for sub-modules called by the Scheduler

- This table serves as reference for the Scheduler design

- Calling Frequency

- System State(s) in which the function is called

- Execution Requirements for Serial Communication Functions

- Sub-Module called by (Serial Comm Function Name)

- Memory Map Definition Requirements

- Sub Modules (Functions)

- This table identifies the software segments for functions identified in this module.

- Name of Sub Module

- BVDiag_Per1()

- RTE_AP_BVDIAG_APPL_CODE

- Local Functions

- This table identifies the software segments for local functions identified in this module.

- AP_BVDIAG_CODE

- Known Issues / Limitations With Design

- B1,B4 faults are removed from BMW,K2XX SER.

- Revision Control Log

- Change Description

- Author Initials

- Initial AutoSAR release.

- SOFTWARE MODULE DESIGN SPECIFICATION

- Battery Voltage

- DOCPROPERTY "Product Line" \* MERGEFORMAT

- Niveditha Reddy

- Nexteer CONFIDENTIAL

- S/W module design template, Rev 3.0a
