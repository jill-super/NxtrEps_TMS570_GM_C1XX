---
title: "Vector vs. custom code"
description: "How to tell Vector-provided code from in-house code."
sidebar:
  order: 1
---

## How origin was determined

A file is treated as **Vector-provided** when its header states
`This software is copyright protected and proprietary to Vector Informatik GmbH`
(659 occurrences in this snapshot), or when it lives under the Vector-owned
`GM_C1XX_EPS_TMS570/SwProject/Source/{BSW,GenData,GenDataRte,GenDataOS}` trees.
RTE contract stubs (`utp/contract/`, `tools/contract/`) and DaVinci artefacts
(`.arxml`, `.dcf`, `.dcb`, `generate/*.tt`) are **Vector-generated** scaffolding
around **Custom** Nexteer application code.

Third-party origins: **TI** (`Fee`, `Fls` — Flash/EEPROM drivers for TMS570),
**Gliwa** (`GliwaT1` — timing analysis), **PRQA** (`QAC` configuration).

## Module origin matrix

| Module | Layer | Origin |
| --- | --- | --- |
| [AbsHwPos_TcI2cVd](../asw/AbsHwPos_TcI2cVd/) | asw | Custom |
| [ActivePull](../asw/ActivePull/) | asw | Custom |
| [Adc](../mcal/Adc/) | mcal | Custom |
| [Assist](../asw/Assist/) | asw | Custom |
| [AssistFirewall](../asw/AssistFirewall/) | asw | Custom |
| [AstLmt_CM](../asw/AstLmt_CM/) | asw | Custom |
| [AvgFricLrn](../asw/AvgFricLrn/) | asw | Custom |
| [BVDiag](../asw/BVDiag/) | asw | Custom |
| [BatteryVoltage](../asw/BatteryVoltage/) | asw | Custom |
| [BkCpPc](../sa/BkCpPc/) | sa | Custom |
| [CMS_Common](../libs/CMS_Common/) | libs | Custom |
| [CmMtrCurr](../sa/CmMtrCurr/) | sa | Custom |
| [ComplErr](../asw/ComplErr/) | asw | Custom |
| [CtrlTemp](../sa/CtrlTemp/) | sa | Custom |
| [CtrldDisShtdn](../asw/CtrldDisShtdn/) | asw | Custom |
| [Damping](../asw/Damping/) | asw | Custom |
| [DampingFirewall](../asw/DampingFirewall/) | asw | Custom |
| [DiagMgr](../asw/DiagMgr/) | asw | Custom |
| [DigColPs](../sa/DigColPs/) | sa | Custom |
| [DigHwTrqSENT](../sa/DigHwTrqSENT/) | sa | Custom |
| [DigMSB](../sa/DigMSB/) | sa | Custom |
| [Dma](../mcal/Dma/) | mcal | Custom |
| [EOTActuatorMng](../asw/EOTActuatorMng/) | asw | Custom |
| [EtDmpFw](../asw/EtDmpFw/) | asw | Custom |
| [Fee](../bsw/Fee/) | bsw | TI |
| [Fls](../mcal/Fls/) | mcal | TI |
| [FltInjection](../asw/FltInjection/) | asw | Custom |
| [FrqDepDmpnInrtCmp](../asw/FrqDepDmpnInrtCmp/) | asw | Custom |
| [GMSrlComOutput](../asw/GMSrlComOutput/) | asw | Custom |
| [GMStrtStop](../asw/GMStrtStop/) | asw | Custom |
| [GenPosTraj](../asw/GenPosTraj/) | asw | Custom |
| [GliwaT1](../libs/GliwaT1/) | libs | Gliwa |
| [HOWDetect](../asw/HOWDetect/) | asw | Custom |
| [HiLoadStall](../asw/HiLoadStall/) | asw | Custom |
| [HighFreqAssist](../asw/HighFreqAssist/) | asw | Custom |
| [HwPwUp](../asw/HwPwUp/) | asw | Custom |
| [HystComp](../asw/HystComp/) | asw | Custom |
| [I2cNxtr](../mcal/I2cNxtr/) | mcal | Custom |
| [LmtCod](../asw/LmtCod/) | asw | Custom |
| [LrnEOT](../asw/LrnEOT/) | asw | Custom |
| [Metrics](../libs/Metrics/) | libs | Custom |
| [MtrCtrl_CM](../cdd/MtrCtrl_CM/) | cdd | Custom |
| [MtrTempEst](../asw/MtrTempEst/) | asw | Custom |
| [MtrVel_Digi](../sa/MtrVel_Digi/) | sa | Custom |
| [NvMMgr](../bsw/NvMMgr/) | bsw | Custom |
| [NvMProxy](../cdd/NvMProxy/) | cdd | Custom |
| [NxtrLib](../libs/NxtrLib/) | libs | Custom |
| [OvrVoltMon](../sa/OvrVoltMon/) | sa | Custom |
| [Polarity](../asw/Polarity/) | asw | Custom |
| [PosServo](../asw/PosServo/) | asw | Custom |
| [PwrLmtFuncCr](../asw/PwrLmtFuncCr/) | asw | Custom |
| [QAC](../libs/QAC/) | libs | Third-party |
| [Return](../asw/Return/) | asw | Custom |
| [ReturnFirewall](../asw/ReturnFirewall/) | asw | Custom |
| [SF46_GCCDiag_Implementation](../asw/SF46_GCCDiag_Implementation/) | asw | Custom |
| [SF47_TSMit_Implementation](../asw/SF47_TSMit_Implementation/) | asw | Custom |
| [SVDiag](../sa/SVDiag/) | sa | Custom |
| [SVDrvr_CM](../cdd/SVDrvr_CM/) | cdd | Custom |
| [SgnlCond](../asw/SgnlCond/) | asw | Custom |
| [ShtdnMech](../sa/ShtdnMech/) | sa | Custom |
| [SpiNxt](../mcal/SpiNxt/) | mcal | Custom |
| [StOpCtrl](../asw/StOpCtrl/) | asw | Custom |
| [StaMd](../asw/StaMd/) | asw | Custom |
| [StabilityComp](../asw/StabilityComp/) | asw | Custom |
| [StdDef](../mcal/StdDef/) | mcal | Custom |
| [Sweep](../asw/Sweep/) | asw | Custom |
| [TMS570_Startup](../mcal/TMS570_Startup/) | mcal | Custom |
| [TMS570_uDiag](../cdd/TMS570_uDiag/) | cdd | Custom |
| [ThrmDutyCycle](../asw/ThrmDutyCycle/) | asw | Custom |
| [TmprlMon](../sa/TmprlMon/) | sa | Custom |
| [TqRsDg](../asw/TqRsDg/) | asw | Custom |
| [TrqArblim](../asw/TrqArblim/) | asw | Custom |
| [TrqOsc](../asw/TrqOsc/) | asw | Custom |
| [TrqOvlSta](../asw/TrqOvlSta/) | asw | Custom |
| [TuningSelAuth](../asw/TuningSelAuth/) | asw | Custom |
| [VehDyn](../asw/VehDyn/) | asw | Custom |
| [VehSpdLmt](../asw/VehSpdLmt/) | asw | Custom |
| [WhlImbRej](../asw/WhlImbRej/) | asw | Custom |
| [Xcp](../bsw/Xcp/) | bsw | Custom |
| [ePWM](../mcal/ePWM/) | mcal | Custom |
