---
title: "GMSrlComOutput — Serial_Communication_Output_MDD"
description: "Converted .doc document from GMSrlComOutput/doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/GMSrlComOutput/doc/Serial_Communication_Output_MDD.doc`.

- Serial Communications Output

- High-Level Description

- The Serial Communications Output module provides a signal level interface between the EPS application layer and the serial communications software. Provide for the network management functionality for the serial communications interface. This module will be customized for each distinct vehicle platform. This module will be responsible for converting the range and resolution of the Application Laye

- This module processes the data for transmit signals that are sent from the EPS controller to other ECUs on the communication bus. Global application input data is scaled appropriately and then transferred to the serial communications Interaction Layer using function calls or macros provided. Similarly, the Serial Communications Input module, takes the signal data that is received from the Interact

- Component Diagram

- This diagram shows all data that is shared between functions within the module.

- Variable Data Dictionary

- For details on module input / output variable, refer to the Data Dictionary for the application. Input / output variable names are listed here for reference.

- (Note: Full variable names required in table.)

- Module Inputs (Global Variable Name)

- Module Outputs (Global Variable Name)

- LKATrqDelivered_HwNm_f32

- BusOffCE_Cnt_lgc

- HwTrq_HwNm_f32

- BusOffHS_Cnt_lgc

- LKAState_State_enum

- HOWEstimate_Uls_f32

- SrlComHwPosStatus_Cnt_u16

- SrlComHwPos_HwDeg_f32

- HwVelValid_Cnt_lgc

- APADrvrInterventionDetected_Cnt_lgc

- APAState_State_enum

- Rte_TrqOvlSta_TrqOvlStaMfgEnable_Cnt_b08

- TrimCompEOL_Cnt_lgc

- HandwheelVel_HwRadpS_f32

- ESCState_State_enum

- ESCTorqueDelivered_HwNm_f32

- DiagRmpToZeroActive_Cnt_lgc

- DiagStsHwPosDis_Cnt_lgc

- SrlComSysPwrMd_Cnt_enum

- Module Internal Variables

- This section identifies the name, range and resolutions for module specific data created by this module. If there are no range restrictions on the variable, the term

- is placed into the table for legal range.

- Variable Name

- Software Segment

- DTCTriggeredFlag_Cnt_M_lgc[DEM_MAX_NUMBER_EVENT_ENTRY + 1]

- See Data Dictionary

- SRLCOMOUTPUT_START_SEC_VAR_CLEARED_UNSPECIFIED

- SRLCOMOUTPUT_START_SEC_VAR_SAVED_ZONEH_UNSPECIFIED

- DTCFailed_Cnt_M_lgc[DEM_MAX_NUMBER_EVENT_ENTRY + 1]

- CurrentDTCSentThisIC_Cnt_M_lgc

- BusOffPresentChannel0_Cnt_M_lgc

- BusOffPresentChannel1_Cnt_M_lgc

- BusOffDiagActiveChannel0_Cnt_M_lgc

- BusOffDiagActiveChannel1_Cnt_M_lgc

- CTCEventId_Cnt_M_u8

- SRLCOMOUTPUT_START_SEC_VAR_CLEARED_8

- CTCEventIdSV_Cnt_M_u8

- GMStatus_Cnt_M_u8[D_NUMOFDEMEVENTS_CNT_U08 + 1]

- LastReportedDTCEventID_Cnt_M_u8

- StartTimerToSetDTCFlag_mS_M_u32p0

- SRLCOMOUTPUT_START_SEC_VAR_CLEARED_32

- DemDTCNum_Cnt_M_u32[DEM_MAX_NUMBER_EVENT_ENTRY + 1]

- PwrStrIOLmpCmdSV_Cnt_M_lgc

- StrAsstRedLmpCmdSV_Cnt_M_lgc

- LastReportedGMStatus_Cnt_M_u8

- LKATrqOvrlDlvdRC_Cnt_M_u8

- DrvStrIntfrDetARC_Cnt_M_u08

- ElcPwrStrAvalStatARC_Cnt_M_u08

- StWhlAngAliveRollCnt_Cnt_M_u08

- ESCRollCount_Cnt_T_u08

