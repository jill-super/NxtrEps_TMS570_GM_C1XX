---
title: "Build system"
description: "How the EPS firmware is built: RTE rules, linker script and host tools."
sidebar:
  order: 0
---

## Overview

The firmware targets the TI TMS570 (ARM Cortex-R4, `TMS570LS202x`) and is built from the
`GM_C1XX_EPS_TMS570/SwProject` tree. There is no top-level Makefile/CMake in this snapshot:
the build is driven by the RTE build rules, the linker command file and the host-side tool chain below.

## RTE build rules

`SwProject/Source/GenDataRte/mak/` contains the Vector-generated RTE build fragments:

`Rte_cfg.mak`, `Rte_check.mak`, `Rte_defs.mak`, `Rte_rules.mak`

plus the integration entry points `SwProject/Source/` (`AppStartupCallout.c`, `ApplCallbacks.c`,
`IoHwAb.c`, `NtWrap.c`, `SchM.c`, `RteErrata*.c`).

## Linker and memory layout

Linker command file: `SwProject/TMS570LS202x6SFlashLnk.cmd`. Post-build steps live in
`SwProject/postbuild.bat` and `archive.bat` (repo root of the integration project).

## Host-side tools

`GM_C1XX_EPS_TMS570/Tools/` contains: `AsrProject`, `CCT`, `DataDictTool`, `GliwaT1`, `GnuWin32`, `HexView`, `Metrics`, `NexteerArtt`, `OilTool`, `Patch`, `Postbuild`, `QAC`, `Trimmer`, `hex470`.

Notable tools: `HexView` (checksum/vector-table post-processing), `AsrProject` (AUTOSAR
generators incl. `MicrosarGen` and `Artt`), `NexteerArtt`, `Metrics`, `QAC`, `DataDictTool`,
`Trimmer`, `GliwaT1` config and the `hex470`/`GnuWin32` utilities.

## Typical build flow

1. Generate RTE/BSW configuration with DaVinci Configurator (Vector) into `SwProject/Source/GenData*`.
2. Generate each SW-C configuration via its `generate/*_Generate.bat` / `.tt` templates.
3. Compile the TMS570 sources with the TI ARM compiler (`hex470`).
4. Link with `TMS570LS202x6SFlashLnk.cmd`, run `postbuild.bat` and `HexView`.
