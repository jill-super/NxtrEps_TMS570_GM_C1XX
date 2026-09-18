---
title: "Integration — report/index_WithPS"
description: "Converted document index_WithPS.pdf."
---

> **Converted document.** Source: `GM_C1XX_EPS_TMS570/SwProject/VehPwrMd/utp/Tessy/report/index_WithPS.pdf`.

## Page 1

### TEST OVERVIEW REPORT 2015-07-03, 13:17:21+0530

### Project VehPwrMd

© Report created by TESSY V3.1.12, report template V2.0 1

Summary Overall Test Object Results (including Coverage)

Total Test Objects: 5

Successful: 5

Failed: 0

Not Executed: 0

Date: 2015-07-03

Time: 13:17:21+0530

### Selected Project Items

Test Collection "C1XX_UnitTest"

### Used Test Environments

TI TMS 570 PLS UDE (Default)

Test Case Results for Each Test Object (without Coverage)

The table above shows each test object on the x axis and the number of test cases of the respective test

object on the y axis. Each bar is divided into passed, not executed and failed test cases. The test case results

do not take into account any coverage result (i.e. if all test cases of a test object are passed in this table but

the coverage is failed, the overall test object result will be failed).

Statement (C0) Coverage: Total Statements for Each Test Object

The table above shows each test object on the x axis and the number of statements of the respective test

object on the y axis. Each bar is divided into reached statements (i.e. statements that have been executed

during the test) and unreached statements.



## Page 2

### TEST OVERVIEW REPORT 2015-07-03, 13:17:21+0530

### Project VehPwrMd

© Report created by TESSY V3.1.12, report template V2.0 2

Branch (C1) Coverage: Total Branches for Each Test Object

The table above shows each test object on the x axis and the number of branches of the respective test object

on the y axis. Each bar is divided into reached branches (i.e. branches that have been executed during the

test) and unreached branches.

Decision Coverage: Total Decision Outcomes for Each Test Object

The table above shows test objects on the x axis and the number of possible outcomes of all decisions of the

respective test object on the y axis. To achieve full DC coverage, each decision must evaluate to both true and

false.

Each bar is divided into reached and unreached decision outcomes.

MC/DC Coverage: Total Condition Combinations for Each Test Object

The table above shows test objects on the x axis and the number of condition combinations of all decisions of

the respective test object on the y axis. The number of condition combinations is based on the number of

boolean conditions within each decision of the test object. To achieve full MC/DC coverage, each decision

requires all contained atomic conditions to evaluate to both true and false independently of all other conditions.

The cumulated number of rows within such tables of condition combinations is what is displayed in this table.

Each bar is divided into reached condition combinations (i.e. combinations of boolean condition values that

have been executed during the test) and unreached condition combinations.



## Page 3

### TEST OVERVIEW REPORT 2015-07-03, 13:17:21+0530

### Project VehPwrMd

© Report created by TESSY V3.1.12, report template V2.0 3

MCC Coverage: Total Condition Combinations for Each Test Object

The table above shows test objects on the x axis and the number of condition combinations of all decisions of

the respective test object on the y axis. The number of condition combinations is based on the number of

boolean conditions within each decision of the test object. To achieve full MCC coverage, each decision

requires all contained atomic conditions to evaluate to all possible combinations of true and false values. The

cumulated number of rows within such tables of condition combinations is what is displayed in this table.

Each bar is divided into reached condition combinations (i.e. combinations of boolean condition values that

have been executed during the test) and unreached condition combinations.



## Page 4

### TEST OVERVIEW REPORT 2015-07-03, 13:17:21+0530

### Project VehPwrMd

© Report created by TESSY V3.1.12, report template V2.0 4

### Test Object List

The following table lists all test objects with their test case and coverage results. The cumulated results for modules, folders and test collections are also displayed, the

indentation within the name column indicates the parent relationship of the elements.

Please note that only test objects are numbered within the first column. This number is referenced on the x axis within the overview charts for test case and coverage results

available on previous pages (if included into the report).

No. Name C0 C1 DC MC/DC MCC Test Cases Result

VehPwrMd 100 % 100 % 100 % 100 % 100 % 9 of 9 passed

C1XX_UnitTest 100 % 100 % 100 % 100 % 100 % 9 of 9 passed

VehPwrMd 100 % 100 % 100 % 100 % 100 % 9 of 9 passed

1 IgnFailureDiag 100 % 100 % 100 % 100 % 100 % 3 of 3 passed

2 VehPwrMd_Init1 100 % 100 % - - - 1 of 1 passed

3 VehPwrMd_Per1 100 % 100 % 100 % 100 % 100 % 3 of 3 passed

4 VehPwrMd_Trns1 100 % 100 % - - - 1 of 1 passed

5 VehPwrMd_Trns2 100 % 100 % - - - 1 of 1 passed



## Page 5

### TEST DETAILS REPORT 2015-07-03, 13:12:52+0530

### IgnFailureDiag

© Report created by TESSY V3.1.12, report template V2.1 1

### Project VehPwrMd

### Module VehPwrMd

### Test Object IgnFailureDiag

Instrumentation: Test Object Only

Statement (C0) Coverage 100 %

Decision Coverage 100 %

Branch (C1) Coverage 100 %

MCC Coverage 100 %

MC/DC Coverage 100 %

### Statistics

Total Testcases 3

Successful 3

Failed 0

Not Executed 0

### Module Properties

Project Root Directory D:\Synergy_Work_Area\VehPwrMd

Configuration File D:\Synergy_Work_Area\VehPwrMd\UnitTestEnv\config\TMS570_GCC_UDE_CCS4_Config.xml

Target Environment TI TMS 570 PLS UDE (Default)

### Kind of Test Unit Test

### Linker Options

Source File(s)

File $(PROJECTROOT)\VehPwrMd\src\Ap_VehPwrMd.c

Compiler Options -Dconst= -D_DATA_ACCESS= -Dstatic= -I$(PROJECTROOT)\VehPwrMd\utp\contract -I$(PROJECTROOT)\StdDef\include -I$

(PROJECTROOT)\NxtrLib\include -I$(Compiler Install Path)\include -I$(PROJECTROOT)\VehPwrMd\include -I$(PROJECTROOT)

\VehPwrMd\utp\contract\Ap_VehPwrMd

### Comments/Description/Specification

### Name Text

Module 'VehPwrMd' *****************************************************************************

Name of Tester:	Spoorti Mali

Code File(s) Under Test:	  Ap_VehPwrMd.c

Code File(s) Version:	2

Module Design Document:	Vehicle_Power_Mode_MDD.docx

Module Design Document Version:	1

Data Dictionary Version:	2

Unit Test Plan Version:	2

Optimization Level:	Level 2

Compiler (CodeGen) Version:	TMS470_4.9.5

Model Type:	Excel Macro

Model Version:	Nexteer EPS Unit Test Tool 2.7d/EPS Library 1.32

Total FLASH Used (Bytes):	416

Total RAM Used (Bytes):	8

Total CALS Used (Bytes):	14

Special Test Requirements:

Test Date:	07-03-2015

Comments:	"Note 1: Inline functions defined in globalmacro.h are not unit tested.

Note 2: ""CBD_Sandbox_dbg.map""map file is embedded for reference."

*****************************************************************************

### Attributes

### Name Value

Compiler Install Path $(ProgramFiles)\Texas Instruments\ccsv4\tools\compiler\tms470_4.9.5

Float Precision 9

InitObjDir $(PROJECTROOT)\UnitTestEnv\static_build_files\obj

InitSrcDir $(PROJECTROOT)\UnitTestEnv\static_build_files\src

Linker File $(PROJECTROOT)\UnitTestEnv\static_build_files\sys_link.cmd

Makefile Template $(PROJECTROOT)\UnitTestEnv\config\Nexteer_ts_make_ude_ti_tms570_ps.tpl

Target Install Path $(ProgramFiles)\pls\UDE 3.2

### Timer Enabled false

Timer Prescale 0

Timer Resolution 1

### Timer Unit Cycles



## Page 6

### TEST DETAILS REPORT 2015-07-03, 13:12:52+0530

### IgnFailureDiag

© Report created by TESSY V3.1.12, report template V2.1 2

### Attributes

### Name Value

UDE Config File $(PROJECTROOT)\UnitTestEnv\config\TMS570_UDE_12PIN_JTAG.cfg

Workspace File D:\Synergy_Work_Area\VehPwrMd\UnitTestEnv\config\UDE_TMS570_DEBUG.WSP



## Page 7

### TEST DETAILS REPORT 2015-07-03, 13:12:52+0530

