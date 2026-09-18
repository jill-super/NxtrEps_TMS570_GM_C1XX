---
title: "MtrCtrl_CM"
description: "MtrCtrl_CM: purpose, files, API and documents (Complex Device Drivers (CDD))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house motor-control CDD cluster (Ap_CurrCmd, Ap_PICurrCntrl, ...).*
## Purpose and responsibility
Software area `MtrCtrl_CM` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_CurrCmd.c`, `Ap_CurrParamComp.c`, `Ap_PICurrCntrl.c`, `Ap_PeakCurrEst.c`, `Ap_QuadDet.c`, `Ap_TrqCanc.c`, `Ap_TrqCmdScl.c` |
| `include/` | `Ap_MtrCtrl.h` |
| AUTOSAR model | 10 `.arxml` file(s), e.g. `Ap_CurrCmd.arxml` |
| Generation templates | `Ap_CurrCmd_Cfg.arxml.tt`, `Ap_CurrCmd_Cfg.h.tt`, `Ap_CurrCmd_Generate.bat`, `Ap_CurrCmd_bswmd.arxml`, `Ap_CurrParamComp_Cfg.arxml.tt`, `Ap_CurrParamComp_Cfg.h.tt` |
## Public API
Top RTE/component symbols referenced in the sources (102 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_CurrCmd_Per1_CurrentGainSvc_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_CurrCmd_Per1_EstKe_VpRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_CurrCmd_Per1_EstLd_Henry_f32` | RTE-generated symbol |
| `Rte_IRead_CurrCmd_Per1_EstLq_Henry_f32` | RTE-generated symbol |
| `Rte_IRead_CurrCmd_Per1_EstR_Ohm_f32` | RTE-generated symbol |
| `Rte_IRead_CurrCmd_Per1_IvtrLoaMtgtnEn_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_CurrCmd_Per1_MRFMtrVel_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_CurrCmd_Per1_MRFTrqCmdScl_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_CurrCmd_Per1_MotCurrLoaMtgtnEn_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_CurrCmd_Per1_MtrQuad_Cnt_u08` | RTE-generated symbol |
| `Rte_IRead_CurrCmd_Per1_Vecu_Volt_f32` | RTE-generated symbol |
| `Rte_IRead_CurrCmd_Per1_VehSpd_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_CurrCmd_Per1_MtrCurrAngle_Rev_f32` | RTE-generated symbol |
| `Rte_IWriteRef_CurrCmd_Per1_MtrCurrAngle_Rev_f32` | RTE-generated symbol |
| `Rte_IWrite_CurrCmd_Per1_MtrCurrDaxRef_Amp_f32` | RTE-generated symbol |
| `Rte_IWriteRef_CurrCmd_Per1_MtrCurrDaxRef_Amp_f32` | RTE-generated symbol |
| `Rte_IWrite_CurrCmd_Per1_MtrCurrQaxRef_Amp_f32` | RTE-generated symbol |
| `Rte_IWriteRef_CurrCmd_Per1_MtrCurrQaxRef_Amp_f32` | RTE-generated symbol |
| `Rte_Call_CurrCmd_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_CurrCmd_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_Pim_EOLNomMtrParam` | RTE-generated symbol |
| `Rte_IWrite_CurrParamComp_Init_EstKe_VpRadpS_f32` | RTE-generated symbol |
| `Rte_IWriteRef_CurrParamComp_Init_EstKe_VpRadpS_f32` | RTE-generated symbol |
| `Rte_IWrite_CurrParamComp_Init_EstLd_Henry_f32` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_CurrCmd_Cfg.h` `Ap_CurrParamComp_Cfg.h` `Ap_MtrCtrl.h` `Ap_PICurrCntrl_Cfg.h` `Ap_PeakCurrEst_Cfg.h` `Ap_QuadDet_Cfg.h` `Ap_TrqCanc_Cfg.h` `Ap_TrqCmdScl_Cfg.h` `CalConstants.h` `GlobalMacro.h` `Interpolation.h` `MemMap.h` `MtrCtrl_Cfg.h` `Rte_Ap_CurrCmd.h` `Rte_Ap_CurrParamComp.h` `Rte_Ap_PICurrCntrl.h` `Rte_Ap_PeakCurrEst.h` `Rte_Ap_QuadDet.h` `Rte_Ap_TrqCanc.h` `Rte_Ap_TrqCmdScl.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_CurrCmd` `Ap_CurrCmd_Cfg.h` `Rte.h` `Rte_Ap_CurrCmd.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `Ap_CurrParamComp` `Ap_CurrParamComp_Cfg.h` `Rte.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [MtrCtrl_CM — CurrCmd_MDD](./MtrCtrl_CM-CurrCmd_MDD/) | `MtrCtrl_CM/doc/CurrCmd_MDD.doc` |
| [MtrCtrl_CM — CurrParamComp_MDD](./MtrCtrl_CM-CurrParamComp_MDD/) | `MtrCtrl_CM/doc/CurrParamComp_MDD.docx` |
| [MtrCtrl_CM — MtrCntrl_Integration_Manual](./MtrCtrl_CM-MtrCntrl_Integration_Manual/) | `MtrCtrl_CM/doc/MtrCntrl_Integration_Manual.docx` |
| [MtrCtrl_CM — PICurrentContrl](./MtrCtrl_CM-PICurrentContrl/) | `MtrCtrl_CM/doc/PICurrentContrl.doc` |
| [MtrCtrl_CM — PeakCurrEst_MDD](./MtrCtrl_CM-PeakCurrEst_MDD/) | `MtrCtrl_CM/doc/PeakCurrEst_MDD.docx` |
| [MtrCtrl_CM — Quadrant_Detection_MDD](./MtrCtrl_CM-Quadrant_Detection_MDD/) | `MtrCtrl_CM/doc/Quadrant_Detection_MDD.docx` |
| [MtrCtrl_CM — TorqueCmdScaling_MDD](./MtrCtrl_CM-TorqueCmdScaling_MDD/) | `MtrCtrl_CM/doc/TorqueCmdScaling_MDD.doc` |
| [MtrCtrl_CM — TrqCanc_MDD](./MtrCtrl_CM-TrqCanc_MDD/) | `MtrCtrl_CM/doc/TrqCanc_MDD.docx` |

*Repository path: `MtrCtrl_CM/`* 
