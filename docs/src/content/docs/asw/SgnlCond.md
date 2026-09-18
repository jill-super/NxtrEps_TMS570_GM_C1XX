---
title: "SgnlCond"
description: "SgnlCond: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_SignlCondn).*
## Purpose and responsibility
Software area `SgnlCond` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_SignlCondn.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_SignlCondn.arxml` |
| Generation templates | `Ap_SignlCondn_Cfg.arxml.tt`, `Ap_SignlCondn_Cfg.h.tt`, `Ap_SignlCondn_Generate.bat`, `Ap_SignlCondn_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (9 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_SignlCondn_Per1_SrlComVehSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IRead_SignlCondn_Per1_SrlCom_VehicleLonAccel_KphpS_f32` | RTE-generated symbol |
| `Rte_IWrite_SignlCondn_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IWriteRef_SignlCondn_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_SignlCondn_Per1_Vehicle_LonAccel_KphpS_f32` | RTE-generated symbol |
| `Rte_IWriteRef_SignlCondn_Per1_Vehicle_LonAccel_KphpS_f32` | RTE-generated symbol |
| `Rte_Call_FaultInjection_SCom_FltInjection` | RTE-generated symbol |
| `Rte_Call_SignlCondn_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_SignlCondn_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_SignlCondn_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_SignlCondn.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_SignlCondn` `Ap_SignlCondn_Cfg.h` `Rte.h` `Rte_Ap_SignlCondn.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `Ap_SignlCondn_Cfg.h` `CalConstants.h` `Compiler_Cfg.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [SgnlCond — SignalConditioning_MDD](./SgnlCond-SignalConditioning_MDD/) | `SgnlCond/doc/SignalConditioning_MDD.docx` |

*Repository path: `SgnlCond/`* 
