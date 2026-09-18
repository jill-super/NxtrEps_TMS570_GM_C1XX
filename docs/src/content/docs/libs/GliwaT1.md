---
title: "GliwaT1"
description: "GliwaT1: purpose, files, API and documents (Libraries & Common)."
---

:::caution[Third-party — Gliwa]
Third-party timing-analysis code from Gliwa GmbH (`know-how in embedded software`). Do not modify.
:::
*Origin: **Gliwa** — Gliwa T1 timing-analysis target code (third-party, Gliwa GmbH).*
## Purpose and responsibility
Software area `GliwaT1` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `T1_AppInterface.c`, `T1_config.c`, `libt1base.a`, `libt1com8.a`, `libt1cont.a`, `libt1delay.a`, `libt1flex.a`, `libt1mod.a`, `libt1scope.a`, `sys_pmu.asm` |
| `include/` | `Metrics.h`, `T1_AppInterface.h`, `T1_MemMap.h`, `T1_baseConfig.h`, `T1_baseInterface.h`, `T1_bid.h`, `T1_config.h`, `T1_contConfig.h`, `T1_contInterface.h`, `T1_delayConfig.h`, `T1_delayInterface.h`, `T1_flexConfig.h` |
## Public API
| File | Function |
| --- | --- |
| T1_AppInterface.c | `T1_AppInit()` |
| T1_AppInterface.c | `T1_AppHandler()` |
| T1_AppInterface.c | `T1_AppBgHandler()` |
| T1_config.c | `osPrefetchAbort()` |
| T1_config.c | `osDataAbort()` |
## Usage and dependencies
Selected project headers included by this module:
`Std_Types.h` `T1_AppInterface.h` `T1_AppInterface_Cfg.h` `T1_MemMap.h` `T1_baseConfig.h` `T1_baseInterface.h` `T1_bid.h` `T1_contConfig.h` `T1_delayConfig.h` `T1_flexConfig.h` `T1_scopeConfig.h` `T1_scopeInterface.h` `T1_targetSpecifics.h` `osek.h` `sys_common.h` `sys_pmu.h`
## Documents
No `doc/` documents for this module.

*Repository path: `GliwaT1/`* 
