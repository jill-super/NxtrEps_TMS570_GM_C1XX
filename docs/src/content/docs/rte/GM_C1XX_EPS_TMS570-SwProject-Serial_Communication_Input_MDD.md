---
title: "Integration — doc/Serial_Communication_Input_MDD"
description: "Converted document Serial_Communication_Input_MDD.doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/GM_C1XX_EPS_TMS570/SwProject/SrlComInput/doc/Serial_Communication_Input_MDD.doc`.

- Serial Communications Input

- High-Level Description

- The Serial Communications Input module provides a signal level interface between the EPS application layer and the serial communications software. Provide for the network management functionality for the serial communications interface. This module will be customized for each distinct vehicle platform. This module will be responsible for converting the range and resolution of the Application Layer

- This module processes the data for signals that are received by the EPS controller from other ECUs on the communication bus. Serial Communications signal input data is scaled appropriately and then transferred to the global application data for use by the EPS application software. Similarly, the Serial Communications Output module, takes the global data to the EPS application software scales the d

- Component Diagram

- This diagram shows all data that is shared between functions within the module.

- Variable Data Dictionary

- For details on module input / output variable, refer to the Data Dictionary for the application. Input / output variable names are listed here for reference.

- Module Inputs (Global Variable Name)

- Module Outputs (Global Variable Name)

- ECUResetPerformed_Cnt_G_lgc

- SrlComAmbTemp_DegC_f32

- Rte_TrqOvlSta_TrqOvlStaMfgEnable_Cnt_b08

- SrlComEngTemp_DegC_f32

- RxMsgsSrlComSvcDft_Cnt_lgc

- RespMsgBuffer[]

- WIREnabled_Cnt_lgc

- APARecoverableFaults_Cnt_lgc

- IlNwmGetStatus[]

- APANonRecoverableFaults_Cnt_lgc

- IlNwmStateNormalCommHalted[]

- APARequest_Cnt_lgc

- IlNwmStateNoCommunication[]

- SrlComLatAccel_g_f32

- DiagStsDefVehSpd_Cnt_lgc

- SrlComYawRate_DegpS_f32

- SrlComWIRFltStatus_Cnt_u16

- EngRunAtvForCTCInhibit_Cnt_lgc

- PrevSrlComEngOn_Cnt_lgc

- SrlComLWhlSpd_Hz_f32

- DiagRmpToZeroActive_Cnt_lgc

- SrlComLWhlSpdVld_Cnt_lgc

- BusOffCE_Cnt_lgc

- SrlComRWhlSpd_Hz_f32

- BusOffHS_Cnt_lgc

- SrlComRWhlSpdVld_Cnt_lgc

- SrlComSysPwrMd_Cnt_enum

- SPMForCTCInhibit_Cnt_lgc

- DesiredTunPers_Cnt_u16

- SecureVehicleSpeed_Kph_f32

- LKAInhibit_Cnt_lgc

- LKAFault_Cnt_lgc

- LKACmd_HwNm_f32

- LKARequest_Cnt_lgc

- SrlComVehSpd_Kph_f32

- VehicleSpeedValid_Cnt_lgc

- StrtStopFaultActive_Cnt_lgc

- SrlComEngineSpeed_Rpm_f32

- SrlComEngOn_Cnt_lgc

- SrlComSPMOn_Cnt_lgc

- PosSrvoHwAngle_HwDeg_f32

- PowertrainCrankActive_Cnt_lgc

- ShiftLeverIsInReverse_Cnt_lgc

- HapticRequest_Cnt_lgc

- SrlComVehicleLonAccel_KphpS_f32

- Module Internal Variables

- This section identifies the name, range and resolutions for module specific data created by this module. If there are no range restrictions on the variable, the term

- is placed into the table for legal range.

- Variable Name

- Software Segment

- LastPlsChngTimeL_mS_M_u32

- AP_SRLCOMINPUT_VAR

- LastPlsChngTimeR_mS_M_u32

- InvStartTimeL_mS_M_u32

- InvStartTimeR_mS_M_u32

