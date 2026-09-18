---
title: "Metrics"
description: "Metrics: purpose, files, API and documents (Libraries & Common)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house CPU-load metrics module using the PMU.*
## Purpose and responsibility
Software area `Metrics` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Metrics.c`, `sys_pmu.asm` |
| `include/` | `Metrics.h`, `Metrics_Enable.h`, `sys_pmu.h` |
| Generation templates | `Metrics_Cfg.c.tt`, `Metrics_Cfg.h.tt`, `Metrics_Generate.bat`, `Metrics_RteHookImport.txt.tt`, `Metrics_bswmd.arxml` |
## Public API
| File | Function |
| --- | --- |
| Metrics.c | `Metrics_RunnableStart()` |
## Usage and dependencies
Selected project headers included by this module:
`Det.h` `GlobalMacro.h` `MemMap.h` `Metrics.h` `Metrics_Cfg.h` `Metrics_Enable.h` `Rte_Type.h` `Std_Types.h` `SystemTime.h` `filters.h` `oseksctx.h` `string.h` `sys_common.h` `sys_pmu.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Metrics_Cfg.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [Metrics — Metrics_Integration_Manual](./Metrics-Metrics_Integration_Manual/) | `Metrics/doc/Metrics_Integration_Manual.docx` |
| [Metrics — Metrics_MDD](./Metrics-Metrics_MDD/) | `Metrics/doc/Metrics_MDD.docx` |

*Repository path: `Metrics/`* 
