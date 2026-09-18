---
title: "Xcp"
description: "Xcp: purpose, files, API and documents (Basic Software (BSW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house XCP handler SW-C (Ap_ApXcp) on top of the Vector XCP stack.*
## Purpose and responsibility
Software area `Xcp` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_ApXcp.c` |
| `include/` | `Ap_ApXcp.h` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_ApXcp.arxml` |
| Generation templates | `Ap_ApXcp_Cfg.c.tt`, `Ap_ApXcp_Cfg.h.tt`, `Ap_ApXcp_Generate.bat`, `Ap_ApXcp_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (8 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_ApXcp_Per1_ActiveTunPers_Cnt_u16` | RTE-generated symbol |
| `Rte_IRead_ApXcp_Per1_ActiveTunSet_Cnt_u16` | RTE-generated symbol |
| `Rte_IRead_ApXcp_Per1_DesiredTunPers_Cnt_u16` | RTE-generated symbol |
| `Rte_IRead_ApXcp_Per1_DesiredTunSet_Cnt_u16` | RTE-generated symbol |
| `Rte_IWrite_ApXcp_Per1_ActiveTunOvrPtrAddr_Cnt_u32` | RTE-generated symbol |
| `Rte_IWriteRef_ApXcp_Per1_ActiveTunOvrPtrAddr_Cnt_u32` | RTE-generated symbol |
| `Rte_IWrite_ApXcp_Per1_TuningSessionActPtr_Cnt_u8` | RTE-generated symbol |
| `Rte_IWriteRef_ApXcp_Per1_TuningSessionActPtr_Cnt_u8` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_ApXcp.h` `Ap_ApXcp_Cfg.h` `EPS_DiagSrvcs_SrvcLUTbl.h` `EPS_DiagSrvcs_XCP.Interface.h` `EPS_DiagSrvcs_XCP.h` `Eep_30_At25128.h` `Mcu.h` `MemMap.h` `Rte_Ap_ApXcp.h` `Std_Types.h` `SystemTime.h` `XcpProf.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Rte.h` `Rte_Ap_ApXcp.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [Xcp — ApXcp_Integration_Manual](./Xcp-ApXcp_Integration_Manual/) | `Xcp/doc/ApXcp_Integration_Manual.docx` |

*Repository path: `Xcp/`* 