- OldRawWhlFreqL_Hz_M_f32

- OldRawWhlFreqR_Hz_M_f32

- PulseScale_RevpCnt_M_f32

- WhlTstmpRes_SecpCnt_M_f32

- VehSpdAvgNDrvn_Kph_M_f32

- ManualVehSpd_Kph_M_f32

- AmbTempVldStartTime_mS_M_u32

- AmbTempVldAccum_Cnt_M_u16

- EngTempVldStartTime_mS_M_u32

- EngTempVldAccum_Cnt_M_u16

- LatAccVldStartTime_mS_M_u32

- LatAccVldAccum_Cnt_M_u16

- YawRateVldStartTime_mS_M_u32

- YawRateVldAccum_Cnt_M_u16

- VehSpdVldStartTime_mS_M_u32

- VehSpdVldAccum_Cnt_M_u16

- VehicleDynamicsESCHybCEVldStartTime_mS_M_u32

- VehicleDynamicsESCHybCEVldAccum_Cnt_M_u16

- ParkAssistParallelCEVldStartTime_mS_M_u32

- ParkAssistParallelCEVldAccum_Cnt_M_u16

- VSEActVldAccum_Cnt_M_u16

- TCSysEVldAccum_Cnt_M_u16

- TCSysAVldAccum_Cnt_M_u16

- TrnsShftLvrPosVldAccum_Cnt_M_u16

- ABSFldVldAccum_Cnt_M_u16

- WhlGrndVlctyRtDrvnHSVldAccum_Cnt_M_u16

- WhlGrndVlctyLftDrvnHSVldAccum_Cnt_M_u16

- WhlGrndVlctyRtNnDrvnHSVldAccum_Cnt_M_u16

- WhlGrndVlctyLftNnDrvnHSVldAccum_Cnt_M_u16

- WhlGrndVlctyRtDrvnCEVldAccum_Cnt_M_u16

- WhlGrndVlctyLftDrvnCEVldAccum_Cnt_M_u16

- WhlGrndVlctyRtNnDrvnCEVldAccum_Cnt_M_u16

- WhlGrndVlctyLftNnDrvnCEVldAccum_Cnt_M_u16

- AntilockTCbrakeVldStartTime_mS_M_u32p0

- RedntVSEActARCVldStartTime_mS_M_u32

- RedntVSEActARCVldAccum_Cnt_M_u16

- RedntVSEActVldStartTime_mS_M_u32

- RedntVSEActVldAccum_Cnt_M_u16

- ABSActvProtPValVldStartTime_mS_M_u32

- ABSActvProtPValVldAccum_Cnt_M_u16

- ABSActvProtARCVldStartTime_mS_M_u32

- ABSActvProtARCVldAccum_Cnt_M_u16

- ABSActvProtVldStartTime_mS_M_u32

- ABSActvProtVldAccum_Cnt_M_u16

- VSEActVldStartTime_mS_M_u32p0

- TCSysEVldStartTime_mS_M_u32p0

- TCSysAVldStartTime_mS_M_u32p0

- ABSFldVldStartTime_mS_M_u32p0

- VhDynCVldStartTime_mS_M_u32p0

- VhDynCVldAccum_Cnt_M_u16

- LKATqOvrDltCmdPrtVlVldStartTime_mS_M_u32

- LKATqOvrDltCmdPrtVlVldAccum_Cnt_M_u16

- LKATqOvrDltCmdRCVldStartTime_mS_M_u32

- LKATqOvrDltCmdRCVldAccum_Cnt_M_u16

- Msg1E9Loss_mS_M_u32

- Msg1E9LossAccum_Cnt_M_u16

- Msg214Loss_mS_M_u32

- Msg214LossAccum_Cnt_M_u16

- Msg232Loss_mS_M_u32

- Msg232LossAccum_Cnt_M_u16

- Msg0C9Loss_mS_M_u32

- Msg0C9LossAccum_Cnt_M_u16

- Msg0C1Loss_mS_M_u32

- Msg0C1LossAccum_Cnt_M_u16

