---
title: "TrqOsc — Torque_Oscillation_Function_CM_MDD"
description: "Converted .doc document from TrqOsc/doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/TrqOsc/doc/Torque_Oscillation_Function_CM_MDD.doc`.

- Module Design Document

- Torque Oscillation Function

- DATE: April 3, 2014

- Prepared By:

- Software Group,

- Nexteer Automotive,

- Saginaw, MI, USA

- Location: The official version of this document is stored in the Nexteer Configuration Management System and is uniquely identified by: <Project_ID>_<Config Id>

- Revision History

- Started initial version of the MDD

- Lovepreet Kaur

- Table of Contents

- TOC \o "1-2" \h \z \u

- HYPERLINK \l "_Toc384291154"

- Abbrevations And Acronyms

- PAGEREF _Toc384291154 \h

- HYPERLINK \l "_Toc384291155"

- PAGEREF _Toc384291155 \h

- HYPERLINK \l "_Toc384291156"

- Torque_Oscillation_Fuction & High-Level Description

- PAGEREF _Toc384291156 \h

- HYPERLINK \l "_Toc384291157"

- Design details of software module

- PAGEREF _Toc384291157 \h

- HYPERLINK \l "_Toc384291158"

- Graphical representation of Torque_Oscillation

- PAGEREF _Toc384291158 \h

- HYPERLINK \l "_Toc384291159"

- Data Flow Diagram

- PAGEREF _Toc384291159 \h

- HYPERLINK \l "_Toc384291160"

- Module level DFD

- PAGEREF _Toc384291160 \h

- HYPERLINK \l "_Toc384291161"

- Sub-Module level DFD

- PAGEREF _Toc384291161 \h

- HYPERLINK \l "_Toc384291162"

- COMPONENT FLOW DIAGRAM

- PAGEREF _Toc384291162 \h

- HYPERLINK \l "_Toc384291163"

- Variable Data Dictionary

- PAGEREF _Toc384291163 \h

- HYPERLINK \l "_Toc384291164"

- User defined typedef definition/declaration

- PAGEREF _Toc384291164 \h

- HYPERLINK \l "_Toc384291165"

- Variable definition for enumerated types

- PAGEREF _Toc384291165 \h

- HYPERLINK \l "_Toc384291166"

- Constant Data Dictionary

- PAGEREF _Toc384291166 \h

- HYPERLINK \l "_Toc384291167"

- Program(fixed) Constants

- PAGEREF _Toc384291167 \h

- HYPERLINK \l "_Toc384291168"

- Embedded Constants

- PAGEREF _Toc384291168 \h

- HYPERLINK \l "_Toc384291169"

- PAGEREF _Toc384291169 \h

- HYPERLINK \l "_Toc384291170"

- PAGEREF _Toc384291170 \h

- HYPERLINK \l "_Toc384291171"

- Module specific Lookup Tables Constants

- PAGEREF _Toc384291171 \h

- HYPERLINK \l "_Toc384291172"

- Library Functions / Macros

- PAGEREF _Toc384291172 \h

- HYPERLINK \l "_Toc384291173"

- Data Hiding Functions

- PAGEREF _Toc384291173 \h

- HYPERLINK \l "_Toc384291174"

- Software Module Implementation

- PAGEREF _Toc384291174 \h

- HYPERLINK \l "_Toc384291175"

- Initialization Functions

- PAGEREF _Toc384291175 \h

- HYPERLINK \l "_Toc384291176"

- Init: TrqOsc_Init

- PAGEREF _Toc384291176 \h

- HYPERLINK \l "_Toc384291177"

- Design Rationale

- PAGEREF _Toc384291177 \h

- HYPERLINK \l "_Toc384291178"

- Module Outputs

- PAGEREF _Toc384291178 \h

- HYPERLINK \l "_Toc384291179"

- Module Internal

- PAGEREF _Toc384291179 \h

- HYPERLINK \l "_Toc384291180"

- PERIODIC FUNCTIONS

- PAGEREF _Toc384291180 \h

- HYPERLINK \l "_Toc384291181"

- Per: TrqOsc_Per1

- PAGEREF _Toc384291181 \h

- HYPERLINK \l "_Toc384291182"

- PAGEREF _Toc384291182 \h

- HYPERLINK \l "_Toc384291183"

- Store Module Inputs to Local copies

- PAGEREF _Toc384291183 \h

- HYPERLINK \l "_Toc384291184"

- (Processing of function)

- PAGEREF _Toc384291184 \h

- HYPERLINK \l "_Toc384291185"

- Store Local copy of outputs into Module Outputs

- PAGEREF _Toc384291185 \h

- HYPERLINK \l "_Toc384291186"

- Interrupt Functions

- PAGEREF _Toc384291186 \h

- HYPERLINK \l "_Toc384291187"

- Isr: <ModuleName>_Isr<n)>

- PAGEREF _Toc384291187 \h

- HYPERLINK \l "_Toc384291188"

- PAGEREF _Toc384291188 \h

- HYPERLINK \l "_Toc384291189"