### IgnFailureDiag

© Report created by TESSY V3.1.12, report template V2.1 3

Test Case 1: Metrics Test

Specification Performance Metrics (With "None" Instrumentation

and WithPS Environment)

Cycles:

TS1.1  1039.00 Cycles

TS1.2  1119.00 Cycles

Description Vector Description:

TS1.1   "Shortest Execution Path

if (((TRUE == SrlComEngOn_Cnt_T_lgc)F || (TRUE == SrlComSPMOn_Cnt_T_lgc)) F&& (FALSE == EPSEn_Cnt_T_lgc))F"

TS1.2   "Longest Execution Path

if (((TRUE == SrlComEngOn_Cnt_T_lgc)T || (TRUE == SrlComSPMOn_Cnt_T_lgc)) F&& (FALSE == EPSEn_Cnt_T_lgc))F"

Test Step 1.1 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 0

IGNDiagStartTime_mS_M_u32p0 100

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 0

SrlComSPMOn_Cnt_T_lgc 0

k_IGNDiagTime_mS_u16p0 3400

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 1230

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 89089

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 89089 89089

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Test Step 1.2 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 0

IGNDiagStartTime_mS_M_u32p0 200

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 1

SrlComSPMOn_Cnt_T_lgc 0

k_IGNDiagTime_mS_u16p0 2500

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 40000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 9999

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 200 200

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1



## Page 8

### TEST DETAILS REPORT 2015-07-03, 13:12:52+0530

### IgnFailureDiag

© Report created by TESSY V3.1.12, report template V2.1 4

Test Case 2: Boundary Test

Specification Performance Metrics (With "None" Instrumentation

and WithPS Environment)

Cycles:

TS2.1   1141.00 Cycles

TS2.2   1108.00 Cycles

TS2.3   1013.00 Cycles

TS2.4   1039.00 Cycles

TS2.5   1013.00 Cycles

TS2.6   1031.00 Cycles

TS2.7   1088.00 Cycles

TS2.8   564.00 Cycles

TS2.9   556.00 Cycles

TS2.10   1048.00 Cycles

TS2.11   1031.00 Cycles

TS2.12   1031.00 Cycles

TS2.13   995.00 Cycles

TS2.14   995.00 Cycles

TS2.15   995.00 Cycles

TS2.16   995.00 Cycles

TS2.17   1031.00 Cycles

Description Vector Description:

TS2.1	SrlComEngOn_Cnt_T_lgc=>min

TS2.2	SrlComEngOn_Cnt_T_lgc=>max

TS2.3	SrlComSPMOn_Cnt_T_lgc=>min

TS2.4	SrlComSPMOn_Cnt_T_lgc=>max

TS2.5	EPSEn_Cnt_T_lgc=>min

TS2.6	EPSEn_Cnt_T_lgc=>max

TS2.7	k_IGNDiagTime_mS_u16p0=>min

TS2.8	k_IGNDiagTime_mS_u16p0=>max

TS2.9	k_IGNDiagTime_mS_u16p0=>mid/Default

TS2.10	Rte_Call_SystemTime_DtrmnElapsedTime_mS_u16=>min

TS2.11	Rte_Call_SystemTime_DtrmnElapsedTime_mS_u16=>max

TS2.12	Rte_Call_SystemTime_DtrmnElapsedTime_mS_u16=>mid

TS2.13	Rte_Call_SystemTime_GetSystemTime_mS_u32=>min

TS2.14	Rte_Call_SystemTime_GetSystemTime_mS_u32=>max

TS2.15	Rte_Call_SystemTime_GetSystemTime_mS_u32=>mid

TS2.16	All min

TS2.17	All max

Test Step 2.1 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 0

IGNDiagStartTime_mS_M_u32p0 1596

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 0

SrlComSPMOn_Cnt_T_lgc 1

k_IGNDiagTime_mS_u16p0 300

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 4500

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 5555

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1596 1596

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Test Step 2.2 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 1

IGNDiagStartTime_mS_M_u32p0 2514

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 1

SrlComSPMOn_Cnt_T_lgc 0

k_IGNDiagTime_mS_u16p0 4000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 3000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 6666

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 6666 6666

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1



## Page 9

### TEST DETAILS REPORT 2015-07-03, 13:12:52+0530

### IgnFailureDiag

© Report created by TESSY V3.1.12, report template V2.1 5

### Name Actual Value Expected Value Result

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Test Step 2.3 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 0

IGNDiagStartTime_mS_M_u32p0 7485

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 0

SrlComSPMOn_Cnt_T_lgc 0

k_IGNDiagTime_mS_u16p0 250

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 4525

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 7777

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 7777 7777

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Test Step 2.4 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 1

IGNDiagStartTime_mS_M_u32p0 9325

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 1

SrlComSPMOn_Cnt_T_lgc 1

k_IGNDiagTime_mS_u16p0 5500

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 1230

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 8888

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 8888 8888

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1



## Page 10

### TEST DETAILS REPORT 2015-07-03, 13:12:52+0530

### IgnFailureDiag

© Report created by TESSY V3.1.12, report template V2.1 6

Test Step 2.5 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 0

IGNDiagStartTime_mS_M_u32p0 8541

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 0

SrlComSPMOn_Cnt_T_lgc 0

k_IGNDiagTime_mS_u16p0 2500

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 40000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 9999

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 9999 9999

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Test Step 2.6 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 1

IGNDiagStartTime_mS_M_u32p0 6325

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 1

SrlComSPMOn_Cnt_T_lgc 0

k_IGNDiagTime_mS_u16p0 1200

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 55200

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 1000

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1000 1000

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Test Step 2.7 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 0

IGNDiagStartTime_mS_M_u32p0 4500

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 1

SrlComSPMOn_Cnt_T_lgc 0

k_IGNDiagTime_mS_u16p0 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 35000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 1234

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 4500 4500

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1



## Page 11

### TEST DETAILS REPORT 2015-07-03, 13:12:52+0530

### IgnFailureDiag

© Report created by TESSY V3.1.12, report template V2.1 7

Test Step 2.8 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 0

IGNDiagStartTime_mS_M_u32p0 3000

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 0

SrlComSPMOn_Cnt_T_lgc 1

k_IGNDiagTime_mS_u16p0 60000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 41250

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 645

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 3000 3000

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 *none*

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 *none*

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 *none*

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Test Step 2.9 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 0

IGNDiagStartTime_mS_M_u32p0 4525

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 1

SrlComSPMOn_Cnt_T_lgc 1

k_IGNDiagTime_mS_u16p0 5000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 2300

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 6867

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 4525 4525

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 *none*

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 *none*

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 *none*

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Test Step 2.10 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 0

IGNDiagStartTime_mS_M_u32p0 1230

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 1

SrlComSPMOn_Cnt_T_lgc 1

k_IGNDiagTime_mS_u16p0 123

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 89089

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1230 1230

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 *none*

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 *none*

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 *none*

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1



## Page 12

### TEST DETAILS REPORT 2015-07-03, 13:12:52+0530

### IgnFailureDiag

© Report created by TESSY V3.1.12, report template V2.1 8

Test Step 2.11 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 0

IGNDiagStartTime_mS_M_u32p0 40000

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 1

SrlComSPMOn_Cnt_T_lgc 1

k_IGNDiagTime_mS_u16p0 4500

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 65535

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 1452

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 40000 40000

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Test Step 2.12 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 0

IGNDiagStartTime_mS_M_u32p0 55200

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 1

SrlComSPMOn_Cnt_T_lgc 1

k_IGNDiagTime_mS_u16p0 6500

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 38000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 6874

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 55200 55200

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Test Step 2.13 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 1

IGNDiagStartTime_mS_M_u32p0 35000

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 0

SrlComSPMOn_Cnt_T_lgc 0

k_IGNDiagTime_mS_u16p0 8000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 1230

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 0

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 0 0

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0



## Page 13

### TEST DETAILS REPORT 2015-07-03, 13:12:52+0530

### IgnFailureDiag

© Report created by TESSY V3.1.12, report template V2.1 9

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Test Step 2.14 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 1

IGNDiagStartTime_mS_M_u32p0 41250

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 0

SrlComSPMOn_Cnt_T_lgc 0

k_IGNDiagTime_mS_u16p0 7500

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 40000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 4294967295

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 4294967295 4294967295

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Test Step 2.15 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 1

IGNDiagStartTime_mS_M_u32p0 2300

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 0

SrlComSPMOn_Cnt_T_lgc 0

k_IGNDiagTime_mS_u16p0 4500

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 55200

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 2147483647

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 2147483647 2147483647

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Test Step 2.16 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 0