- DemDTCNum_Cnt_M_u32[D_NUMOFDEMEVENTS_CNT_U08 + 1U]

- BusOffFltChannel0RecoverTimer_mS_M_u32

- BusOffFltChannel0DetectionTimer_mS_M_u32

- BusOffFltChannel1RecoverTimer_mS_M_u32

- BusOffFltChannel1DetectionTimer_mS_M_u32

- PrevWarningIndSignal_Cnt_M_u08[DEM_NUMBER_OF_INDICATORS]

- 3.1.1 User defined typedef definition/declaration

- This section documents any user types uniquely used for the module.

- Typedef Name

- Element Name

- User Defined Type

- RT_DTC_Triggered_778

- DTCTriggered

- DTCWrnIndRqdSt

- DTCTstFldPwrUpSt

- DTCTstNPsdPwrupSt

- DTCTstNPsdPwrUpSt

- DTCTstFldCdClrdStat

- DTCTstNPsdCdClrdSt

- DTCCurrentStatus

- DTCCodeSupported

- DTCFaulttype

- DTCFaultType

- Constant Data Dictionary

- Calibration Constants

- This section lists the calibrations used by the module. For details on calibration constants, refer to the Data Dictionary for the application.

- Constant Name

- k_MaxHOWEstimate_Uls_f32

- k_SComTrqPosPol_Cnt_s08

- k_LKAMfgEnable_Cnt_lgc

- k_APAMfgEnable_Cnt_lgc

- k_BusOffFaultTimeChannel0_mS_u16

- k_BusOffRecoveryTimeChannel0_mS_u16

- k_BusOffFaultTimeChannel1_mS_u16

- k_BusOffRecoveryTimeChannel1_mS_u16

- Program(fixed) Constants

- Embedded Constants

- All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

- D_TESTFAILED_CNT_U8

- D_FAILEDTHISCYC_CNT_U8

- D_CONFIRMED_CNT_U8

- D_TESTNCTHISCYC_CNT_U8

- D_WARNINGIND_CNT_U8

- D_EPSSOURCEID_CNT_U16

- Dem_Warning_Indicator * (defined in Dem.h)

- Dem_Steering_Reduced_Assist * (defined in Dem.h)

- D_NUMOFDEMEVENTS_CNT_U08

- D_HWPOSSTATUSVALID_CNT_U16

- D_APAMFGENABLE_CNT_U08

- D_INVALID_CNT_U08

- D_VALID_CNT_U08

- D_ENABLED_CNT_U08

- D_FAILED_CNT_U08

- D_LKAACTIVE_CNT_U08

- D_HANDSON_CNT_U08

- D_HANDSOFF_CNT_U08

- D_DISABLED_CNT_U08

- D_LKAMFGENABLE_CNT_U08

- D_LKADRIVERAPPLIEDTORQUESF_NM_F32

- D_LKADRIVERAPPLIEDTORQUEMAX_NM_F32

- D_LKATRQDELIVEREDSF_NM_F32

- D_LKATRQDELIVEREDMIN_NM_F32

- D_LKATRQDELIVEREDMAX_NM_F32

- D_TOTALTORQUESF_NM_F32

- D_TOTALTORQUEMIN_NM_F32

- D_TOTALTORQUEMAX_NM_F32

- D_USEDATA_CNT_U08

- D_DONTUSEDATA_CNT_U08

- D_SENSORTYPE4_CNT_u08

- D_CALSTATUNKNOWN_CNT_U08

- D_CALSTATCALIBRATED_CNT_U08

- D_STRWHANGSCALE_ULS_F32

- D_STRWHANGLOLMT_ULS_F32

- D_STRWHANGHILMT_ULS_F32

- D_STRWHANGGRDLOLMT_ULS_F32

- D_STRWHANGGRDHILMT_ULS_F32

- D_WARNINGINDSTEERINGREDUCEDASSIST2_ENABLED

- This section lists the global constants used by the module. For details on global constants, refer to the Data Dictionary for the application.

- D_180OVRPI_ULS_F32

- Module specific Lookup Tables Constants

- (This is for lookup tables (arrays) with fixed values, same name as other tables)

- Functions/Macros used by the Sub-Modules

- Library Functions / Macros

