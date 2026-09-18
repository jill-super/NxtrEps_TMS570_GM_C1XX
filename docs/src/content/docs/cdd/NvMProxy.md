---
title: "NvMProxy"
description: "NvMProxy: purpose, files, API and documents (Complex Device Drivers (CDD))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house CDD (Cd_NvMProxy) bridging SW-Cs to the NvM stack.*
## Purpose and responsibility
Software area `NvMProxy` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Cd_NvMProxy.c` |
| `include/` | `Cd_NvMProxy.h` |
| AUTOSAR model | 3 `.arxml` file(s), e.g. `NvMProxy.arxml` |
| Generation templates | `Cd_NvMProxy_Cfg.h.tt`, `Cd_NvMProxy_Generate.bat`, `Cd_NvMProxy_PBcfg.c.tt`, `Cd_NvMProxy_bswmd.arxml`, `Cd_NvMProxy_swc.arxml.tt` |
## Public API
Top RTE/component symbols referenced in the sources (2 unique in total):
| Symbol | Kind |
| --- | --- |
| `SchM_Enter_NvMProxy` | component symbol |
| `SchM_Exit_NvMProxy` | component symbol |
## Usage and dependencies
Selected project headers included by this module:
`Cd_NvMProxy.h` `Cd_NvMProxy_Cfg.h` `Crc.h` `MemMap.h` `NvM.h` `SchM_NvMProxy.h` `Std_Types.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_DiagMgr.h` `Cd_NvMProxy_Cfg.h` `Compiler_Cfg.h` `Crc.h` `MemMap.h` `NvM.h` `NvM_Types.h` `Rte_Type.h` `SchM_NvMProxy.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [NvMProxy — NvMProxy_Integration_Manual](./NvMProxy-NvMProxy_Integration_Manual/) | `NvMProxy/doc/NvMProxy_Integration_Manual.docx` |
| [NvMProxy — NvMProxy_MDD](./NvMProxy-NvMProxy_MDD/) | `NvMProxy/doc/NvMProxy_MDD.docx` |

*Repository path: `NvMProxy/`* 