IGNDiagStartTime_mS_M_u32p0 0

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 0

SrlComSPMOn_Cnt_T_lgc 0

k_IGNDiagTime_mS_u16p0 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 0

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 0 0

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184



## Page 14

### TEST DETAILS REPORT 2015-07-03, 13:12:52+0530

### IgnFailureDiag

© Report created by TESSY V3.1.12, report template V2.1 10

### Name Actual Value Expected Value Result

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Test Step 2.17 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 1

IGNDiagStartTime_mS_M_u32p0 4294967295

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 1

SrlComSPMOn_Cnt_T_lgc 1

k_IGNDiagTime_mS_u16p0 60000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 65535

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 4294967295

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 4294967295 4294967295

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Test Case 3: Path Test

Specification Performance Metrics (With "None" Instrumentation

and WithPS Environment)

Cycles:

TC3.1   4496.00 Cycles

TC3.2   3502.00 Cycles

TC3.3   3880.00 Cycles

TC3.4   3092.00 Cycles

TC3.5   3161.00 Cycles

TC3.6   4757.00 Cycles

Description Vector Description:

TC3.1   if (((TRUE == SrlComEngOn_Cnt_T_lgc)T || (TRUE == SrlComSPMOn_Cnt_T_lgc)) F&& (FALSE == EPSEn_Cnt_T_lgc))F

TC3.2   if (((TRUE == SrlComEngOn_Cnt_T_lgc)F || (TRUE == SrlComSPMOn_Cnt_T_lgc)) T&& (FALSE == EPSEn_Cnt_T_lgc))T

TC3.3   if (((TRUE == SrlComEngOn_Cnt_T_lgc)F || (TRUE == SrlComSPMOn_Cnt_T_lgc)) F&& (FALSE == EPSEn_Cnt_T_lgc))F

TC3.4   if (((TRUE == SrlComEngOn_Cnt_T_lgc)T|| (TRUE == SrlComSPMOn_Cnt_T_lgc))T&& (FALSE == EPSEn_Cnt_T_lgc))T

TC3.5   (((TRUE == SrlComEngOn_Cnt_T_lgc)==>False || (TRUE == SrlComSPMOn_Cnt_T_lgc)==>False) && (FALSE == EPSEn_Cnt_T_lgc))

TC3.6   (((TRUE == SrlComEngOn_Cnt_T_lgc)==>False || (TRUE == SrlComSPMOn_Cnt_T_lgc)==>True) && (FALSE ==

EPSEn_Cnt_T_lgc)==>True)

Test Step 3.1 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 0

IGNDiagStartTime_mS_M_u32p0 100

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 1

SrlComSPMOn_Cnt_T_lgc 0

k_IGNDiagTime_mS_u16p0 2500

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 40000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 9999

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 100 100

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1



## Page 15

### TEST DETAILS REPORT 2015-07-03, 13:12:52+0530

### IgnFailureDiag

© Report created by TESSY V3.1.12, report template V2.1 11

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Test Step 3.2 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 1

IGNDiagStartTime_mS_M_u32p0 200

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 0

SrlComSPMOn_Cnt_T_lgc 1

k_IGNDiagTime_mS_u16p0 4500

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 65535

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 1452

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1452 1452

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Test Step 3.3 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 0

IGNDiagStartTime_mS_M_u32p0 300

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 1

SrlComSPMOn_Cnt_T_lgc 0

k_IGNDiagTime_mS_u16p0 3400

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 1230

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 89089

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 300 300

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 *none*

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 *none*

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Test Step 3.4 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 1

IGNDiagStartTime_mS_M_u32p0 400

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 1

SrlComSPMOn_Cnt_T_lgc 1

k_IGNDiagTime_mS_u16p0 123

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 1230

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 89089

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 89089 89089

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1



## Page 16

### TEST DETAILS REPORT 2015-07-03, 13:12:52+0530

### IgnFailureDiag

© Report created by TESSY V3.1.12, report template V2.1 12

### Name Actual Value Expected Value Result

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Test Step 3.5 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 0

IGNDiagStartTime_mS_M_u32p0 7485

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 0

SrlComSPMOn_Cnt_T_lgc 0

k_IGNDiagTime_mS_u16p0 250

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 4525

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 7777

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 7777 7777

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Test Step 3.6 (Repeat Count = 1)

### Name Input Value

EPSEn_Cnt_T_lgc 0

IGNDiagStartTime_mS_M_u32p0 1596

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

SrlComEngOn_Cnt_T_lgc 0

SrlComSPMOn_Cnt_T_lgc 1

k_IGNDiagTime_mS_u16p0 300

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 4500

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 5555

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1596 1596

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1



## Page 17

### TEST DETAILS REPORT 2015-07-03, 13:16:03+0530

VehPwrMd_Trns1

© Report created by TESSY V3.1.12, report template V2.1 1

### Project VehPwrMd

### Module VehPwrMd

Test Object VehPwrMd_Trns1

Instrumentation: Test Object Only

Statement (C0) Coverage 100 %

Branch (C1) Coverage 100 %

### Statistics

Total Testcases 1

Successful 1

Failed 0

Not Executed 0

### Module Properties

Project Root Directory D:\Synergy_Work_Area\VehPwrMd

Configuration File D:\Synergy_Work_Area\VehPwrMd\UnitTestEnv\config\TMS570_GCC_UDE_CCS4_Config.xml

Target Environment TI TMS 570 PLS UDE (Default)

### Kind of Test Unit Test

### Linker Options

Source File(s)

File $(PROJECTROOT)\VehPwrMd\src\Ap_VehPwrMd.c

Compiler Options -Dconst= -D_DATA_ACCESS= -Dstatic= -I$(PROJECTROOT)\VehPwrMd\utp\contract -I$(PROJECTROOT)\StdDef\include -I$

(PROJECTROOT)\NxtrLib\include -I$(Compiler Install Path)\include -I$(PROJECTROOT)\VehPwrMd\include -I$(PROJECTROOT)

\VehPwrMd\utp\contract\Ap_VehPwrMd

### Comments/Description/Specification

### Name Text

Module 'VehPwrMd' *****************************************************************************

Name of Tester:	Spoorti Mali

Code File(s) Under Test:	  Ap_VehPwrMd.c

Code File(s) Version:	2

Module Design Document:	Vehicle_Power_Mode_MDD.docx

Module Design Document Version:	1

Data Dictionary Version:	2

Unit Test Plan Version:	2

Optimization Level:	Level 2

Compiler (CodeGen) Version:	TMS470_4.9.5

Model Type:	Excel Macro

Model Version:	Nexteer EPS Unit Test Tool 2.7d/EPS Library 1.32

Total FLASH Used (Bytes):	416

Total RAM Used (Bytes):	8

Total CALS Used (Bytes):	14

Special Test Requirements:

Test Date:	07-03-2015

Comments:	"Note 1: Inline functions defined in globalmacro.h are not unit tested.

Note 2: ""CBD_Sandbox_dbg.map""map file is embedded for reference."

*****************************************************************************

### Attributes

### Name Value

Compiler Install Path $(ProgramFiles)\Texas Instruments\ccsv4\tools\compiler\tms470_4.9.5

Float Precision 9

InitObjDir $(PROJECTROOT)\UnitTestEnv\static_build_files\obj

InitSrcDir $(PROJECTROOT)\UnitTestEnv\static_build_files\src

Linker File $(PROJECTROOT)\UnitTestEnv\static_build_files\sys_link.cmd

Makefile Template $(PROJECTROOT)\UnitTestEnv\config\Nexteer_ts_make_ude_ti_tms570_ps.tpl

Target Install Path $(ProgramFiles)\pls\UDE 3.2

### Timer Enabled false

Timer Prescale 0

Timer Resolution 1

### Timer Unit Cycles

UDE Config File $(PROJECTROOT)\UnitTestEnv\config\TMS570_UDE_12PIN_JTAG.cfg

Workspace File D:\Synergy_Work_Area\VehPwrMd\UnitTestEnv\config\UDE_TMS570_DEBUG.WSP



## Page 18

### TEST DETAILS REPORT 2015-07-03, 13:16:03+0530

VehPwrMd_Trns1

© Report created by TESSY V3.1.12, report template V2.1 2

Test Case 1: Boundary Test

Specification Performance Metrics (With "None" Instrumentation

and WithPS Environment)

Cycles:

TS1.1  1092.00 Cycles

Description Vector Description:

TS1.1: Call trace is checked

Test Step 1.1 (Repeat Count = 1)

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

CanStop 2 CanStop 2