- The library functions / Macros that are called by the various sub modules are identified below,

- Data Hiding Functions

- The data hiding functions / macros used in this module are identified below,

- Dem_GetIndicatorStatus

- IlPutTxPwrStrIO

- IlPutTxStrngAsstRdcdIO

- IlPutTxStrAngSnsChksm_1

- IlPutTxStrAngSnsChksm_0

- IlPutTxStrWhAngGrdGroup_1

- IlPutTxStrWhAngGroup_1

- IlPutTxStrWhAngGrdGroup_0

- IlPutTxStrWhAngGroup_0

- IlPutTxStrWhAngGrd_1

- IlPutTxStrWhAngGrd_0

- IlPutTxStrWhAng_1

- IlPutTxStrWhAng_0

- IlPutTxStrWhlAngSenTyp_1

- IlPutTxStrWhlAngSenTyp_0

- IlPutTxStWhlAngAliveRollCnt_1

- IlPutTxStWhlAngAliveRollCnt_0

- IlPutTxStrWhlAngSenCalStat_1

- IlPutTxStrWhlAngSenCalStat_0

- IlPutTxStrWhAngGrdV_1

- IlPutTxStrWhAngGrdMsk_1

- IlPutTxStrWhAngGrdV_0

- IlPutTxStrWhAngGrdMsk_0

- IlPutTxStrWhAngV_1

- IlPutTxStrWhAngMsk_1

- IlPutTxStrWhAngV_0

- IlPutTxStrWhAngMsk_0

- IlPutTxDTCI_DTCFaultType_778

- IlPutTxLKADrvAppldTrqGroup

- IlPutTxHndsOffStrWhlDtStGroup

- Rte_Call_SystemTime_DtrmnElapsedTime_mS_u16

- Rte_Call_SystemTime_GetSystemTime_mS_u32

- Rte_Call_NxtrDiagMgr_GetNTCActive

- IlPutTxElecPwrStrAvalStat

- IlPutTxDrvStrIntfrDtcdV

- IlPutTxDrvStrIntfrDtcd

- IlPutTxDrvStrIntfrDetARC

- IlPutTxDrvStrIntfrDetPrtVal

- IlPutTxElcPwrStrAvalStatARC

- IlPutTxElcPwrStrAvalStatPVal

- IlPutTxDrvStrIntfrDtcdGroup

- CanPartOffline

- CanPartOnline

- IlPutTxElPwrStTtlTqDlrd

- IlPutTxTrqOvrlTrqDStat

- IlPutTxTrqOvrlDvrdARC

- IlPutTxTrqOvrlDltTrqDlrd

- IlPutTxTrqOvrlDChksm

- Rte_Call_NxtrDiagMgr_SetNTCStatus

- 51. Rte_Pim_DTCTrigSts[D_NUMOFDEMEVENTS_CNT_U08]

- IlPutTxStrAsstRdcdLvl2IO

- Local Functions/Macros Used by this MDD only

- (Note if they are defined in another source file, then reference the appropriate header file)

- The local functions/macros in this module are identified below,

- ISOToGMStatus()

- SrlComOuput_BusOffHandlerInit()

- SrlComOutput_BusOffHandler(P2VAR(boolean, AUTOMATIC, AUTOMATIC) BusOffHS_Cnt_T_lgc, P2VAR(boolean, AUTOMATIC, AUTOMATIC) BusOffCE_Cnt_T_lgc)

- SrlComOutput_WarningIndicatorHandler(Dem_IndicatorIdType Dem_IndicatorId)

- : Flow charts are not being updated as no value add observed.

- Software Module Implementation

- Initialization Functions

- Init: SrlComOutput_Init1

- Design Rationale

- Request Full Communication mode.

- Module Internal

- EMBED Visio.Drawing.11

- Module Outputs

- Program Flow End

- Periodic Functions

- Per: SrlComOutput_Per1

- Process and update Transmit signal data.

- Program Flow Start

- Store Module Inputs to Local copies

- See section below

- Store Local copy of outputs into Module Outputs

- See section above.

- Per: SrlComOutput_Per2

- Rte_Read_SrlComHwPos_HwDeg_f32(&SrlComHwPos_HwDeg_T_f32)

