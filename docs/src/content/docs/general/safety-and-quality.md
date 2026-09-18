---
title: "Safety and quality"
description: "ASIL D, MISRA/QAC and unit-test strategy evidence in the repo."
sidebar:
  order: 5
---

## Functional safety (ISO 26262 ASIL D)

The EPS is developed to ASIL D. In-repo evidence:

- `TmprlMon` (temporal monitor) and `TqRsDg` (torque reasonableness diagnostics) plus
  firewall SW-Cs (`AssistFirewall`, `DampingFirewall`, `ReturnFirewall`, `EtDmpFw`).
- `TMS570_uDiag` micro-diagnostics (ESM, FPU, static registers, peripheral MPU) and `FlsTst`.
- `FltInjection` SW-C for fault-injection testing; `ShtdnMech` shutdown mechanisms.
- Redundant/ plausibility paths: `DigColPs` + `DigColPsInt`, `MtrVel` triple sources, `SVDiag`.

## MISRA / QAC

- Project-wide QAC configuration in `QAC/` (see [QAC](../libs/QAC/)) and the
  [MISRA Compliance Guidelines](../libs/QAC-MISRA-Compliance-Guidelines/) conversion.
- Per-module `doc/QAC_Results/` (`.err`/`.met`) record static-analysis findings.

## Unit testing

Tessy artefacts in every module's `utp/` folder — see [Unit-test reports](./unit-test-reports/).