## Page 19

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 1

### Project VehPwrMd

### Module VehPwrMd

Test Object VehPwrMd_Per1

Instrumentation: Test Object Only

Statement (C0) Coverage 100 %

Decision Coverage 100 %

Branch (C1) Coverage 100 %

MCC Coverage 100 %

MC/DC Coverage 100 %

### Statistics

Total Testcases 3

Successful 3

Failed 0

Not Executed 0

### Module Properties

Project Root Directory D:\Synergy_Work_Area\VehPwrMd

Configuration File D:\Synergy_Work_Area\VehPwrMd\UnitTestEnv\config\TMS570_GCC_UDE_CCS4_Config.xml

Target Environment TI TMS 570 PLS UDE (Default)

### Kind of Test Unit Test

### Linker Options

Source File(s)

File $(PROJECTROOT)\VehPwrMd\src\Ap_VehPwrMd.c

Compiler Options -Dconst= -D_DATA_ACCESS= -Dstatic= -I$(PROJECTROOT)\VehPwrMd\utp\contract -I$(PROJECTROOT)\StdDef\include -I$

(PROJECTROOT)\NxtrLib\include -I$(Compiler Install Path)\include -I$(PROJECTROOT)\VehPwrMd\include -I$(PROJECTROOT)

\VehPwrMd\utp\contract\Ap_VehPwrMd

### Comments/Description/Specification

### Name Text

Module 'VehPwrMd' *****************************************************************************

Name of Tester:	Spoorti Mali

Code File(s) Under Test:	  Ap_VehPwrMd.c

Code File(s) Version:	2

Module Design Document:	Vehicle_Power_Mode_MDD.docx

Module Design Document Version:	1

Data Dictionary Version:	2

Unit Test Plan Version:	2

Optimization Level:	Level 2

Compiler (CodeGen) Version:	TMS470_4.9.5

Model Type:	Excel Macro

Model Version:	Nexteer EPS Unit Test Tool 2.7d/EPS Library 1.32

Total FLASH Used (Bytes):	416

Total RAM Used (Bytes):	8

Total CALS Used (Bytes):	14

Special Test Requirements:

Test Date:	07-03-2015

Comments:	"Note 1: Inline functions defined in globalmacro.h are not unit tested.

Note 2: ""CBD_Sandbox_dbg.map""map file is embedded for reference."

*****************************************************************************

### Attributes

### Name Value

Compiler Install Path $(ProgramFiles)\Texas Instruments\ccsv4\tools\compiler\tms470_4.9.5

Float Precision 9

InitObjDir $(PROJECTROOT)\UnitTestEnv\static_build_files\obj

InitSrcDir $(PROJECTROOT)\UnitTestEnv\static_build_files\src

Linker File $(PROJECTROOT)\UnitTestEnv\static_build_files\sys_link.cmd

Makefile Template $(PROJECTROOT)\UnitTestEnv\config\Nexteer_ts_make_ude_ti_tms570_ps.tpl

Target Install Path $(ProgramFiles)\pls\UDE 3.2

### Timer Enabled false

Timer Prescale 0

Timer Resolution 1

### Timer Unit Cycles



## Page 20

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 2

### Attributes

### Name Value

UDE Config File $(PROJECTROOT)\UnitTestEnv\config\TMS570_UDE_12PIN_JTAG.cfg

Workspace File D:\Synergy_Work_Area\VehPwrMd\UnitTestEnv\config\UDE_TMS570_DEBUG.WSP



## Page 21

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 3

Test Case 1: Metrics Test

Specification Performance Metrics (With "None" Instrumentation

and WithPS Environment)

Cycles:

TS1.1   3615.00 Cycles

TS1.2   3411.00 Cycles

Description Vector Description:

TS1.1   "Longest Execution Path:

if (TRUE == EngONSrlComSvcDft_Cnt_T_lgc)=>FALSE,

if ((TRUE == EPSEn_Cnt_T_lgc) ||

((RTE_MODE_StaMd_Mode_OPERATE == SystemState_Cnt_T_enum) &&

(TRUE == SrlComSPMOn_Cnt_T_lgc)))=>FALSE,

if (((TRUE == SrlComEngOn_Cnt_T_lgc) &&

(FALSE == EngMissingFlt_Cnt_T_lgc)) ||

((RTE_MODE_StaMd_Mode_OPERATE == SystemState_Cnt_T_enum) &&

(TRUE == VehSpdValid_Cnt_T_lgc) &&

(VehSpd_Kph_T_f32 > k_RmpDnAsstVehSpdLimit_Kph_f32)))=>FALSE,

if ((FALSE == CTermActive_Cnt_T_lgc) || (FALSE == ATermActive_Cnt_T_lgc))=>TRUE"

TS1.2   "Shortest Execution Path:

if (TRUE == EngONSrlComSvcDft_Cnt_T_lgc)=>TRUE,

if (TRUE == EPSEn_Cnt_T_lgc)=>TRUE"

Test Step 1.1 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 1234

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 0

k_IGNDiagTime_mS_u16p0 300

k_RampDnRt_UlspmS_f32 0.100000001

k_RampUpRtLoSpd_UlspmS_f32 0.200000003

k_RmpDnAsstVehSpdLimit_Kph_f32 125.300003

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 4500

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 5555

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 120.300003

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1234 1234

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.100000001 0.100000001 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1



## Page 22

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 4

Test Step 1.2 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 645

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 4

k_IGNDiagTime_mS_u16p0 4000

k_RampDnRt_UlspmS_f32 0.200000003

k_RampUpRtLoSpd_UlspmS_f32 0.300000012

k_RmpDnAsstVehSpdLimit_Kph_f32 254.100006

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 3000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 6666

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 250.5

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 6666 6666

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.300000012 0.300000012 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1



## Page 23

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 5

Test Case 2: Boundary Test

Specification Performance Metrics (With "None" Instrumentation

and WithPS Environment)

Cycles:

TS2.1   3615.00 Cycles

TS2.2   3411.00 Cycles

TS2.3   3461.00 Cycles

TS2.4   3372.00 Cycles

TS2.5   3439.00 Cycles

TS2.6   3372.00 Cycles

TS2.7   3439.00 Cycles

TS2.8   3372.00 Cycles

TS2.9   3441.00 Cycles

TS2.10   3408.00 Cycles

TS2.11   3441.00 Cycles

TS2.12   3450.00 Cycles

TS2.13   3540.00 Cycles

TS2.14   3417.00 Cycles

TS2.15   3481.00 Cycles

TS2.16   3494.00 Cycles

TS2.17   3408.00 Cycles

TS2.18   3496.00 Cycles

TS2.19   3424.00 Cycles

TS2.20   3343.00 Cycles

TS2.21   2956.00 Cycles

TS2.22   3465.00 Cycles

TS2.23   3382.00 Cycles

TS2.24   3424.00 Cycles

TS2.25   3415.00 Cycles

TS2.26   3373.00 Cycles

TS2.27   3441.00 Cycles

TS2.28   3408.00 Cycles

TS2.29   3372.00 Cycles

TS2.30   3423.00 Cycles

TS2.31   3372.00 Cycles

TS2.32   3374.00 Cycles

Description Vector Description:

TS2.1	EngONSrlComSvcDft_Cnt_lgc=>Min

TS2.2	EngONSrlComSvcDft_Cnt_lgc=>Max

TS2.3	SrlComEngOn_Cnt_lgc=>Min

TS2.4	SrlComEngOn_Cnt_lgc=>Max

TS2.5	SrlComSPMOn_Cnt_lgc=>Min

TS2.6	SrlComSPMOn_Cnt_lgc=>Max

TS2.7	VehSpdValid_Cnt_lgc=>Min

TS2.8	VehSpdValid_Cnt_lgc=>Max

TS2.9	VehSpd_Kph_f32=>Min

TS2.10	VehSpd_Kph_f32=>Max

TS2.11	VehSpd_Kph_f32=>Mid

TS2.12	k_RmpDnAsstVehSpdLimit_Kph_f32=Min

TS2.13	k_RmpDnAsstVehSpdLimit_Kph_f32=Max

TS2.14	k_RmpDnAsstVehSpdLimit_Kph_f32=Mid

TS2.15	k_RmpDnAsstVehSpdLimit_Kph_f32=Default

TS2.16	k_RampDnRt_UlspmS_f32=>Min

TS2.17	k_RampDnRt_UlspmS_f32=>Max

TS2.18	k_RampDnRt_UlspmS_f32=>Mid/Default

TS2.19	k_RampUpRtLoSpd_UlspmS_f32=>Min

