---
title: "SF47_TSMit_Implementation — TSMit_Integration_Manual"
description: "Converted .docx document from SF47_TSMit_Implementation/doc."
---

> **Converted document.** Source: `SF47_TSMit_Implementation/doc/TSMit_Integration_Manual.docx` (Word .docx, converted automatically; formatting, tables and figures preserved as Markdown — consult the original for normative layout).

# Integration Manual – Torque Steer Mitigation

Table of Contents

## Dependencies

### SWCs

| Module | Required Feature |
| --- | --- |
| None |  |

Note : Referencing the external components should be avoided in most cases. Only in unavoidable circumstance external components should be refered. Developer should track the references.

### Global Functions(Non RTE) to be provided to Integration Project

None

## Configuration

### Build Time Config

| Modules | Notes |  |
| --- | --- | --- |
| None |  |  |

### Configuration Files to be provided by Integration Project

None

#### Da Vinci Parameter Configuration Changes

| Parameter | Notes | SWC |
| --- | --- | --- |
| None |  |  |

#### DaVinci Interrupt Configuration Changes

| ISR Name | VIM # | Priority Dependency | Notes |
| --- | --- | --- | --- |
| None |  |  |  |

#### Manual Configuration Changes

| Constant | Notes | SWC |
| --- | --- | --- |
| None |  |  |

## Integration

### Required Global Data Inputs

- HandwheelAuthority_Uls_f32
- HandwheelPosition_HwDeg_f32
- HandwheelVelocity_HwRadpS_f32
- HwTorque_HwNm_f32
- PreLimitMtrTrqCmd_MtrNm_f32
- SrlComABSActive_Cnt_lgc
- SrlComESCActive_Cnt_lgc
- SrlComTCSActive_Cnt_lgc
- SrlComTransmissionTrq_TransNm_f32
- SrlComYawRate_DegpS_f32
- VehicleSpeed_Kph_f32
### Required Global Data Outputs

- TSMitCommand_MtrNm_f32
- TSMitLearningEnabled_Cnt_lgc
### Specific Include Path present

No

## Runnable Scheduling

This section specifies the required runnable scheduling.

| Init | Scheduling Requirements | Trigger |
| --- | --- | --- |
| TSMit_Init1 | None | On Init |

| Runnable | Scheduling Requirements | Trigger |
| --- | --- | --- |
| TSMit_Per1 | None | RTE (10ms) |

## Memory Mapping

### Mapping

| Memory Section | Contents | Notes |
| --- | --- | --- |
| TSMIT_START_SEC_VAR_CLEARED_32 | float32, uint32 |  |
| TSMIT_START_SEC_VAR_CLEARED_UNSPECIFIED | LPF32KSV_Str |  |

* Each …START_SEC… constant is terminated by a …STOP_SEC… constant as specified in the AUTOSAR Memory Mapping requirements.

### Usage

| Feature | RAM | ROM |
| --- | --- | --- |
| N/A |  |  |

Table 1: ARM Cortex R4 Memory Usage

### Non  RTE NvM Blocks

| Block Name |
| --- |
| None |

Note : Size of the NVM block if configured in developer

### RTE NvM Blocks

| Block Name |
| --- |
| Rte_Pim_TSMitGainLrn |
| Rte_Pim_TSMitDisableEOL |

Note : Size of the NVM block if configured in developer

## Compiler Settings

### Preprocessor MACRO

None

### Optimization Settings

N/A

## Revision Control Log

| **Rev #** | **Change Description** | **Date ** | **Author** |
| --- | --- | --- | --- |
| 1 | Initial version | 24-Jul-14 | JWJ |