- Msg1F1Loss_mS_M_u32

- Msg1F1LossAccum_Cnt_M_u16

- Msg1F5Loss_mS_M_u32

- Msg1F5LossAccum_Cnt_M_u16

- Msg3E9Loss_mS_M_u32

- Msg3E9LossAccum_Cnt_M_u16

- Msg500Loss_mS_M_u32

- Msg500LossAccum_Cnt_M_u16

- Msg348CELoss_mS_M_u32

- Msg348CELossAccum_Cnt_M_u16

- Msg348HSLoss_mS_M_u32

- Msg348HSLossAccum_Cnt_M_u16

- Msg180HSLoss_mS_M_u32

- Msg180HSLossAccum_Cnt_M_u16

- Msg34ACELoss_mS_M_u32

- Msg34ACELossAccum_Cnt_M_u16

- Msg34AHSLoss_mS_M_u32

- Msg34AHSLossAccum_Cnt_M_u16

- Msg337Loss_mS_M_u32

- Msg337LossAccum_Cnt_M_u16

- Msg17DLoss_mS_M_u32

- Msg17DLossAccum_Cnt_M_u16

- Msg182Loss_mS_M_u32

- Msg182LossAccum_Cnt_M_u16

- Msg3F1Loss_mS_M_u32

- Msg3F1LossAccum_Cnt_M_u16

- Msg4C1Loss_mS_M_u32

- Msg4C1LossAccum_Cnt_M_u16

- Msg180HSLKALoss_mS_M_u32

- Msg17DLKALoss_mS_M_u32

- Msg348HSLKALoss_mS_M_u32

- Msg348CELKALoss_mS_M_u32

- Msg34AHSLKALoss_mS_M_u32

- Msg34ACELKALoss_mS_M_u32

- Msg1E9LKALoss_mS_M_u32

- Msg214LKALoss_mS_M_u32

- WhlGrndVlctyRtDrvnCEStuck_mS_M_u32

- WhlGrndVlctyLftDrvnCEStuck_mS_M_u32

- WhlGrndVlctyRtNnDrvnCEStuck_mS_M_u32

- WhlGrndVlctyLftNnDrvnCEStuck_mS_M_u32

- WhlGrndVlctyRtDrvnHSStuck_mS_M_u32

- WhlGrndVlctyLftDrvnHSStuck_mS_M_u32

- WhlGrndVlctyRtNnDrvnHSStuck_mS_M_u32

- WhlGrndVlctyLftNnDrvnHSStuck_mS_M_u32

- WhlGrndVlctyRtDrvnCEVldStartTime_mS_M_u32

- WhlGrndVlctyLftDrvnCEVldStartTime_mS_M_u32

- WhlGrndVlctyRtNnDrvnCEVldStartTime_mS_M_u32

- WhlGrndVlctyLftNnDrvnCEVldStartTime_mS_M_u32

- WhlGrndVlctyRtDrvnHSVldStartTime_mS_M_u32

- WhlGrndVlctyLftDrvnHSVldStartTime_mS_M_u32

- WhlGrndVlctyRtNnDrvnHSVldStartTime_mS_M_u32

- WhlGrndVlctyLftNnDrvnHSVldStartTime_mS_M_u32

- OldSeqNumR_Cnt_M_u16

- OldWhlDistTstmL_Cnt_M_u16

- OldWhlDistTstmR_Cnt_M_u16

- OldWhlPCntrL_Cnt_M_u16

- OldWhlPCntrR_Cnt_M_u16

- StartStopFault_Cnt_M_b16

- WhlGrndVlctyRtDrvnCE_Cnt_M_u16

- WhlGrndVlctyLftDrvnCE_Cnt_M_u16

- TrnsShftLvrPosVldStartTime_mS_M_u32

- LastPlsChngTimeL_mS_M_u32p0

- WhlGrndVlctyRtNnDrvnCE_Cnt_M_u16

- LastPlsChngTimeR_mS_M_u32p0

- WhlGrndVlctyRtDrvnHS_Cnt_M_u16