TS2.20	k_RampUpRtLoSpd_UlspmS_f32=>Max

TS2.21	k_RampUpRtLoSpd_UlspmS_f32=>Mid/Default

TS2.22	Rte_Call_NxtrDiagMgr_GetNTCFailed=Min

TS2.23	Rte_Call_NxtrDiagMgr_GetNTCFailed=>Max

TS2.24	Rte_Mode_SystemState_Mode=>RTE_MODE_StaMd_Mode_DISABLE

TS2.25	Rte_Mode_SystemState_Mode=>RTE_MODE_StaMd_Mode_OFF

TS2.26	Rte_Mode_SystemState_Mode=>RTE_MODE_StaMd_Mode_OPERATE

TS2.27	Rte_Mode_SystemState_Mode=>RTE_MODE_StaMd_Mode_WARMINIT

TS2.28	Rte_Mode_SystemState_Mode=>RTE_TRANSITION_StaMd_Mode

TS2.29	Rte_Call_EpsEn_OP_GET=>Min

TS2.30	Rte_Call_EpsEn_OP_GET=>Max

TS2.31	All min

TS2.32	All max

Test Step 2.1 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 1234

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 0

k_IGNDiagTime_mS_u16p0 300

k_RampDnRt_UlspmS_f32 0.100000001

k_RampUpRtLoSpd_UlspmS_f32 0.200000003

k_RmpDnAsstVehSpdLimit_Kph_f32 125.300003

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 4500

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 5555

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc



## Page 24

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 6

### Name Input Value

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 120.300003

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1234 1234

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.100000001 0.100000001 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.2 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 645

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 4

k_IGNDiagTime_mS_u16p0 4000

k_RampDnRt_UlspmS_f32 0.200000003

k_RampUpRtLoSpd_UlspmS_f32 0.300000012

k_RmpDnAsstVehSpdLimit_Kph_f32 254.100006

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 3000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 6666

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 250.5

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 6666 6666

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1



## Page 25

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 7

### Name Actual Value Expected Value Result

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.300000012 0.300000012 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.3 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 6867

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 1

k_IGNDiagTime_mS_u16p0 250

k_RampDnRt_UlspmS_f32 0.300000012

k_RampUpRtLoSpd_UlspmS_f32 0.400000006

k_RmpDnAsstVehSpdLimit_Kph_f32 250.5

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 4525

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 7777

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 40.2000008

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 6867 6867

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.300000012 0.300000012 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1



## Page 26

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 8

Test Step 2.4 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 89089

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 5500

k_RampDnRt_UlspmS_f32 0.400000006

k_RampUpRtLoSpd_UlspmS_f32 0.5

k_RmpDnAsstVehSpdLimit_Kph_f32 40.2000008

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 1230

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 8888

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 112.199997

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 8888 8888

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.5 0.5 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.5 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 1452

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 3

k_IGNDiagTime_mS_u16p0 2500

k_RampDnRt_UlspmS_f32 0.5

k_RampUpRtLoSpd_UlspmS_f32 0.600000024

k_RmpDnAsstVehSpdLimit_Kph_f32 112.199997

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 40000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 9999

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc



## Page 27

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 9

### Name Input Value

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 85.3000031

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 9999 9999

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.5 0.5 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.6 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 6874

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 4

k_IGNDiagTime_mS_u16p0 1200

k_RampDnRt_UlspmS_f32 0.600000024

k_RampUpRtLoSpd_UlspmS_f32 0.75

k_RmpDnAsstVehSpdLimit_Kph_f32 85.3000031

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 55200

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 1000

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 90.5

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1000 1000

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1



## Page 28

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 10

### Name Actual Value Expected Value Result

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.75 0.75 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.7 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 8888

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 1

k_IGNDiagTime_mS_u16p0 250

k_RampDnRt_UlspmS_f32 0.75

k_RampUpRtLoSpd_UlspmS_f32 0.800000012

k_RmpDnAsstVehSpdLimit_Kph_f32 90.5

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 35000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 1234

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 140.5

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1234 1234

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.75 0.75 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1



## Page 29

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 11

Test Step 2.8 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 9999

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 5500

k_RampDnRt_UlspmS_f32 0.800000012

k_RampUpRtLoSpd_UlspmS_f32 0.899999976

k_RmpDnAsstVehSpdLimit_Kph_f32 140.5

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 41250

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 645

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 400

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 645 645

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.899999976 0.899999976 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.9 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 1000

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 3

k_IGNDiagTime_mS_u16p0 2500

k_RampDnRt_UlspmS_f32 0.899999976

k_RampUpRtLoSpd_UlspmS_f32 0.0199999996

k_RmpDnAsstVehSpdLimit_Kph_f32 140.5

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 2300

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 6867

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc



## Page 30

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 12

### Name Input Value

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 0

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 6867 6867

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.899999976 0.899999976 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.10 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 1234

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 1200

k_RampDnRt_UlspmS_f32 0.0199999996

k_RampUpRtLoSpd_UlspmS_f32 0.0500000007

k_RmpDnAsstVehSpdLimit_Kph_f32 155.199997

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 1230

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 89089

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 511

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1234 1234

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0



## Page 31

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 13

### Name Actual Value Expected Value Result

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.0199999996 0.0199999996 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.11 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 645

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 4500

k_RampDnRt_UlspmS_f32 0.0500000007

k_RampUpRtLoSpd_UlspmS_f32 0.200000003

k_RmpDnAsstVehSpdLimit_Kph_f32 254.100006

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 40000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 1452

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 250.199997

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1452 1452

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.200000003 0.200000003 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1



## Page 32

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 14

Test Step 2.12 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 6867

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 6500

k_RampDnRt_UlspmS_f32 0.200000003

k_RampUpRtLoSpd_UlspmS_f32 0.0199999996

k_RmpDnAsstVehSpdLimit_Kph_f32 0

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 55200

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 6874

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 350.200012

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 6867 6867

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.0199999996 0.0199999996 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.13 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 89089

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 8000

k_RampDnRt_UlspmS_f32 0.0199999996

k_RampUpRtLoSpd_UlspmS_f32 0.0500000007

k_RmpDnAsstVehSpdLimit_Kph_f32 255

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 35000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 8888

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc



## Page 33

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 15

### Name Input Value

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 254.100006

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 8888 8888

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.0199999996 0.0199999996 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.14 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 1452

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 3

k_IGNDiagTime_mS_u16p0 7500

k_RampDnRt_UlspmS_f32 0.0500000007

k_RampUpRtLoSpd_UlspmS_f32 0.75

k_RmpDnAsstVehSpdLimit_Kph_f32 120.5

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 41250

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 9999

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 250.5

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1452 1452

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1



## Page 34

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 16

### Name Actual Value Expected Value Result

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.75 0.75 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.15 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 1234

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 1200

k_RampDnRt_UlspmS_f32 0.0199999996

k_RampUpRtLoSpd_UlspmS_f32 0.0500000007

k_RmpDnAsstVehSpdLimit_Kph_f32 10

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 1230

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 89089

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 511

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1234 1234

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.0199999996 0.0199999996 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1



## Page 35

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 17

Test Step 2.16 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 6874

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 4500

k_RampDnRt_UlspmS_f32 2.99999992e-005

k_RampUpRtLoSpd_UlspmS_f32 0.800000012

k_RmpDnAsstVehSpdLimit_Kph_f32 125.300003

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 55200

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 1000

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 40.2000008

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 6874 6874

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 2.99999992e-005 2.99999992e-005 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.17 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 8888

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 250

k_RampDnRt_UlspmS_f32 1

k_RampUpRtLoSpd_UlspmS_f32 0.899999976

k_RmpDnAsstVehSpdLimit_Kph_f32 254.100006

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 1230

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 1234

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc



## Page 36

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 18

### Name Input Value

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 112.199997

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1234 1234

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 1 1 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.18 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 9999

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 5500

k_RampDnRt_UlspmS_f32 0.000500000024

k_RampUpRtLoSpd_UlspmS_f32 0.0199999996

k_RmpDnAsstVehSpdLimit_Kph_f32 250.5

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 40000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 645

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 85.3000031

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 9999 9999

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0



## Page 37

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 19

### Name Actual Value Expected Value Result

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.000500000024 0.000500000024 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.19 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 1000

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 2500

k_RampDnRt_UlspmS_f32 0.300000012

k_RampUpRtLoSpd_UlspmS_f32 2.99999992e-005

k_RmpDnAsstVehSpdLimit_Kph_f32 40.2000008

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 55200

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 6867

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 90.5

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 6867 6867

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 2.99999992e-005 2.99999992e-005 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1