- (Processing of the ISR function)

- PAGEREF _Toc384291189 \h

- HYPERLINK \l "_Toc384291190"

- TRANSIENT FUNCTIONS

- PAGEREF _Toc384291190 \h

- HYPERLINK \l "_Toc384291191"

- Per: <ModuleName>_Trns<n>

- PAGEREF _Toc384291191 \h

- HYPERLINK \l "_Toc384291192"

- PAGEREF _Toc384291192 \h

- HYPERLINK \l "_Toc384291193"

- PAGEREF _Toc384291193 \h

- HYPERLINK \l "_Toc384291194"

- PAGEREF _Toc384291194 \h

- HYPERLINK \l "_Toc384291195"

- PAGEREF _Toc384291195 \h

- HYPERLINK \l "_Toc384291196"

- Serial Communication Functions

- PAGEREF _Toc384291196 \h

- HYPERLINK \l "_Toc384291197"

- SComm: <MODULENAME>

- PAGEREF _Toc384291197 \h

- HYPERLINK \l "_Toc384291198"

- PAGEREF _Toc384291198 \h

- HYPERLINK \l "_Toc384291199"

- PAGEREF _Toc384291199 \h

- HYPERLINK \l "_Toc384291200"

- PAGEREF _Toc384291200 \h

- HYPERLINK \l "_Toc384291201"

- PAGEREF _Toc384291201 \h

- HYPERLINK \l "_Toc384291202"

- Local Function/Macro Definitions

- PAGEREF _Toc384291202 \h

- HYPERLINK \l "_Toc384291203"

- Local Function #1

- PAGEREF _Toc384291203 \h

- HYPERLINK \l "_Toc384291204"

- PAGEREF _Toc384291204 \h

- HYPERLINK \l "_Toc384291205"

- GLObAL Function/Macro Definitions

- PAGEREF _Toc384291205 \h

- HYPERLINK \l "_Toc384291206"

- GLObAL Function #1

- PAGEREF _Toc384291206 \h

- HYPERLINK \l "_Toc384291207"

- PAGEREF _Toc384291207 \h

- HYPERLINK \l "_Toc384291208"

- Known Limitations With Design

- PAGEREF _Toc384291208 \h

- HYPERLINK \l "_Toc384291209"

- UNIT TEST CONSIDERATION

- PAGEREF _Toc384291209 \h

- HYPERLINK \l "_Toc384291210"

- PAGEREF _Toc384291210 \h

- Abbreviation

- Design functional diagram

- Module design Document

- This section Lists the title & version of all the documents that are referred for development of this document

- MDD Guidelines

- Software Naming Conventions

- SF-43 Torque Oscillation

- This function lets motor to generate a sinusoidal torque command for a given frequency and fixed amplitude. This can be used to send a sudden alert to driver or for any other application. Frequency can assume only certain values and amplitude can be limited differently for each of those frequencies.

- EMBED Visio.Drawing.11

- Typedef Name

- Element Name

- User Defined Type

- Constant Name

- D_TRQOSCPERMMAXFREQ_HZ_U12P4

- D_TRQOSCPERMMINFREQ_HZ_U12P4

- D_TRQOSCMAXAMP_MTRNM_F32

- Single Precision Float

- D_TRQOSCMINAMP_MTRNM_F32

- D_TRQOSCMAXDC_MTRNM_F32

- D_TRQOSCDCTRENDLPFKN_HZ_F32

- D_FALSE_CNT_LGC

- D_2MS_SEC_F32

- D_2PI_ULS_F32

- D_ZERO_ULS_F32

- Software Segment

- FPM_InitFixedPoint_m

- LPF_KUpdate_f32_m

- LPF_OpUpdate_f32_m

- FPM_FloatToFixed_m

- FPM_FixedToFloat_m

- t need initialization because it is mapped to a cleared section in memory and therefore, LPF_KUpdate_f32_m function is used instead of the LPF complete macro.

- Since, Unit Delay logic in DC Compare flag is basically latching the DCExceeded Flag with the OR operand, no previous DC Compare flag has been defined or used in the code in order to implement the Unit-Delay logic. Only TrqOsc_DCExceeded_Cnt_M_lgc variable is used which is able to perform the latching operation with fewer lines of code.

- DOCPROPERTY "Module Name" \* MERGEFORMAT

- Function Name

- (Exact name used)

- Arguments Passed

- (if none, write None)

- <Refer MDD guidelines[1]>

- (Insert more rows for additional passed arguments)

- Return Value

- (if no value returned, write N/A)

- (Place flowchart/design for local function)

- Explanation of what should be and should not be mentioned in design rationale limitations

- <This section is for appendix>

- Nexteer Automotive Confidential Proprietary Information

- Do Not Copy/Distribute Without Prior Permission

- Module Design Document Template

- Version: 01 Date: 04/02/2014

- Document identifier: <Project_id>_<Config id>

- Nexteer Automotive

- PAGE \* Arabic \* MERGEFORMAT

- NUMPAGES \* MERGEFORMAT

- ulcXPXPXPXPXPX