- WhlGrndVlctyLftDrvnHS_Cnt_M_u16

- WhlGrndVlctyRtNnDrvnHS_Cnt_M_u16

- WhlGrndVlctyLftNnDrvnHS_Cnt_M_u16

- PrevLKARollingCounter_Cnt_M_u16

- LKAInhibit_Cnt_M_b16

- LKAFault_Cnt_M_b16

- ABSActvProtARC_Cnt_M_u08

- RedntVSEActARC_Cnt_M_u08

- ManualVehSpdOvrRide_Cnt_M_lgc

- VehSpdAvgNDrvnInValid_Cnt_M_lgc

- RedntVSEAct_Cnt_M_lgc

- VSEAct_Cnt_M_lgc

- WhlGrndVlctyRtDrvnCEValid_Cnt_M_lgc

- WhlGrndVlctyLftDrvnCEValid_Cnt_M_lgc

- WhlGrndVlctyRtNnDrvnCEValid_Cnt_M_lgc

- WhlGrndVlctyLftNnDrvnCEValid_Cnt_M_lgc

- WhlGrndVlctyRtDrvnHSValid_Cnt_M_lgc

- WhlGrndVlctyLftDrvnHSValid_Cnt_M_lgc

- WhlGrndVlctyRtNnDrvnHSValid_Cnt_M_lgc

- WhlGrndVlctyLftNnDrvnHSValid_Cnt_M_lgc

- WhlGrndVlctyDrvnCEMissing_Cnt_M_lgc

- WhlGrndVlctyNnDrvnCEMissing_Cnt_M_lgc

- WhlGrndVlctyDrvnHSMissing_Cnt_M_lgc

- LKAFaultLatch_Cnt_D_b16

- APARecoverableFaults_Cnt_M_b08

- APANonRecoverableFaults_Cnt_M_b08

- PrevStrWhlTctlFdbkReqActRC_Cnt_M_u08

- PrevStrWhlAngReqARC_Cnt_M_u08

- InvStartTimeL_mS_M_u32p0

- InvStartTimeR_mS_M_u32p0

- WhlGrndVlctyNnDrvnHSMissing_Cnt_M_lgc

- WIRFltStatusAcc_Cnt_M_u16

- User defined typedef definition/declaration

- This section documents any user types uniquely used for the module.

- Typedef Name

- Element Name

- User Defined Type

- RT_Chassis_General_Status_1

- VehDynYawRate

- VehDynYawRateV

- RT_PPEI_Vehicle_Speed_and_Distance

- VehSpdAvgNonDrvnGroup

- RT_VehSpdAvgNonDrvnGroup

- RT_PPEI_Platform_General_Status

- SysBkupPwrMdEn

- SysBkUpPwrMd

- BkupPwrModeMstrVDA

- RT_PPEI_Steering_Wheel_Angle_CE

- StrAngSnsChksm

- StWhlAngAliveRollCnt

- StrWhAngGrdMsk

- StrWhAngGrdV

- StrWhlAngSenCalStat

- StrWhlAngSenTyp

- StrWhlAngMsgUnused1

- StrWhlAngMsgUnused2

- StrWhlAngMsgUnused3

- VehSpdAvgNDrvn

- VehSpdAvgNDrvnV

- RT_Platform_Eng_Cntrl_Requests

- OtsAirTmpCrVal

- OtsAirTmpCrValV

- OtsAirTmpCrValMsk

- RT_Wheel_Pulses_HS

- WhlRotStatTmstmpRes

- WhlPlsPerRevNonDrvn

- RT_Engine_General_Status_4

- WRSWhlDistPCntr

- WRSWhlDisTpRC

- WRSWhlDistTstm

- WRSWhlDistVal

- WRSWhlRotStatRst

- RT_PPEI_NonDrivn_Whl_Rotationl_Stat

- WhlRotStatLft

- WhlRotStatRght

- Constant Data Dictionary

- Calibration Constants

- This section lists the calibrations used by the module. For details on calibration constants, refer to the Data Dictionary for the application.

- Constant Name