## Page 38

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 20

Test Step 2.20 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 1234

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 1200

k_RampDnRt_UlspmS_f32 0.400000006

k_RampUpRtLoSpd_UlspmS_f32 1

k_RmpDnAsstVehSpdLimit_Kph_f32 112.199997

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 35000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 89089

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 140.5

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 89089 89089

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 1 1 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.21 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 645

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 250

k_RampDnRt_UlspmS_f32 0.5

k_RampUpRtLoSpd_UlspmS_f32 0.000500000024

k_RmpDnAsstVehSpdLimit_Kph_f32 85.3000031

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 41250

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 1452

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc



## Page 39

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 21

### Name Input Value

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 400

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1452 1452

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.000500000024 0.000500000024 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.22 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 6867

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 3

k_IGNDiagTime_mS_u16p0 5500

k_RampDnRt_UlspmS_f32 0.600000024

k_RampUpRtLoSpd_UlspmS_f32 0.200000003

k_RmpDnAsstVehSpdLimit_Kph_f32 90.5

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 1230

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 6874

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 250.5

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 6867 6867

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 *none*

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 *none*

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1



## Page 40

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 22

### Name Actual Value Expected Value Result

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.200000003 0.200000003 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.23 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 89089

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 2500

k_RampDnRt_UlspmS_f32 0.75

k_RampUpRtLoSpd_UlspmS_f32 0.300000012

k_RmpDnAsstVehSpdLimit_Kph_f32 140.5

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 40000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 8888

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 40.2000008

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 8888 8888

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.75 0.75 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.24 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 5555



## Page 41

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 23

### Name Input Value

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 0

k_IGNDiagTime_mS_u16p0 1200

k_RampDnRt_UlspmS_f32 0.800000012

k_RampUpRtLoSpd_UlspmS_f32 0.400000006

k_RmpDnAsstVehSpdLimit_Kph_f32 110.300003

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 55200

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 9999

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 112.199997

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 5555 5555

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.800000012 0.800000012 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.25 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 6666

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 1

k_IGNDiagTime_mS_u16p0 250

k_RampDnRt_UlspmS_f32 0.899999976

k_RampUpRtLoSpd_UlspmS_f32 0.5

k_RmpDnAsstVehSpdLimit_Kph_f32 254.100006

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 35000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 1000

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32



## Page 42

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 24

### Name Input Value

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 85.3000031

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1000 1000

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.899999976 0.899999976 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.26 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 7777

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 5500

k_RampDnRt_UlspmS_f32 0.0199999996

k_RampUpRtLoSpd_UlspmS_f32 0.600000024

k_RmpDnAsstVehSpdLimit_Kph_f32 250.5

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 41250

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 1234

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 90.5

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 7777 7777

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.0199999996 0.0199999996 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625



## Page 43

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 25

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.27 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 8888

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 3

k_IGNDiagTime_mS_u16p0 2500

k_RampDnRt_UlspmS_f32 0.0500000007

k_RampUpRtLoSpd_UlspmS_f32 0.75

k_RmpDnAsstVehSpdLimit_Kph_f32 40.2000008

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 1230

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 645

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 140.5

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 645 645

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.0500000007 0.0500000007 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.28 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 9999

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela



## Page 44

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 26

### Name Input Value

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 4

k_IGNDiagTime_mS_u16p0 1200

k_RampDnRt_UlspmS_f32 0.200000003

k_RampUpRtLoSpd_UlspmS_f32 0.800000012

k_RmpDnAsstVehSpdLimit_Kph_f32 112.199997

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 40000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 6867

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 400

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 9999 9999

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.200000003 0.200000003 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.29 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 1000

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 250

k_RampDnRt_UlspmS_f32 0.300000012

k_RampUpRtLoSpd_UlspmS_f32 0.899999976

k_RmpDnAsstVehSpdLimit_Kph_f32 85.3000031

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 55200

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 89089

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc



## Page 45

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 27

### Name Input Value

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 250.5

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1000 1000

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.300000012 0.300000012 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.30 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 2000

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 1

k_IGNDiagTime_mS_u16p0 5500

k_RampDnRt_UlspmS_f32 0.400000006

k_RampUpRtLoSpd_UlspmS_f32 0.0199999996

k_RmpDnAsstVehSpdLimit_Kph_f32 90.5

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 35000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 1452

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 40.2000008

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1452 1452

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.0199999996 0.0199999996 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625



## Page 46

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 28

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.31 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 0

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 0

k_IGNDiagTime_mS_u16p0 0

k_RampDnRt_UlspmS_f32 2.99999992e-005

k_RampUpRtLoSpd_UlspmS_f32 2.99999992e-005

k_RmpDnAsstVehSpdLimit_Kph_f32 0

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 0

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 0

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 0 0

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 2.99999992e-005 2.99999992e-005 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 2.32 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 4294967295

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela



## Page 47

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 29

### Name Input Value

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 4

k_IGNDiagTime_mS_u16p0 60000

k_RampDnRt_UlspmS_f32 1

k_RampUpRtLoSpd_UlspmS_f32 1

k_RmpDnAsstVehSpdLimit_Kph_f32 255

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 65535

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 4294967295

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 511

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 4294967295 4294967295

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 1 1 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1



## Page 48

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 30

Test Case 3: Path Test

Specification Performance Metrics (With "None" Instrumentation

and WithPS Environment)

Cycles:

TC3.1   9870.00 Cycles

TC3.2   6246.00 Cycles

TC3.3   9677.00 Cycles

TC3.4   6305.00 Cycles

TC3.5   9663.00 Cycles

TC3.6   11276.00 Cycles

TC3.7   10431.00 Cycles

TC3.8   10080.00 Cycles

TC3.9   10500.00 Cycles

TC3.10   10010.00 Cycles

TC3.11   10001.00 Cycles

TC3.12   10885.00 Cycles

Description Vector Description:

TC3.1   if (TRUE == EngONSrlComSvcDft_Cnt_T_lgc)=>FALSE

TC3.2   if (TRUE == EPSEn_Cnt_T_lgc)=>TRUE

TC3.3   "if ((TRUE == EPSEn_Cnt_T_lgc) ||

((RTE_MODE_StaMd_Mode_OPERATE == SystemState_Cnt_T_enum) &&

(TRUE == SrlComSPMOn_Cnt_T_lgc)))=>TRUE"

TC3.4   if (TRUE == EPSEn_Cnt_T_lgc)=>FALSE

TC3.5   "if ((FALSE == CTermActive_Cnt_T_lgc) || (FALSE == ATermActive_Cnt_T_lgc))=>FALSE,

if (((TRUE == SrlComEngOn_Cnt_T_lgc) &&

(FALSE == EngMissingFlt_Cnt_T_lgc)) ||

((RTE_MODE_StaMd_Mode_OPERATE == SystemState_Cnt_T_enum) &&

(TRUE == VehSpdValid_Cnt_T_lgc) &&

(VehSpd_Kph_T_f32 > k_RmpDnAsstVehSpdLimit_Kph_f32)))=>TRUE"

TC3.6   "((TRUE == EPSEn_Cnt_T_lgc)==>False ||

((RTE_MODE_StaMd_Mode_OPERATE == SystemState_Cnt_T_enum)==>True &&

(TRUE == SrlComSPMOn_Cnt_T_lgc)==>False))"

TC3.7   "((TRUE == EPSEn_Cnt_T_lgc)==>False ||

((RTE_MODE_StaMd_Mode_OPERATE == SystemState_Cnt_T_enum)==>True &&

(TRUE == SrlComSPMOn_Cnt_T_lgc)==>True))   &&  (((TRUE == SrlComEngOn_Cnt_T_lgc)==>False &&

(FALSE == EngMissingFlt_Cnt_T_lgc)) ||

((RTE_MODE_StaMd_Mode_OPERATE == SystemState_Cnt_T_enum)==>True &&

(TRUE == VehSpdValid_Cnt_T_lgc)==>False &&

(VehSpd_Kph_T_f32 > k_RmpDnAsstVehSpdLimit_Kph_f32)))"

TC3.8   "(((TRUE == SrlComEngOn_Cnt_T_lgc)==>False &&

(FALSE == EngMissingFlt_Cnt_T_lgc)) ||

((RTE_MODE_StaMd_Mode_OPERATE == SystemState_Cnt_T_enum)==>True &&

(TRUE == VehSpdValid_Cnt_T_lgc)==>True &&

(VehSpd_Kph_T_f32 > k_RmpDnAsstVehSpdLimit_Kph_f32)))"

