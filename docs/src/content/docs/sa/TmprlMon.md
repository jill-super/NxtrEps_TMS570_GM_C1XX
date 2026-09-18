---
title: "TmprlMon"
description: "TmprlMon: purpose, files, API and documents (Sensor / Actuator Abstraction)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-Cs (Sa_TmprlMon/2).*
## Purpose and responsibility
Software area `TmprlMon` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Sa_TmprlMon.c`, `Sa_TmprlMon2.c` |
| AUTOSAR model | 5 `.arxml` file(s), e.g. `Sa_TmprlMon.arxml` |
| Generation templates | `Sa_TmprlMon2_Cfg.arxml.tt`, `Sa_TmprlMon2_Cfg.h.tt`, `Sa_TmprlMon2_Generate.bat`, `Sa_TmprlMon2_bswmd.arxml`, `Sa_TmprlMon_Cfg.arxml.tt`, `Sa_TmprlMon_Cfg.h.tt` |
## Public API
Top RTE/component symbols referenced in the sources (25 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_Call_WdMonitor_OP_SET` | RTE-generated symbol |
| `Rte_Call_TmprlMon_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_TmprlMon_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IRead_TmprlMon_Per2_TMFTestStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_TmprlMon_Per2_TMFTestComplete_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_TmprlMon_Per2_TMFTestComplete_Cnt_lgc` | RTE-generated symbol |
| `Rte_Call_FetDrvCntl_OP_GET` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_PwrSwitchEn_OP_GET` | RTE-generated symbol |
| `Rte_Call_SysFault2_OP_SET` | RTE-generated symbol |
| `Rte_Call_SysFault3_OP_SET` | RTE-generated symbol |
| `Rte_Call_WdReset_OP_SET` | RTE-generated symbol |
| `Rte_Call_SystemTime_DtrmnElapsedTime_mS_u16` | RTE-generated symbol |
| `Rte_Call_SystemTime_GetSystemTime_mS_u32` | RTE-generated symbol |
| `Rte_Call_TmprlMon_Per2_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_SysFault3_OP_GET` | RTE-generated symbol |
| `Rte_Call_TmprlMon_Per2_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_SysFault2_OP_GET` | RTE-generated symbol |
| `Rte_Call_TmprlMon_Per3_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_TmprlMon_Per3_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IWrite_TmprlMon_Trns1_TMFTestComplete_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_TmprlMon_Trns1_TMFTestComplete_Cnt_lgc` | RTE-generated symbol |
| `Rte_Call_TmprlMon2_Per1_CP0_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Sa_TmprlMon.h` `Rte_Sa_TmprlMon2.h` `Sa_TmprlMon2_Cfg.h` `Sa_TmprlMon_Cfg.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`CalConstants.h` `Compiler_Cfg.h` `MemMap.h` `Sa_TmprlMon` `Rte.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Sa_TmprlMon.h` `Rte_Type.h` `Sa_TmprlMon_Cfg.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [TmprlMon — Temporal_Monitor_2_MDD](./TmprlMon-Temporal_Monitor_2_MDD/) | `TmprlMon/doc/Temporal_Monitor_2_MDD.docx` |
| [TmprlMon — Temporal_Monitor_MDD](./TmprlMon-Temporal_Monitor_MDD/) | `TmprlMon/doc/Temporal_Monitor_MDD.docx` |

*Repository path: `TmprlMon/`* 