- k_WhlPlsPerRev_Cnt_u16p0

- k_WhlTstmpRes_SecpCnt_f32

- k_AmbTempDflt_DegC_f32

- k_EngTempDflt_DegC_f32

- k_Msg1E9TimeOut_mS_u16p0

- k_Msg1E9TimeOutDiag_Cnt_str

- k_LatAccDflt_MpSecSqrd_f32

- k_YawRateDflt_DegpSec_f32

- k_Msg232TimeOut_mS_u16p0

- k_Msg232TimeOutDiag_Cnt_str

- k_Msg0C9TimeOut_mS_u16p0

- k_Msg0C9TimeOutDiag_Cnt_str

- k_Msg0C1TimeOut_mS_u16p0

- k_Msg0C1TimeOutDiag_Cnt_str

- k_Msg500TimeOut_mS_u16p0

- k_Msg500TimeOutDiag_Cnt_str

- k_Msg1F1TimeOut_mS_u16p0

- k_Msg1F1TimeOutDiag_Cnt_str

- k_Msg1F5TimeOut_mS_u16p0

- k_Msg1F5TimeOutDiag_Cnt_str

- k_Msg1E9LKATimeOut_mS_u16p0

- k_Msg214LKATimeOut_mS_u16p0

- k_Msg180HSLKATimeOut_mS_u16p0

- k_Msg348HSLKATimeOut_mS_u16p0

- k_Msg348CELKATimeOut_mS_u16p0

- k_Msg34AHSLKATimeOut_mS_u16p0

- k_Msg34ACELKATimeOut_mS_u16p0

- k_Msg17DTimeOut_mS_u16p0

- k_Msg214TimeOut_mS_u16p0

- k_Msg214TimeOutDiag_Cnt_str

- k_Msg17DLKATimeOut_mS_u16p0

- k_Msg180HSTimeOut_mS_u16p0

- k_Msg180HSTimeOutDiag_Cnt_str

- k_Msg348HSTimeOut_mS_u16p0

- k_Msg348HSTimeOutDiag_Cnt_str

- k_Msg348CETimeOut_mS_u16p0

- k_Msg348CETimeOutDiag_Cnt_str

- k_Msg34AHSTimeOut_mS_u16p0

- k_Msg34AHSTimeOutDiag_Cnt_str

- k_Msg34ACETimeOut_mS_u16p0

- k_Msg34ACETimeOutDiag_Cnt_str

- k_DefaultSecureVehcileSpeed_Kph_f32

- k_Msg3E9TimeOut_mS_u16p0

- k_Msg3E9TimeOutDiag_Cnt_str

- k_Msg337TimeOut_mS_u16

- k_Msg337TimeOutDiag_Cnt_str

- k_Msg182TimeOut_mS_u16

- k_Msg182TimeOutDiag_Cnt_str

- k_Msg4C1TimeOut_mS_u16p0

- k_Msg4C1TimeOutDiag_Cnt_str

- k_Msg3F1TimeOut_mS_u16p0

- k_Msg3F1TimeOutDiag_Cnt_str

- k_DefaultVehSpd_Kph_f32

- k_WhlRotVldTimeOut_mS_u16p0

- k_MaxFreqChg_Hz_f32

- k_LKATqOvrDltCmdPrtVlVldDiag_Cnt_str

- k_LKATqOvrDltCmdPrtVlVldTimeOut_mS_u16p0

- k_SComTrqPosPol_Cnt_s08

- k_LKATqOvrDltCmdRCVldDiag_Cnt_str

- k_LKATqOvrDltCmdRCVldTimeOut_mS_u16p0

- k_LatAccValDiag_Cnt_str

- k_LatAccValTimeOut_mS_u16p0

- k_YawRateValDiag_Cnt_str

- k_YawRateValTimeOut_mS_u16p0

- k_VSEActValTimeOut_mS_u16p0

- k_VSEActValDiag_Cnt_str

- k_TCSysEValTimeOut_mS_u16p0

- k_TCSysEValDiag_Cnt_str

- k_TCSysAValTimeOut_mS_u16p0