TC3.9   "(((TRUE == SrlComEngOn_Cnt_T_lgc)==>False &&

(FALSE == EngMissingFlt_Cnt_T_lgc)) ||

((RTE_MODE_StaMd_Mode_OPERATE == SystemState_Cnt_T_enum)==>True &&

(TRUE == VehSpdValid_Cnt_T_lgc)==>True &&

(VehSpd_Kph_T_f32 > k_RmpDnAsstVehSpdLimit_Kph_f32)==>True))"

TC3.10   ((FALSE == CTermActive_Cnt_T_lgc)==>False || (FALSE == ATermActive_Cnt_T_lgc)==>True)

TC3.11   "(((TRUE == SrlComEngOn_Cnt_T_lgc) ==>True&&

(FALSE == EngMissingFlt_Cnt_T_lgc))==>False ||

((RTE_MODE_StaMd_Mode_OPERATE == SystemState_Cnt_T_enum)==>True &&

(TRUE == VehSpdValid_Cnt_T_lgc)==>False &&

(VehSpd_Kph_T_f32 > k_RmpDnAsstVehSpdLimit_Kph_f32)))"

TC3.12   "(((TRUE == SrlComEngOn_Cnt_T_lgc) ==>True&&

(FALSE == EngMissingFlt_Cnt_T_lgc))==>False ||

((RTE_MODE_StaMd_Mode_OPERATE == SystemState_Cnt_T_enum)==>True &&

(TRUE == VehSpdValid_Cnt_T_lgc)==>True &&

(VehSpd_Kph_T_f32 > k_RmpDnAsstVehSpdLimit_Kph_f32)==>True))"

Test Step 3.1 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 1234

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 0

k_IGNDiagTime_mS_u16p0 300

k_RampDnRt_UlspmS_f32 0.100000001

k_RampUpRtLoSpd_UlspmS_f32 0.200000003

k_RmpDnAsstVehSpdLimit_Kph_f32 125.300003

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 4500

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 5555

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32



## Page 49

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 31

### Name Input Value

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 120.300003

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1234 1234

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.100000001 0.100000001 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 3.2 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 645

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 4

k_IGNDiagTime_mS_u16p0 4000

k_RampDnRt_UlspmS_f32 0.200000003

k_RampUpRtLoSpd_UlspmS_f32 0.300000012

k_RmpDnAsstVehSpdLimit_Kph_f32 254.100006

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 3000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 6666

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 250.5

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 6666 6666

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.300000012 0.300000012 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625



## Page 50

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 32

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 3.3 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 1000

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 3

k_IGNDiagTime_mS_u16p0 2500

k_RampDnRt_UlspmS_f32 0.899999976

k_RampUpRtLoSpd_UlspmS_f32 0.0199999996

k_RmpDnAsstVehSpdLimit_Kph_f32 140.5

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 2300

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 6867

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 0

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 6867 6867

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.899999976 0.899999976 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 3.4 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 1234

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela



## Page 51

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 33

### Name Input Value

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 1200

k_RampDnRt_UlspmS_f32 0.0199999996

k_RampUpRtLoSpd_UlspmS_f32 0.0500000007

k_RmpDnAsstVehSpdLimit_Kph_f32 155.199997

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 1230

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 89089

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 511

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1234 1234

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.0199999996 0.0199999996 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 3.5 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 645

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 4500

k_RampDnRt_UlspmS_f32 0.0500000007

k_RampUpRtLoSpd_UlspmS_f32 0.200000003

k_RmpDnAsstVehSpdLimit_Kph_f32 254.100006

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 40000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 1452

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc



## Page 52

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 34

### Name Input Value

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 250.199997

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1452 1452

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.200000003 0.200000003 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 3.6 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 6874

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 4500

k_RampDnRt_UlspmS_f32 2.99999992e-005

k_RampUpRtLoSpd_UlspmS_f32 0.800000012

k_RmpDnAsstVehSpdLimit_Kph_f32 125.300003

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 55200

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 1000

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 40.2000008

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 6874 6874

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 2.99999992e-005 2.99999992e-005 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625



## Page 53

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 35

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 3.7 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 6867

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 6500

k_RampDnRt_UlspmS_f32 0.200000003

k_RampUpRtLoSpd_UlspmS_f32 0.0199999996

k_RmpDnAsstVehSpdLimit_Kph_f32 0

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 55200

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 6874

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 350.200012

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 6867 6867

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.0199999996 0.0199999996 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 3.8 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 8888

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela



## Page 54

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 36

### Name Input Value

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 250

k_RampDnRt_UlspmS_f32 1

k_RampUpRtLoSpd_UlspmS_f32 0.899999976

k_RmpDnAsstVehSpdLimit_Kph_f32 254.100006

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 1230

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 1234

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 112.199997

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1234 1234

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 1 1 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 3.9 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 1234

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 1200

k_RampDnRt_UlspmS_f32 0.400000006

k_RampUpRtLoSpd_UlspmS_f32 1

k_RmpDnAsstVehSpdLimit_Kph_f32 112.199997

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 35000

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 89089

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc



## Page 55

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 37

### Name Input Value

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 140.5

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 89089 89089

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 1 1 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 3.10 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 1452

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 3

k_IGNDiagTime_mS_u16p0 7500

k_RampDnRt_UlspmS_f32 0.0500000007

k_RampUpRtLoSpd_UlspmS_f32 0.75

k_RmpDnAsstVehSpdLimit_Kph_f32 120.5

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 0

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 0

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 41250

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 9999

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 250.5

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 1452 1452

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 1 1

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.75 0.75 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625



## Page 56

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 38

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1 Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 3.11 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 1000

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 2500

k_RampDnRt_UlspmS_f32 0.899999976

k_RampUpRtLoSpd_UlspmS_f32 0.0199999996

k_RmpDnAsstVehSpdLimit_Kph_f32 140.5

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 2300

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 6867

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 0

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 6867 6867

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 0 0

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.899999976 0.899999976 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 0 0 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1

Test Step 3.12 (Repeat Count = 1)

### Name Input Value

IGNDiagStartTime_mS_M_u32p0 1000

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET(signal) tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed(NTCFailed_Ptr_T_lgc) tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr

Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16(ElapsedTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela



## Page 57

### TEST DETAILS REPORT 2015-07-03, 13:15:30+0530

VehPwrMd_Per1

© Report created by TESSY V3.1.12, report template V2.1 39

### Name Input Value

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32(CurrentTime) tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren

Rte_Inst_Ap_VehPwrMd tgt_Rte_Inst_Ap_VehPwrMd

Rte_Mode_Ap_VehPwrMd_SystemState_Mode() 2

k_IGNDiagTime_mS_u16p0 2500

k_RampDnRt_UlspmS_f32 0.899999976

k_RampUpRtLoSpd_UlspmS_f32 0.0199999996

k_RmpDnAsstVehSpdLimit_Kph_f32 140.5

tgt_Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET_signal 1

tgt_Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed_NTCFailed_Ptr 1

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_DtrmnElapsedTime_mS_u16_Ela 2300

tgt_Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32_Curren 6867

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_ATermActive_Cnt_lgc tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_CTermActive_Cnt_lgc tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampRate_XpmS_f32 tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_OperRampValue_Uls_f32 tgt_VehPwrMd_Per1_OperRampValue_Uls_f32

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComEngOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpdValid_Cnt_lgc tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc

tgt_Rte_Inst_Ap_VehPwrMd.VehPwrMd_Per1_VehSpd_Kph_f32 tgt_VehPwrMd_Per1_VehSpd_Kph_f32

tgt_VehPwrMd_Per1_EngONSrlComSvcDft_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_SrlComEngOn_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_SrlComSPMOn_Cnt_lgc.value 0

tgt_VehPwrMd_Per1_VehSpdValid_Cnt_lgc.value 1

tgt_VehPwrMd_Per1_VehSpd_Kph_f32.value 255

### Name Actual Value Expected Value Result

IGNDiagStartTime_mS_M_u32p0 6867 6867

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(NTC_Cnt_T_enum) 184 184

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Param_Cnt_T_u08) 1 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus(Status_Cnt_T_enum) 0 0

tgt_VehPwrMd_Per1_ATermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_CTermActive_Cnt_lgc.value 1 1

tgt_VehPwrMd_Per1_OperRampRate_XpmS_f32.value 0.0199999996 0.0199999996 ± 0.0001

tgt_VehPwrMd_Per1_OperRampValue_Uls_f32.value 1 1 ± 0.00390625

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1 Rte_Call_Ap_VehPwrMd_EpsEn_OP_GET 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_GetNTCFailed 1

Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1 Rte_Mode_Ap_VehPwrMd_SystemState_Mode 1

