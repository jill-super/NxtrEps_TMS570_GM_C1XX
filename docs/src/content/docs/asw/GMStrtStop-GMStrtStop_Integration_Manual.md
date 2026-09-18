---
title: "GMStrtStop — GMStrtStop_Integration_Manual"
description: "Converted .doc document from GMStrtStop/doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/GMStrtStop/doc/GMStrtStop_Integration_Manual.doc`.

- Integration Manual

- VERSION: 23.0

- DATE: 203-JunMay-2016

- Prepared By:

- DOCPROPERTY "Prepared by Group" \* MERGEFORMAT

- Krishna Anne

- DOCPROPERTY "Prepared for Group" \* MERGEFORMAT

- Software Engineering

- DOCPROPERTY Company \* MERGEFORMAT

- Nexteer Automotive

- DOCPROPERTY Location \* MERGEFORMAT

- Saginaw, MI, USA

- Location: The official version of this document is stored in the Nexteer Configuration Management System.

- Revision History

- Initial Version

- Jared W Julien

- Updated to V002 of FDD

- (Updated t emplate too)

- Fix issues found with FDD during peer reviews

- Table of Contents

- TOC \o "1-2" \h \z \u

- HYPERLINK \l "_Toc452715865"

- Abbrevations And Acronyms

- PAGEREF _Toc452715865 \h

- HYPERLINK \l "_Toc452715866"

- PAGEREF _Toc452715866 \h

- HYPERLINK \l "_Toc452715867"

- Dependencies

- PAGEREF _Toc452715867 \h

- HYPERLINK \l "_Toc452715868"

- PAGEREF _Toc452715868 \h

- HYPERLINK \l "_Toc452715869"

- Global Functions(Non RTE) to be provided to Integration Project

- PAGEREF _Toc452715869 \h

- HYPERLINK \l "_Toc452715870"

- Configuration REQUIREMeNTS

- PAGEREF _Toc452715870 \h

- HYPERLINK \l "_Toc452715871"

- Build Time Config

- PAGEREF _Toc452715871 \h

- HYPERLINK \l "_Toc452715872"

- Configuration Files to be provided by Integration Project

- PAGEREF _Toc452715872 \h

- HYPERLINK \l "_Toc452715873"

- Da Vinci Parameter Configuration Changes

- PAGEREF _Toc452715873 \h

- HYPERLINK \l "_Toc452715874"

- DaVinci Interrupt Configuration Changes

- PAGEREF _Toc452715874 \h

- HYPERLINK \l "_Toc452715875"

- Manual Configuration Changes

- PAGEREF _Toc452715875 \h

- HYPERLINK \l "_Toc452715876"

- Integration DATAFLOW REQUIREMENTS

- PAGEREF _Toc452715876 \h

- HYPERLINK \l "_Toc452715877"

- Required Global Data Inputs

- PAGEREF _Toc452715877 \h

- HYPERLINK \l "_Toc452715878"

- Required Global Data Outputs

- PAGEREF _Toc452715878 \h

- HYPERLINK \l "_Toc452715879"

- Specific Include Path present

- PAGEREF _Toc452715879 \h

- HYPERLINK \l "_Toc452715880"

- Runnable Scheduling

- PAGEREF _Toc452715880 \h

- HYPERLINK \l "_Toc452715881"

- Memory Map REQUIREMENTS

- PAGEREF _Toc452715881 \h

- HYPERLINK \l "_Toc452715882"

- PAGEREF _Toc452715882 \h

- HYPERLINK \l "_Toc452715883"

- PAGEREF _Toc452715883 \h

- HYPERLINK \l "_Toc452715884"

- PAGEREF _Toc452715884 \h

- HYPERLINK \l "_Toc452715885"

- Compiler Settings

- PAGEREF _Toc452715885 \h

- HYPERLINK \l "_Toc452715886"

- Preprocessor MACRO

- PAGEREF _Toc452715886 \h

- HYPERLINK \l "_Toc452715887"

- Optimization Settings

- PAGEREF _Toc452715887 \h

- HYPERLINK \l "_Toc452715888"

- PAGEREF _Toc452715888 \h

- Abbreviation

- Design functional diagram

- Module design Document

- This section lists the title & version of all the documents that are referred for development of this document

- MDD Guidelines

- Software Naming Conventions

- Coding standards

- Required Feature

- Note : Referencing the external components should be avoided in most cases. Only in unavoidable circumstance external components should be referred. Developer should track the references.

- <Configuration file that will generated from this components that will require Da Vinci Config generation or manual generation. Describe each parameter >

- Priority Dependency

- Please refer to the FDD.

- This section specifies the required runnable scheduling.

- Scheduling Requirements

- StrtStop_Init1NA

- StrtStop_Per1

- Memory Section

- STRTSTOP_START_SEC_VAR_CLEARED_UNSPECIFIED

- STRTSTOP_START_SEC_VAR_CLEARED_32

- constant is terminated by a

- constant as specified in the AUTOSAR Memory Mapping requirements.

- SEQ Table \* ARABIC

- : ARM Cortex R4 Memory Usage

- Nexteer Automotive Confidential Proprietary Information

- Do Not Copy/Distribute Without Prior Permission

- GMSrtrStop Integration Manual

- Version: 32.0 Date: 2003-JunMay-2016

- PAGE \* Arabic \* MERGEFORMAT

- NUMPAGES \* MERGEFORMAT

- |m|m`m|m|m`m|YR
