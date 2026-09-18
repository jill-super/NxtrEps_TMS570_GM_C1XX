---
title: "GM C1XX EPS TMS570 integration project"
description: "GM_C1XX_EPS_TMS570: purpose, files, API and documents (RTE & System Integration)."
---

:::note[Mixed origin]
This integration area combines **Vector-provided** artefacts (MICROSAR BSW, generated RTE/OS data — do not modify) with **Custom** Nexteer integration code and SW-Cs.
:::
*Origin: **Mixed** — ECU integration project: Vector MICROSAR BSW/RTE/GenData (Vector-provided) plus Nexteer integration SW-Cs (Custom).*
## Purpose and responsibility
ECU integration project for the GM C1XX EPS on TI TMS570: Vector MICROSAR BSW, generated RTE/OS data (`SwProject/Source/GenData*`), interface SW-Cs (`SwProject/*`), linker/loader artefacts and host-side tools (`Tools/`).
## Key files
| Area | Files |
| --- | --- |
| Sources | See repository tree (integration-only area). |
## Public API
No C sources in this area (configuration, generated data or tooling only).
## Usage and dependencies
No project-internal `#include` dependencies detected (standalone or configuration-only).
## Documents
| Document | Source file |
| --- | --- |
| [Integration — report/index_WithOutPS](./GM_C1XX_EPS_TMS570-SwProject-index_WithOutPS/) | `GM_C1XX_EPS_TMS570/SwProject/CDDInterface/utp/Tessy/report/index_WithOutPS.pdf` |
| [Integration — report/index_WithPS](./GM_C1XX_EPS_TMS570-SwProject-index_WithPS/) | `GM_C1XX_EPS_TMS570/SwProject/CDDInterface/utp/Tessy/report/index_WithPS.pdf` |
| [Integration — doc/Customer_Periodic_Services_MDD](./GM_C1XX_EPS_TMS570-SwProject-Customer_Periodic_Services_MDD/) | `GM_C1XX_EPS_TMS570/SwProject/CustPerSrvcs/doc/Customer_Periodic_Services_MDD.doc` |
| [Integration — report/index_WithOutPS](./GM_C1XX_EPS_TMS570-SwProject-index_WithOutPS/) | `GM_C1XX_EPS_TMS570/SwProject/CustPerSrvcs/utp/Tessy/report/index_WithOutPS.pdf` |
| [Integration — report/index_WithPS](./GM_C1XX_EPS_TMS570-SwProject-index_WithPS/) | `GM_C1XX_EPS_TMS570/SwProject/CustPerSrvcs/utp/Tessy/report/index_WithPS.pdf` |
| [Integration — doc/DemIf_MDD](./GM_C1XX_EPS_TMS570-SwProject-DemIf_MDD/) | `GM_C1XX_EPS_TMS570/SwProject/DemIf/doc/DemIf_MDD.docx` |
| [Integration — report/index_WithOutPS](./GM_C1XX_EPS_TMS570-SwProject-index_WithOutPS/) | `GM_C1XX_EPS_TMS570/SwProject/DemIf/utp/Tessy/report/index_WithOutPS.pdf` |
| [Integration — report/index_WithPS](./GM_C1XX_EPS_TMS570-SwProject-index_WithPS/) | `GM_C1XX_EPS_TMS570/SwProject/DemIf/utp/Tessy/report/index_WithPS.pdf` |
| [Integration — report/index_WithOutPS](./GM_C1XX_EPS_TMS570-SwProject-index_WithOutPS/) | `GM_C1XX_EPS_TMS570/SwProject/DfltConfigData/utp/Tessy/report/index_WithOutPS.pdf` |
| [Integration — report/index_WithPS](./GM_C1XX_EPS_TMS570-SwProject-index_WithPS/) | `GM_C1XX_EPS_TMS570/SwProject/DfltConfigData/utp/Tessy/report/index_WithPS.pdf` |
| [Integration — report/index_WithOutPS](./GM_C1XX_EPS_TMS570-SwProject-index_WithOutPS/) | `GM_C1XX_EPS_TMS570/SwProject/IoHwAbstractionUsr/utp/Tessy/report/index_WithOutPS.pdf` |
| [Integration — report/index_WithPS](./GM_C1XX_EPS_TMS570-SwProject-index_WithPS/) | `GM_C1XX_EPS_TMS570/SwProject/IoHwAbstractionUsr/utp/Tessy/report/index_WithPS.pdf` |
| [Integration — doc/SASPlausDiag_MDD](./GM_C1XX_EPS_TMS570-SwProject-SASPlausDiag_MDD/) | `GM_C1XX_EPS_TMS570/SwProject/SASPlausDiag/doc/SASPlausDiag_MDD.docx` |
| [Integration — GenData/WdgM_Graph](./GM_C1XX_EPS_TMS570-SwProject-WdgM_Graph/) | `GM_C1XX_EPS_TMS570/SwProject/Source/GenData/WdgM_Graph.pdf` |
| [Integration — doc/Serial_Communication_Input_MDD](./GM_C1XX_EPS_TMS570-SwProject-Serial_Communication_Input_MDD/) | `GM_C1XX_EPS_TMS570/SwProject/SrlComInput/doc/Serial_Communication_Input_MDD.doc` |
| [Integration — report/index_WithOutPS](./GM_C1XX_EPS_TMS570-SwProject-index_WithOutPS/) | `GM_C1XX_EPS_TMS570/SwProject/SrlComInput/utp/Tessy/report/index_WithOutPS.pdf` |
| [Integration — report/index_WithPS](./GM_C1XX_EPS_TMS570-SwProject-index_WithPS/) | `GM_C1XX_EPS_TMS570/SwProject/SrlComInput/utp/Tessy/report/index_WithPS.pdf` |
| [Integration — doc/Vehicle_Power_Mode_MDD](./GM_C1XX_EPS_TMS570-SwProject-Vehicle_Power_Mode_MDD/) | `GM_C1XX_EPS_TMS570/SwProject/VehPwrMd/doc/Vehicle_Power_Mode_MDD.docx` |
| [Integration — report/index_WithOutPS](./GM_C1XX_EPS_TMS570-SwProject-index_WithOutPS/) | `GM_C1XX_EPS_TMS570/SwProject/VehPwrMd/utp/Tessy/report/index_WithOutPS.pdf` |
| [Integration — report/index_WithPS](./GM_C1XX_EPS_TMS570-SwProject-index_WithPS/) | `GM_C1XX_EPS_TMS570/SwProject/VehPwrMd/utp/Tessy/report/index_WithPS.pdf` |
| [Integration — doc/WIR_Input_Qualification_MDD](./GM_C1XX_EPS_TMS570-SwProject-WIR_Input_Qualification_MDD/) | `GM_C1XX_EPS_TMS570/SwProject/WIRInputQual/doc/WIR_Input_Qualification_MDD.docx` |
| [Integration — artt/ReleaseNotes_Artt_Generator](./GM_C1XX_EPS_TMS570-Tools-ReleaseNotes_Artt_Generator/) | `GM_C1XX_EPS_TMS570/Tools/AsrProject/Generators/Artt/artt/ReleaseNotes_Artt_Generator.pdf` |
| [Integration — HexView/ReferenceManual_HexView](./GM_C1XX_EPS_TMS570-Tools-ReferenceManual_HexView/) | `GM_C1XX_EPS_TMS570/Tools/HexView/ReferenceManual_HexView.pdf` |
| [Integration — HLDD/Build Environment](./GM_C1XX_EPS_TMS570-HLDD-Build-Environment/) | `GM_C1XX_EPS_TMS570/HLDD/Build Environment.docx` |

*Repository path: `GM_C1XX_EPS_TMS570/`* 
