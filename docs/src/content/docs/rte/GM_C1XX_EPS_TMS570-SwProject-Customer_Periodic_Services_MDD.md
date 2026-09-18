---
title: "Integration — doc/Customer_Periodic_Services_MDD"
description: "Converted document Customer_Periodic_Services_MDD.doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/GM_C1XX_EPS_TMS570/SwProject/CustPerSrvcs/doc/Customer_Periodic_Services_MDD.doc`.

- Customer Specific Periodic Services

- High-Level Description

- The Customer Specific Periodic Services module takes care of the processing that has to be achieved to meet customer diagnostic services requirements.

- Component Diagram

- Variable Data Dictionary

- For details on module input / output variable, refer to the Data Dictionary for the application. Input / output variable names are listed here for reference.

- Module Inputs (Global Variable Name)

- Module Outputs (Global Variable Name)

- ThermalLimitFlagCntr_Cnt_u08

- Note: Any input signals that are not listed in the

- Module Inputs

- section above but shown in the component diagram as a receiver port are dummy signals which are used to determine loss of a certain message when data receive error event is triggered.

- Module Internal Variables

- This section identifies the name, range and resolutions for module specific data created by this module. If there are no range restrictions on the variable, the term

- is placed into the table for legal range.

- Variable Name

- Software Segment

- ThermalLimitFlagCntr_Cnt_M_u08

- CUSTPERSRVCS_START_SEC_VAR_SAVED_ZONEH_8

- ThermalLimitFlagClearCntr_Cnt_M_u08

- PrevThermalLimitFlagStatus_Cnt_M_u08

- CUSTPERSRVCS_START_SEC_VAR_CLEARED_8

- LTCompValBefReset_HwNm_M_f32

- Single Precision Float

- CUSTPERSRVCS_START_SEC_VAR_CLEARED_32

- CCWEOTPosBefReset_HwDeg_M_f32

- CWEOTPosBefReset_HwDeg_M_f32

- CCWEOTFndBefReset_Cnt_M_lgc

- CUSTPERSRVCS_START_SEC_VAR_CLEARED_BOOLEAN

- CWEOTFndBefReset_Cnt_M_lgc

- WriteEOTValAftRst_Cnt_M_lgc

- WriteLTCompValAftRst_Cnt_M_lgc

- User defined typedef definition/declaration

- This section documents any user types uniquely used for the module.

- Typedef Name

- Element Name

- User Defined Type

- Constant Data Dictionary

- Calibration Constants

- This section lists the calibrations used by the module. For details on calibration constants, refer to the Data Dictionary for the application.

- Constant Name

- Program(fixed) Constants

- Embedded Constants

- All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

- D_TESTFAILED_CNT_U08

- D_TESTNOTCOMPTHISOPCYCLE_CNT_U08

- D_MAXCLEARCOUNT_CNT_U08

- This section lists the global constants used by the module. For details on global constants, refer to the Data Dictionary for the application.

- Module specific Lookup Tables Constants

- (This is for lookup tables (arrays) with fixed values, same name as other tables)

- Functions/Macros used by the Sub-Modules

- Library Functions / Macros

- The library functions / Macros that are called by the various sub modules are identified below,

- Rte_Call_NxtrDiagMgr_GetNTCStatus

- ActivePull_SCom_ReadParam

- ActivePull_SCom_SetLTComp

- Data Hiding Functions

- The data hiding functions / macros used in this module are identified below,

- Local Functions/Macros Used by this MDD only

- (Note if they are defined in another source file, then reference the appropriate header file)

- The local functions/macros in this module are identified below,

- Software Module Implementation

- Runtime Environment (RTE) Initial Values

- This section lists the initial values of data written by this module but controlled by the RTE. After RTE initialization, the data in this table will contain these values.

- Rte_InitValue_ ThermalLimitFlagCntr_Cnt_u08

- Initialization Functions

- Init: CustPerSrvcs_Init1

- Design Rationale

- Permit the fault counter to clear after a number of ignition cycles without a fault.

- Program Flow Start

- EMBED Visio.Drawing.11

- Program Flow End

- Periodic Functions

- Per: CustPerSrvcs_Per1TuningSelAuth_Per1

- Rte_Call_CustPerSrvcs_Per1_CP0_CheckpointReached();

- Store Module Inputs to Local copies

- See below section

- Store Local copy of outputs into Module Outputs

- See above section

- Rte_Call_CustPerSrvcs_Per1_CP1_CheckpointReached();

- Periodic Event Triggered Functions

- Fault Recovery Functions

- Shutdown Functions

- Interrupt Functions

- Serial Communication Functions

- CustPerSrvcs_SCom_ResetThrmlCntr

- Arguments Passed

- Return Value

- See section above.

- CustPerSrvcs_Scom_ReadActivePullParam

- CustPerSrvcs_Scom_ReadLrnEOTParam

- Transition Functions

- CustPerSrvcs_Trns1

- Execution Requirements

- Execution Sequence of the Module

- The calling frequency for Per1 is chosen as shown below because the fault for which the status being retrieved sets/ clears every 100ms. CustPerSrvcs_Trns1 must execute prior to states and modes OFF transition function execution.

- Execution Rates for sub-modules called by the Scheduler

- This table serves as reference for the Scheduler design

- Function Name

- Calling Frequency

- System State(s) in which the function is called

- CustPerSrvcs_Per1

- On Entering OFF

- Execution Requirements for Serial Communication Functions

- Sub-Module called by (Serial Comm Function Name)

- CustPerSrvcs_Scom_ResetThrmlCntr

- RTE_AP_CUSTPERSRVCS_APPL_CODE

- Memory Map Definition Requirements

- Sub Modules (Functions)

- This table identifies the software segments for functions identified in this module.

- Name of Sub Module

- Local Functions

- This table identifies the software segments for local functions identified in this module.

- Known Issues / Limitations With Design

- Revision Control Log

- Change Description

- Author Initials

- Initial Version

- Added ThermalLimitFlagClearCntr logic

- SOFTWARE MODULE DESIGN SPECIFICATION

- DOCPROPERTY "Product Line" \* MERGEFORMAT

- Lucas WendlingBlake Latchford (zz4r1x)

- Nexteer CONFIDENTIAL

- S/W module design template, Rev 3.0a

- lh\M>M\M\M>Ml