- Rte_Read_SrlComHwPosStatus_Cnt_u16(&SrlComHwPosStatus_Cnt_T_u16)

- Rte_Read_HandwheelVel_HwRadpS_f32(&HandwheelVel_HwRadpS_f32)

- Rte_Read_HwVelValid_Cnt_lgc(&HandwheelVelValid_Cnt_lgc)

- Rte_Read_TrimCompEOL_Cnt_lgc(&TrimCompEOL_Cnt_lgc)

- Rte_Read_DiagStsHwPosDis_Cnt_lgc(&DiagStsHwPosDis_Cnt_T_lgc)

- Rte_Read_APANonRecoverableFaults_Cnt_lgc(&APAFaultPresent_Cnt_T_lgc)

- Rte_Read_SrlComSysPwrMd_Cnt_enum(&SysPwrMd_Cnt_T_enum)

- 6.2.2.4 Description

- Fault Recovery Functions

- Shutdown Functions

- Interrupt Functions

- Serial Communication Functions

- Transition Functions

- SrlComOutput_Trns1

- Local Function/Macro Definitions

- If these are numerous and defined in a separate source file then reference the source file only.

- ISOToGMStatus

- Function Name

- Arguments Passed

- Return Value

- SrlComOutput_BusOffHandlerInit

- SrlComOutput_BusOffHandler

- SysPwrMd_Cnt_T_enum

- BusOffHS_Cnt_T_lgc,

- P2VAR(boolean, AUTOMATIC, AUTOMATIC)

- BusOffCE_Cnt_T_lgc,

- Appl_1E5MsgTxAck_HS

- CanTransmitHandle

- Appl_1E5MsgTxAck_CE

- ApplNwmBusoff

- CanChannelHandle

- ApplNwmBusoffEnd

- Execution Requirements

- Execution Sequence of the Module

- (Describe in words relevant details about the execution sequence of the different sub modules.)

- Execution Rates for sub-modules called by the Scheduler

- This table serves as reference for the Scheduler design

- Calling Frequency

- System State(s) in which the function is called

- SrlComOutput_Init1()

- SrlComOutput_Per1()

- Not in Mode(s) <OFF>

- SrlComOutput_Per2()

- SrlComOutput_Trns1()

- On Entering OFF

- Execution Requirements for Serial Communication Functions

- Sub-Module called by (Serial Comm Function Name)

- Memory Map Definition Requirements

- Sub Modules (Functions)

- This table identifies the software segments for functions identified in this module.

- Name of Sub Module

- RTE_AP_SRLCOMOUTPUT_APPL_CODE

- AP_SRLCOMOUTPUT_CODE

- Local Functions

- This table identifies the software segments for local functions identified in this module.

- ISOToGMStatus ()

- SrlComOuput_BusOffHandlerInit

- Known Issues / Limitations With Design

- INLINE functions defined in

- GlobalMacro.h

- are not unit tested

- Revision Control Log

- Change Description

- Author Initials

- Initial Version

- Additional changes made after completion of unit test.

- Updates for addition of ESC for SCIR 1G

- A7226: Updated checksum calculation as per new GM spec

- A7322: Updated protection vlue calculation to use "binary add" (OR)

- A7302: Correct HowDetect Mode to report enabled as long as LKA is enabled

- A7487: Corrected protection value calculation (again) to match expectation rather than spec which was misleading.

- A7522: Set LKA status to permanently failed when an F1 or F2 fault is present

- Anomaly fix for ranf of APA state output

- BusOff handler

- MDD Updated as per Unit Test findings.

- MDD updated for anomaly fix done - Bus Off fault being set in Accessory and Off power modes (EA3#2426)

- MDD updated to add Rte_Pim_DTCTrigSts. EA3#2060,EA32338

- Added new 0x148 message signal (warning indicator)

- SOFTWARE MODULE DESIGN SPECIFICATION

- C1XX Serial Communications Output

- DOCPROPERTY "Product Line" \* MERGEFORMAT

- 12-Dec-15093-May-16

- Jared Julien

- Nexteer CONFIDENTIAL

- S/W module design template, Rev 3.0a

- {t{tptptptptptptptptptp

- }p}lh}d}d\XME\>:d
