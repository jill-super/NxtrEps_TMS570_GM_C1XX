---
title: "FrqDepDmpnInrtCmp — FrqDepDmpnInrtCmp Integration Manual"
description: "Converted .doc document from FrqDepDmpnInrtCmp/doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/FrqDepDmpnInrtCmp/doc/FrqDepDmpnInrtCmp Integration Manual.doc`.

- Integration Manual

- FreqDepDmpnInrtCmp

- VERSION: 1.0

- DATE: 15-OCT-2015

- Prepared By:

- Software Engineering Group>,

- Nexteer Automotive,

- Saginaw, MI, USA

- Revision History

- Initial version

- Jayakrishnan T

- Table of Contents

- TOC \o "1-2" \h \z \u

- HYPERLINK \l "_Toc432681071"

- Abbrevations And Acronyms

- PAGEREF _Toc432681071 \h

- HYPERLINK \l "_Toc432681072"

- PAGEREF _Toc432681072 \h

- HYPERLINK \l "_Toc432681073"

- Dependencies

- PAGEREF _Toc432681073 \h

- HYPERLINK \l "_Toc432681074"

- PAGEREF _Toc432681074 \h

- HYPERLINK \l "_Toc432681075"

- Global Functions(Non RTE) to be provided to Integration Project

- PAGEREF _Toc432681075 \h

- HYPERLINK \l "_Toc432681076"

- Configuration REQUIREMeNTS

- PAGEREF _Toc432681076 \h

- HYPERLINK \l "_Toc432681077"

- Build Time Config

- PAGEREF _Toc432681077 \h

- HYPERLINK \l "_Toc432681078"

- Configuration Files to be provided by Integration Project

- PAGEREF _Toc432681078 \h

- HYPERLINK \l "_Toc432681079"

- Da Vinci Parameter Configuration Changes

- PAGEREF _Toc432681079 \h

- HYPERLINK \l "_Toc432681080"

- DaVinci Interrupt Configuration Changes

- PAGEREF _Toc432681080 \h

- HYPERLINK \l "_Toc432681081"

- Manual Configuration Changes

- PAGEREF _Toc432681081 \h

- HYPERLINK \l "_Toc432681082"

- Integration DATAFLOW REQUIREMENTS

- PAGEREF _Toc432681082 \h

- HYPERLINK \l "_Toc432681083"

- Required Global Data Inputs

- PAGEREF _Toc432681083 \h

- HYPERLINK \l "_Toc432681084"

- Required Global Data Outputs

- PAGEREF _Toc432681084 \h

- HYPERLINK \l "_Toc432681085"

- Specific Include Path present

- PAGEREF _Toc432681085 \h

- HYPERLINK \l "_Toc432681086"

- Runnable Scheduling

- PAGEREF _Toc432681086 \h

- HYPERLINK \l "_Toc432681087"

- Memory Map REQUIREMENTS

- PAGEREF _Toc432681087 \h

- HYPERLINK \l "_Toc432681088"

- PAGEREF _Toc432681088 \h

- HYPERLINK \l "_Toc432681089"

- PAGEREF _Toc432681089 \h

- HYPERLINK \l "_Toc432681090"

- PAGEREF _Toc432681090 \h

- HYPERLINK \l "_Toc432681091"

- Compiler Settings

- PAGEREF _Toc432681091 \h

- HYPERLINK \l "_Toc432681092"

- Preprocessor MACRO

- PAGEREF _Toc432681092 \h

- HYPERLINK \l "_Toc432681093"

- Optimization Settings

- PAGEREF _Toc432681093 \h

- HYPERLINK \l "_Toc432681094"

- PAGEREF _Toc432681094 \h

- Abbreviation

- Design functional diagram

- Module design Document

- <ADD more to the table if applicable>

- This section lists the title & version of all the documents that are referred for development of this document

- Frequency_Dependant_Damping_And_Inertia_Compenstation_MDD

- SF14 InertiaCompFreqDepDamp

- <Add if more available>

- Required Feature

- Note : Referencing the external components should be avoided in most cases. Only in unavoidable circumstance external components should be referred. Developer should track the references.

- Priority Dependency

- BaseAssistCmd_MtrNm_f32

- CRFMotorVel_MtrRadpS_f32

- FreqDepDmpSrlComSvcDft_Cnt_lgc

- HwTorque_HwNm_f32

- VehicleLonAccel_KphpS_f32

- VehicleSpeed_Kph_f32

- WIRCmdAmpBlnd_MtrNm_f32

- FrqDepDmpnInrtCmp_MtrNm_f32

- This section specifies the required runnable scheduling.

- Scheduling Requirements

- FrqDepDmpnInrtCmp_Init

- FrqDepDmpnInrtCmp_Per1

- Disabled in DISABLE Mode

- Memory Section

- FRQDEPDMPNINRTCMP_START_SEC_VAR_CLEARED_32

- FRQDEPDMPNINRTCMP_START_SEC_VAR_CLEARED_UNSPECIFIED

- constant is terminated by a

- constant as specified in the AUTOSAR Memory Mapping requirements.

- SEQ Table \* ARABIC

- : ARM Cortex R4 Memory Usage

- <This section is for appendix>

- Nexteer Automotive Confidential Proprietary Information

- Do Not Copy/Distribute Without Prior Permission

- Integration Manual Template

- Version: 2.0 Date: 15-Oct-2015

- Nexteer Automotive

- PAGE \* Arabic \* MERGEFORMAT

- NUMPAGES \* MERGEFORMAT

- ~tjd[d[d[d[d