IgnFailureDiag 1 IgnFailureDiag 1

Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1 Rte_Call_Ap_VehPwrMd_NxtrDiagMgr_SetNTCStatus 1

Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1 Rte_Call_Ap_VehPwrMd_SystemTime_GetSystemTime_mS_u32 1

Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1 Rte_Call_VehPwrMd_Per1_CP1_CheckpointReached 1



## Page 58

### TEST DETAILS REPORT 2015-07-03, 13:16:36+0530

VehPwrMd_Trns2

© Report created by TESSY V3.1.12, report template V2.1 1

### Project VehPwrMd

### Module VehPwrMd

Test Object VehPwrMd_Trns2

Instrumentation: Test Object Only

Statement (C0) Coverage 100 %

Branch (C1) Coverage 100 %

### Statistics

Total Testcases 1

Successful 1

Failed 0

Not Executed 0

### Module Properties

Project Root Directory D:\Synergy_Work_Area\VehPwrMd

Configuration File D:\Synergy_Work_Area\VehPwrMd\UnitTestEnv\config\TMS570_GCC_UDE_CCS4_Config.xml

Target Environment TI TMS 570 PLS UDE (Default)

### Kind of Test Unit Test

### Linker Options

Source File(s)

File $(PROJECTROOT)\VehPwrMd\src\Ap_VehPwrMd.c

Compiler Options -Dconst= -D_DATA_ACCESS= -Dstatic= -I$(PROJECTROOT)\VehPwrMd\utp\contract -I$(PROJECTROOT)\StdDef\include -I$

(PROJECTROOT)\NxtrLib\include -I$(Compiler Install Path)\include -I$(PROJECTROOT)\VehPwrMd\include -I$(PROJECTROOT)

\VehPwrMd\utp\contract\Ap_VehPwrMd

### Comments/Description/Specification

### Name Text

Module 'VehPwrMd' *****************************************************************************

Name of Tester:	Spoorti Mali

Code File(s) Under Test:	  Ap_VehPwrMd.c

Code File(s) Version:	2

Module Design Document:	Vehicle_Power_Mode_MDD.docx

Module Design Document Version:	1

Data Dictionary Version:	2

Unit Test Plan Version:	2

Optimization Level:	Level 2

Compiler (CodeGen) Version:	TMS470_4.9.5

Model Type:	Excel Macro

Model Version:	Nexteer EPS Unit Test Tool 2.7d/EPS Library 1.32

Total FLASH Used (Bytes):	416

Total RAM Used (Bytes):	8

Total CALS Used (Bytes):	14

Special Test Requirements:

Test Date:	07-03-2015

Comments:	"Note 1: Inline functions defined in globalmacro.h are not unit tested.

Note 2: ""CBD_Sandbox_dbg.map""map file is embedded for reference."

*****************************************************************************

### Attributes

### Name Value

Compiler Install Path $(ProgramFiles)\Texas Instruments\ccsv4\tools\compiler\tms470_4.9.5

Float Precision 9

InitObjDir $(PROJECTROOT)\UnitTestEnv\static_build_files\obj

InitSrcDir $(PROJECTROOT)\UnitTestEnv\static_build_files\src

Linker File $(PROJECTROOT)\UnitTestEnv\static_build_files\sys_link.cmd

Makefile Template $(PROJECTROOT)\UnitTestEnv\config\Nexteer_ts_make_ude_ti_tms570_ps.tpl

Target Install Path $(ProgramFiles)\pls\UDE 3.2

### Timer Enabled false

Timer Prescale 0

Timer Resolution 1

### Timer Unit Cycles

UDE Config File $(PROJECTROOT)\UnitTestEnv\config\TMS570_UDE_12PIN_JTAG.cfg

Workspace File D:\Synergy_Work_Area\VehPwrMd\UnitTestEnv\config\UDE_TMS570_DEBUG.WSP



## Page 59

### TEST DETAILS REPORT 2015-07-03, 13:16:36+0530

VehPwrMd_Trns2

© Report created by TESSY V3.1.12, report template V2.1 2

Test Case 1: Boundary Test

Specification Performance Metrics (With "None" Instrumentation

and WithPS Environment)

Cycles:

TS1.1  1997.00 Cycles

Description Vector Description:

TS1.1: Call trace is checked

Test Step 1.1 (Repeat Count = 1)

### Test Step Call Trace

### Actual Function Count Expected Function Count Result

SrlComInput_SCom_ResetBus1Timers 1 SrlComInput_SCom_ResetBus1Timers 1

SrlComInput_SCom_ResetBus2Timers 1 SrlComInput_SCom_ResetBus2Timers 1

CanStart 2 CanStart 2



## Page 60

### TEST DETAILS REPORT 2015-07-03, 13:13:31+0530

VehPwrMd_Init1

© Report created by TESSY V3.1.12, report template V2.1 1

### Project VehPwrMd

### Module VehPwrMd

Test Object VehPwrMd_Init1

Instrumentation: Test Object Only

Statement (C0) Coverage 100 %

Branch (C1) Coverage 100 %

### Statistics

Total Testcases 1

Successful 1

Failed 0

Not Executed 0

### Module Properties

Project Root Directory D:\Synergy_Work_Area\VehPwrMd

Configuration File D:\Synergy_Work_Area\VehPwrMd\UnitTestEnv\config\TMS570_GCC_UDE_CCS4_Config.xml

Target Environment TI TMS 570 PLS UDE (Default)

### Kind of Test Unit Test

### Linker Options

Source File(s)

File $(PROJECTROOT)\VehPwrMd\src\Ap_VehPwrMd.c

Compiler Options -Dconst= -D_DATA_ACCESS= -Dstatic= -I$(PROJECTROOT)\VehPwrMd\utp\contract -I$(PROJECTROOT)\StdDef\include -I$

(PROJECTROOT)\NxtrLib\include -I$(Compiler Install Path)\include -I$(PROJECTROOT)\VehPwrMd\include -I$(PROJECTROOT)

\VehPwrMd\utp\contract\Ap_VehPwrMd

### Comments/Description/Specification

### Name Text

Module 'VehPwrMd' *****************************************************************************

Name of Tester:	Spoorti Mali

Code File(s) Under Test:	  Ap_VehPwrMd.c

Code File(s) Version:	2

Module Design Document:	Vehicle_Power_Mode_MDD.docx

Module Design Document Version:	1

Data Dictionary Version:	2

Unit Test Plan Version:	2

Optimization Level:	Level 2

Compiler (CodeGen) Version:	TMS470_4.9.5

Model Type:	Excel Macro

Model Version:	Nexteer EPS Unit Test Tool 2.7d/EPS Library 1.32

Total FLASH Used (Bytes):	416

Total RAM Used (Bytes):	8

Total CALS Used (Bytes):	14

Special Test Requirements:

Test Date:	07-03-2015

Comments:	"Note 1: Inline functions defined in globalmacro.h are not unit tested.

Note 2: ""CBD_Sandbox_dbg.map""map file is embedded for reference."

*****************************************************************************

### Attributes

### Name Value

Compiler Install Path $(ProgramFiles)\Texas Instruments\ccsv4\tools\compiler\tms470_4.9.5

Float Precision 9

InitObjDir $(PROJECTROOT)\UnitTestEnv\static_build_files\obj

InitSrcDir $(PROJECTROOT)\UnitTestEnv\static_build_files\src

Linker File $(PROJECTROOT)\UnitTestEnv\static_build_files\sys_link.cmd

Makefile Template $(PROJECTROOT)\UnitTestEnv\config\Nexteer_ts_make_ude_ti_tms570_ps.tpl

Target Install Path $(ProgramFiles)\pls\UDE 3.2

### Timer Enabled false

Timer Prescale 0

Timer Resolution 1

### Timer Unit Cycles

UDE Config File $(PROJECTROOT)\UnitTestEnv\config\TMS570_UDE_12PIN_JTAG.cfg

Workspace File D:\Synergy_Work_Area\VehPwrMd\UnitTestEnv\config\UDE_TMS570_DEBUG.WSP



> Note: this PDF has 62 pages; only the first 60 were extracted. See the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/GM_C1XX_EPS_TMS570/SwProject/VehPwrMd/utp/Tessy/report/index_WithPS.pdf` for the remainder.

*Source PDF: `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/GM_C1XX_EPS_TMS570/SwProject/VehPwrMd/utp/Tessy/report/index_WithPS.pdf` — 62 page(s), text-extracted automatically.*
