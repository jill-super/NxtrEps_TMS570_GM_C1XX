---
title: "NxtrLib"
description: "NxtrLib: purpose, files, API and documents (Libraries & Common)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house math/filter/interpolation library.*
## Purpose and responsibility
Software area `NxtrLib` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `CheckSums.c`, `SystemTime.c`, `atan2.asm`, `atan2_octants.c`, `filters.c`, `interpolation.c` |
| `include/` | `CheckSums.h`, `Filter_Types.h`, `GlobalMacro.h`, `SinCos.h`, `SystemTime.h`, `atan2.h`, `filters.h`, `fixmath.h`, `fpmtype.h`, `interpolation.h` |
| Generation templates | `SystemTime_Cfg.h.tt` |
## Public API
Top RTE/component symbols referenced in the sources (4 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IrvRead_DtrmnElapsedTime_mS_u16_Time_mS_u32` | RTE-generated symbol |
| `Rte_IrvRead_GetSystemTime_mS_u32_Time_mS_u32` | RTE-generated symbol |
| `Rte_IrvWrite_SystemTime_Per1_Time_mS_u32` | RTE-generated symbol |
| `Rte_IrvRead_SystemTime_Per1_Time_mS_u32` | RTE-generated symbol |
<details><summary>Top-level function definitions</summary>
| File | Function |
| --- | --- |
| interpolation.c | `BilinearXYM_s16_u16Xs16YM_Cnt()` |
| interpolation.c | `BilinearXYM_u16_u16Xu16YM_Cnt()` |
| interpolation.c | `BilinearXYM_s16_s16Xs16YM_Cnt()` |
| interpolation.c | `BilinearXYM_u16_s16Xu16YM_Cnt()` |
| interpolation.c | `BilinearXMYM_u16_u16XMu16YM_Cnt()` |
| interpolation.c | `BilinearXMYM_s16_u16XMs16YM_Cnt()` |
| interpolation.c | `BilinearXMYM_s16_s16XMs16YM_Cnt()` |
| interpolation.c | `BilinearXMYM_u16_s16XMu16YM_Cnt()` |
| interpolation.c | `IntplVarXY_u16_u16Xu16Y_Cnt()` |
| interpolation.c | `IntplVarXY_u16_s16Xu16Y_Cnt()` |
| interpolation.c | `IntplVarXY_s16_s16Xs16Y_Cnt()` |
| interpolation.c | `IntplVarXY_s16_u16Xs16Y_Cnt()` |
| interpolation.c | `IntplFxdX_u16_u16Xu16Y_Cnt()` |
| interpolation.c | `IntplFxdX_u16_s16Xu16Y_Cnt()` |
| interpolation.c | `IntplFxdX_s16_s16Xs16Y_Cnt()` |
| interpolation.c | `IntplFxdX_s16_u16Xs16Y_Cnt()` |
</details>
## Usage and dependencies
Selected project headers included by this module:
`CheckSums.h` `Filter_Types.h` `GlobalMacro.h` `Gpt.h` `Gpt_Cfg.h` `MemMap.h` `Platform_Types.h` `Rte_NexteerLibs.h` `Rte_Type.h` `Std_Types.h` `SystemTime.h` `SystemTime_Cfg.h` `filters.h` `fixmath.h` `fpmtype.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Compiler_Cfg.h` `Platform_Types.h` `Test_SinCos.c` `Test_SinCos.h` `float.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [NxtrLib — Filter_Library_Design_Document](./NxtrLib-Filter_Library_Design_Document/) | `NxtrLib/doc/Filter_Library_Design_Document.doc` |
| [NxtrLib — Interpolation_Design_MDD](./NxtrLib-Interpolation_Design_MDD/) | `NxtrLib/doc/Interpolation_Design_MDD.doc` |
| [NxtrLib — NxtrLib_Systemtime Integration_Manual](./NxtrLib-NxtrLib_Systemtime-Integration_Manual/) | `NxtrLib/doc/NxtrLib_Systemtime Integration_Manual.docx` |
| [NxtrLib — Optimized SinCos Algorithm](./NxtrLib-Optimized-SinCos-Algorithm/) | `NxtrLib/doc/Optimized SinCos Algorithm.docx` |

*Repository path: `NxtrLib/`* 
