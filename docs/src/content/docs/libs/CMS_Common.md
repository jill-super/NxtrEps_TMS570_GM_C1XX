---
title: "CMS_Common"
description: "CMS_Common: purpose, files, API and documents (Libraries & Common)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer common manufacturing/diagnostic services (EPS_DiagSrvcs). One file (EPS_DiagSrvcs_XCP.Vector.c) carries a Vector header.*
## Purpose and responsibility
Software area `CMS_Common` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `EPS_DiagSrvcs_ISO.c`, `EPS_DiagSrvcs_XCP.Vector.c`, `EPS_DiagSrvcs_XCP.c` |
| `include/` | `EPS_DiagSrvcs_CommonData.h`, `EPS_DiagSrvcs_ISO.h`, `EPS_DiagSrvcs_SrvcLUTbl.h`, `EPS_DiagSrvcs_XCP.h` |
## Public API
Top RTE/component symbols referenced in the sources (1 unique in total):
| Symbol | Kind |
| --- | --- |
| `EPS_DiagSrvcs_Init` | component symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_DfltConfigData.h` `CDD_Data.h` `CalConstants.h` `Compiler.h` `DataLogistic.h` `EPS_DiagSrvcs_CommonData.h` `EPS_DiagSrvcs_ISO.Customer.h` `EPS_DiagSrvcs_ISO.Interface.h` `EPS_DiagSrvcs_ISO.h` `EPS_DiagSrvcs_SrvcLUTbl.h` `EPS_DiagSrvcs_XCP.Interface.h` `EPS_DiagSrvcs_XCP.h` `GlobalMacro.h` `MemMap.h` `NvM.h` `Rte_type.h` `Std_Types.h` `SystemTime.h` `fixmath.h` `fpmtype.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_DfltConfigData.h` `Ap_DiagMgr.h` `CDD_Const.h` `CDD_Data.h` `CalConstants.h` `Cd_TcFlshPrg.h` `Compiler_Cfg.h` `DataLogistic.h` `Dem_Cfg.h` `Dem_Types.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
No `doc/` documents for this module.

*Repository path: `CMS_Common/`* 