- k_TCSysAValDiag_Cnt_str

- k_TrnsShftLvrPosVldDiag_Cnt_str

- k_ABSFldValTimeOut_mS_u16p0

- k_TrnsShftLvrPosVldTimeOut_mS_u16p0

- k_ABSFldValDiag_Cnt_str

- k_Ms17DTimeOutDiag_Cnt_str

- k_VhDynCValTimeOut_mS_u16p0

- k_VhDynCValDiag_Cnt_str

- k_RedntVSEActARCVldTimeOut_mS_u16p0

- k_RedntVSEActARCVldDiag_Cnt_str

- k_RedntVSEActVldTimeOut_mS_u16p0

- k_RedntVSEActVldDiag_Cnt_str

- k_ABSActvProtPValVldTimeOut_mS_u16p0

- k_ABSActvProtPValVldDiag_Cnt_str

- k_ABSActvProtARCVldTimeOut_mS_u16p0

- k_ABSActvProtARCVldDiag_Cnt_str

- k_ABSActvProtVldDiag_Cnt_str

- k_WhlGrndVlctyRtDrvnHSVldTimeOut_mS_u16p0

- k_WhlGrndVlctyRtDrvnHSValDiag_Cnt_str

- k_WhlGrndVlctyStuckTime_mS_u16

- k_WhlGrndVlctyLftDrvnHSVldTimeOut_mS_u16p0

- k_WhlGrndVlctyLftDrvnHSValDiag_Cnt_str

- k_WhlGrndVlctyRtNnDrvnHSVldTimeOut_mS_u16p0

- k_WhlGrndVlctyRtNnDrvnHSValDiag_Cnt_str

- k_WhlGrndVlctyLftNnDrvnHSVldTimeOut_mS_u16p0

- k_WhlGrndVlctyLftNnDrvnHSValDiag_Cnt_str

- k_VehSpdValTimeOut_mS_u16p0

- k_VehSpdValDiag_Cnt_Str

- k_AmbTempValTimeOut_mS_u16p0

- k_AmbTempValDiag_Cnt_str

- k_Msg3F1LossTimeOutDiag_Cnt_str

- k_EngTempVldTimeOutDiag_Cnt_str

- k_EngTempValTimeOut_mS_u16p0

- k_EngTempValDiag_Cnt_str

- k_Msg4C1LossTimeOutDiag_Cnt_str

- k_VehicleDynamicsESCHybCEValTimeOut_mS_u16p0

- k_VehicleDynamicsESCHybCEValDiag_Cnt_str

- k_ParkAssistParallelCEVldTimeOutDiag_Cnt_str

- k_ParkAssistParallelValTimeOut_mS_u16p0

- k_ParkAssistParallelValDiag_Cnt_str

- k_WhlGrndVlctyRtDrvnCEVldTimeOut_mS_u16p0

- k_WhlGrndVlctyRtDrvnCEValDiag_Cnt_str

- k_WhlGrndVlctyLftDrvnCEVldTimeOut_mS_u16p0

- k_WhlGrndVlctyLftDrvnCEValDiag_Cnt_str

- k_WhlGrndVlctyRtNnDrvnCEVldTimeOut_mS_u16p0

- k_WhlGrndVlctyRtNnDrvnCEValDiag_Cnt_str

- k_WhlGrndVlctyLftNnDrvnCEVldTimeOut_mS_u16p0

- k_WhlGrndVlctyLftNnDrvnCEValDiag_Cnt_str

- k_WIRFltStatusDiag_Cnt_str

- Program(fixed) Constants

- Embedded Constants

- All embedded constants whose values are provided in Eng units will be evaluated to the equivalent counts by using the FPM_InitFixedPoint_m() macro within the #define statement.

- D_CONFIRMEDDTCBIT_CNT_B8

- D_DEFAULTPERS_CNT_U16

- D_NORMALPERS_CNT_U16

- D_SPORTPERS_CNT_U16

- D_TOWHAULPERS_CNT_U16

- D_WIRFLTVALBIT_CNT_U16
