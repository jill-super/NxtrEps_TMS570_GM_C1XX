---
title: "NxtrLib — Filter_Library_Design_Document"
description: "Converted .doc document from NxtrLib/doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/NxtrLib/doc/Filter_Library_Design_Document.doc`.

- s in hertz and T is in seconds.)

- And the equation for initialization of the state variable is as follows:

- Filt_SV = Input

- Coefficient K Recalculation

- The equation for recalculation of the filter coefficient K is exactly the sa

- Output Update Macro

- Function Name

- LPF_OpUpdate_f32_m

- Arguments Passed

- Input to low pass filter

- Pointer to the state variable structure

- LPF32KSV_Str

- TOC \o "1-4" \h \z

- HYPERLINK \l "_Toc323024626"

- Partial Notch Filter

- PAGEREF _Toc323024626 \h

- HYPERLINK \l "_Toc323024627"

- Filter Equations

- PAGEREF _Toc323024627 \h

- HYPERLINK \l "_Toc323024628"

- Node b State Variable Initialization

- PAGEREF _Toc323024628 \h

- HYPERLINK \l "_Toc323024629"

- Node d State Variable Initialization

- PAGEREF _Toc323024629 \h

- HYPERLINK \l "_Toc323024630"

- Filter Output Calculation

- PAGEREF _Toc323024630 \h

- HYPERLINK \l "_Toc323024631"

- Node b State Variable Calculation

- PAGEREF _Toc323024631 \h

- HYPERLINK \l "_Toc323024632"

- Node d State Variable Calculation

- PAGEREF _Toc323024632 \h

- HYPERLINK \l "_Toc323024633"

- PAGEREF _Toc323024633 \h

- HYPERLINK \l "_Toc323024634"

- Library Routines Design

- PAGEREF _Toc323024634 \h

- HYPERLINK \l "_Toc323024635"

- Notch Filter Initialization Function

- PAGEREF _Toc323024635 \h

- HYPERLINK \l "_Toc323024636"

- Notch Filter State Variable Update Function

- PAGEREF _Toc323024636 \h

- HYPERLINK \l "_Toc323024637"

- Notch Filter Output Update Function

- PAGEREF _Toc323024637 \h

- HYPERLINK \l "_Toc323024638"

- Notch Filter Full Update Function

- PAGEREF _Toc323024638 \h

- HYPERLINK \l "_Toc323024639"

- Notch Filter Structure Acceptable Ranges

- PAGEREF _Toc323024639 \h

- HYPERLINK \l "_Toc323024640"

- PAGEREF _Toc323024640 \h

- HYPERLINK \l "_Toc323024641"

- 1st Order Low Pass Filter, 1 Pole- coefficient

- PAGEREF _Toc323024641 \h

- HYPERLINK \l "_Toc323024642"

- PAGEREF _Toc323024642 \h

- HYPERLINK \l "_Toc323024643"

- PAGEREF _Toc323024643 \h

- HYPERLINK \l "_Toc323024644"

- PAGEREF _Toc323024644 \h

- HYPERLINK \l "_Toc323024645"

- Unity Gain, No Dead band Compensation, Fixed K

- calibratable Kn, fixed 16 bit Kd, 32 Bit State Variable, Truncate divide, Unsigned 16 bit Input

- PAGEREF _Toc323024645 \h

- HYPERLINK \l "_Toc323024646"

- calibratable Kn, fixed 16 bit Kd, 32 Bit State Variable, Truncate divide, Signed 16 bit Input

- PAGEREF _Toc323024646 \h

- HYPERLINK \l "_Toc323024647"

- PAGEREF _Toc323024647 \h

- HYPERLINK \l "_Toc323024648"

- PAGEREF _Toc323024648 \h

- HYPERLINK \l "_Toc323024649"

- PAGEREF _Toc323024649 \h

- HYPERLINK \l "_Toc323024650"

- Variable Gain, Variable D, Variable K

- calibratable 16 bit Kn, variable Kd, 32 Bit State Variable, Truncate divide, Unsigned 16 bit Input

- PAGEREF _Toc323024650 \h

- HYPERLINK \l "_Toc323024651"

- Variable Gain, Variable D, Variable K - calibratable 16 bit Kn, variable Kd, 32 Bit State Variable, Truncate divide, Signed 16 bit Input

- PAGEREF _Toc323024651 \h

- HYPERLINK \l "_Toc323024652"

- 1LP1-CF (Floating Point Implementation)

- PAGEREF _Toc323024652 \h

- HYPERLINK \l "_Toc323024653"

- PAGEREF _Toc323024653 \h

- HYPERLINK \l "_Toc323024654"

- Coefficient K Calculation and State Variable Initialization

- PAGEREF _Toc323024654 \h

- HYPERLINK \l "_Toc323024655"

- PAGEREF _Toc323024655 \h

- HYPERLINK \l "_Toc323024656"

- Normal Operation

- PAGEREF _Toc323024656 \h

- HYPERLINK \l "_Toc323024657"

- PAGEREF _Toc323024657 \h

- HYPERLINK \l "_Toc323024658"

- Unity Gain, No Dead band Compensation, calibratable K, Single-Precision Float Input

- PAGEREF _Toc323024658 \h

- HYPERLINK \l "_Toc323024659"

- 1st Order High Pass Filter, 1 Pole- coefficient

- PAGEREF _Toc323024659 \h

- HYPERLINK \l "_Toc323024660"

- HP-CF (Floating Point Implementation)

- PAGEREF _Toc323024660 \h

- HYPERLINK \l "_Toc323024661"

- PAGEREF _Toc323024661 \h

- HYPERLINK \l "_Toc323024662"

- PAGEREF _Toc323024662 \h

- HYPERLINK \l "_Toc323024663"

- PAGEREF _Toc323024663 \h

- HYPERLINK \l "_Toc323024664"

- PAGEREF _Toc323024664 \h

- HYPERLINK \l "_Toc323024665"

- PAGEREF _Toc323024665 \h

- HYPERLINK \l "_Toc323024666"

- PAGEREF _Toc323024666 \h

- HYPERLINK \l "_Toc323024667"

- Revision Control Log

- PAGEREF _Toc323024667 \h

- The first three equations, 1.1.1, 1.1.2, and 1.1.3 shall be combined into a single Notch Filter Initialization function. The next two equations 1.1.4 and 1.1.5 shall be combined into a single state variable update function. Finally, equation 1.1.6 shall be standalone as the output update function. For convenience, the last two function, state variable update and output update shall be combined int

- SV2 = In * (B2 - A2);

- SV1 = In * (B1 + B2 - A1 - A2);

- SV2 = (B2 * In) - (Out * A2);

- SV1 = (SV2 + (In * B1)) - (Out * A1);

- Out = SV1 + (B0 * In);

- In_Uls_T_f32

- Initial input to the filter

- SVPtr_Cnt_T_Str

- Pointer to state variable struct

- NotchFiltSV_Str

- FiltK_Cnt_T_Str

- Pointer to coefficient structure

- NotchFiltK_Str

- Return Value

- Pseudo Code:

- KPtr_Cnt_Str = FiltK_Cnt_T_Str;

- NF_SvUpdate_f32

- Input to notch filter

- SVPtr_T_Cnt_Str

- Pointer to filter cal struct

- KPtr_Cnt_Str = FiltK_Cnt_T_Str

- NF_OpUpdate_f32

- Input to the notch filter

- Filtered Output, SV Structure Updated

- NF_FullUpdate_f32

- Filtered output

- Full Update simply calls OpUpdate followed by SvUpdate as a convenient alternative to calling each of the functions individually.

- Structure Name

- KPtr_Cnt_Str

- For a module that executes a Notch Filter, in its _Init() sub module execute the following function.

- NF_Init_f32(<Input>, <SV_Ptr>, <FiltK_Ptr>);

- In the same module

- s _Per() sub module execute the following functions in the given sequence,

- NF_OpUpdate_f32(<Input>, <SV_Ptr>);

- NF_SvUpdate_f32(<Input>, <SV_Ptr>, <FiltK_Ptr>);

- Alternatively, a single call to the following function can be made in place of the above pair within the _Per() sub module.

- NF_FullUpdate_f32(<Input>, <SV_Ptr>, <FiltK_Ptr>);

- The Filter topology 1LP1-C is as given,

- There may be multiple library functions defined for the same topology, based on the cut-off frequency, and input size requirements.

- A filter tool is available to design the low pass filter for this topology

- 1st Order Design,1LP1-B.xls

- . This tool provides the bit sizes for all nodes shown in the filter. The tool must be used to see which library function is required for the given input, cut-off frequency, sampling rate, and filter coefficient size.

- The above filter topology requires the following constants to be defined

- Constant Classification

- Numerator of Filter Coefficient

- This may be defined as a calibration constant or an embedded local constant based on the usage.

- Denominator of Filter Coefficient

- Based on the implementation, this value may be a fixed value, which is embedded within the library function/macro or could be passed as a parameter.

- State Variable (filt_SV)

- Output (filt_O)

- The filter equations are given below. Each equation shall be implemented as a library macro.

- State Variable (Node e) Initialization

- The equation to initialize the state variable, (Node e) is as follows:

- filt_SV = Input * Kd.

- Output (Node O) Initialization

- The equation to initialize the output, (Node O) is as follows:

- filt_O = [( ( Input

- (filt_SV / Kd) ) * Kn ) + filt_SV] / Kd

- During normal operation the state variable (Node e) shall be updated prior to the output of the filter (Node O) being updated.

- The equation for the state variable (Node e) is as follows:

- filt_SV = ( ( Input

- (filt_SV / Kd) ) * Kn ) + filt_SV

- The equation for the output (Node O) is as follows:

- filt_O = filt_SV / Kd

- The equations to update filt_Sv and filt_O or the library routines that calculate these values should be executed in the exact order shown above.

- There will be four macros defined for this implementation:- state variable initialization, filter output initialization, state variable update and filter output update.

- State Variable Initialization Macro

- LPF_SvInit_u16InFixKTrunc_m

- Input to the low pass filter

- Initialized value of node e

- Lvalue = Input << Kd

- where Kd is pre-defined for a fixed16 bit filter coefficient = 16 bits

- Filter Output Initialization Macro

- LPF_OpInit_u16InFixKTrunc_m

- Initialized value of the state variable

- Kn - Numerator of the filter coefficient

- Initialized output of the low pass filter

- Lvalue = (((Input

- (Filt_SV >> Kd)) * Kn ), + Filt_SV)>>Kd

- Filter State Variable Update Macro

- LPF_SvUpdate_u16InFixKTrunc_m

- Calculated value of the state variable

- Output of the low pass filter

- Pseudo code:

- <Lvalue> = ( ( Input

- (filt_SV >> Kd) ) * Kn ) + filt_SV

- LPF_OpUpdate_u16InFixKTrunc_m

- <Lvalue> = filt_SV >> Kd

- where Kd is pre-defined for a 16 bit filter coefficient = 16 bits

- For a module that executes a LPF, in its _Init() sub module execute the following macros in the given sequence

- LPF_SvInit_u16InFixKTrunc_m (<Input>)

- LPF_OpInit_u16InFixKTrunc_m (<Input>, <Filt_SV>, <Kn>)

- s _Per() sub module execute the following macros in the given sequence,

- LPF_SvUpdate_u16InFixKTrunc_m (<Input>, <filt_SV>, <Kn>)

- LPF_OpUpdate_u16InFixKTrunc_m ( <filt_SV>)

- There will be three macros defined for this implementation:- state variable initialization, state variable update and filter output update.

- LPF_SvInit_s16InFixKTrunc_m

- Initilized value of Node e

- where Kd is pre-defined for a 16 bit filter coefficient as 16 bits

- LPF_OpInit_s16InFixKTrunc_m

- Numerator of the filter coefficient

- Initialized value of filter output

- LPF_SvUpdate_s16InFixKTrunc_m

- Calculated value of filt_SV

- LPF_OpUpdate_s16InFixKTrunc_m

- calculated value of filter state variable

- <Lvalue> = filt_O >> Kd

- where Kd is pre-defined for a 16 bit filter coefficient = 16

- LPF_SvInit_s16InFixKTrunc_m (<Input>)

- LPF_OpInit_s16InFixKTrunc_m (<Input>, <Filt_SV>, <Kn>)

- s _Per() sub module execute the following macros in the given sequence

- LPF_SvUpdate_s16InFixKTrunc_m (<Input>, <filt_SV>, <Kn>)

- LPF_OpUpdate_s16InFixKTrunc_m ( <filt_SV>)

- The filter topology 1LP1-B is as given,

- filt_SV = Input * G * Kd * D

- filt_O = [( ( (Input * G * D)

- (filt_SV / Kd) ) * Kn ) + filt_SV] / (Kd * D)

- filt_SV = ( ( (Input * G * D)

- filt_O = filt_SV / (Kd * D)

- The multiplication for the Filter Input by G shall be implemented external to the library macros. Thus the Input as used by the macros shall represent actual filter input * G, for non unity gain filter implementation.

- Note: Constraint on this filter is that Node b cannot exceed 16 bits.

- LPF_SvInit_u16InVarKTrunc_m

- Denominator bits of filter coefficient

- Deadband factor

- Initialized value of Node e

- Lvalue = (Input << Kd) << D

- Note:- The multiplication by D shall not be performed for D = 0.

- LPF_OpInit_u16InVarKTrunc_m

- Initialized value of state variable

- Numerator of coefficient

- Low pass filter output

- Lvalue = [((((Input<<D)

- (Filt_SV >> Kd)) * Kn ) + Filt_SV)>>Kd]>>D

- Note:- The multiplication and division by D shall not be performed for D = 0.

- LPF_SvUpdate_u16InVarKTrunc_m

- Calculated value of filter state variable

- <Lvalue> = ( ( (Input << D)

- LPF_OpUpdate_u16InVarKTrunc_m

- <Lvalue> = (filt_SV >> Kd ) >>D

- Note:- The division by D shall not be performed for D = 0.

- LPF_SvInit_u16InVarKTrunc_m (<Input>, <Kd>, <D>)

- LPF_OpInit_u16InVarKTrunc_m (<Input>, <Filt_SV>, <Kn>, <Kd>, <D>)

- LPF_SvUpdate_u16InVarKTrunc_m (<Input>, <filt_SV>, <Kn>, <Kd>, <D>)

- LPF_OpUpdate_u16InVarKTrunc_m ( <filt_SV>, <Kd>, <D>)

- LPF_SvInit_s16InVarKTrunc_m

- LPF_OpInit_s16InVarKTrunc_m

- Initialized value of filter state variable

- Numerator of filter coefficient

- (Filt_SV >> Kd)) * Kn ), + Filt_SV)>>Kd]>>D

- LPF_SvUpdate_s16InVarKTrunc_m

- Calculated value of filt_SV as given below

- LPF_OpUpdate_s16InVarKTrunc_m

- LPF_SvInit_s16InVarKTrunc_m (<Input>, <Kd>, <D>)

- LPF_OpInit_s16InVarKTrunc_m (<Input>, <Filt_SV>, <Kn>, <Kd>, <D>)

- LPF_SvUpdate_s16InVarKTrunc_m (<Input>, <filt_SV>, <Kn>, <Kd>, <D>)

- LPF_OpUpdate_s16InVarKTrunc_m ( <filt_SV>, <Kd>, <D>)

- The filter topology 1LP1-CF is as given,

- The equation to calculate the filter coefficient K is as follows: (Where Fp is

- me as that defined in the initialization function above.

- filt_Out = ( ( Input

- prev_SV ) * K ) + prev_SV

- The value of filt_SV is the value of filt_Out from the previous call to the above function.

- There will be three macros defined for this implementation:- state variable and coefficient initialization, coefficient calculation, and filter output update.

- Coefficient and State Variable Initialization Macro

- LPF_Init_f32_m

- Initial input to filter

- Pole cutoff frequency in hertz

- Sampling interval in seconds

- REF _Ref323022249 \r

- Initial output, node O

- <SV_Str-> SV_Uls_f32> = Input

- <Lvalue> = Input

- LPF_KUpdate_f32_m(Fp, T, SV_Str)

- Coefficient Recalculation Macro

- LPF_KUpdate_f32_m

- New value of K stored in state variable structure

- <SV_Str-> K_Uls_f32>

- Output of low pass filter

- <Lvalue> = <SV_Str->SV_Uls_f32> =

- <SV_Str->SV_Uls_f32>) * <SV_Str->K_Uls_f32> + <SV_Str->SV_Uls_f32>

- Usable ranges for LPF32KSV_Str Structure

- For a module that executes a LPF, in its _Init() sub module execute the following macros:

- LPF_Init_f32_m(<Input>, <Fp>, <T>, <LPF32KSV_Str>)

- s _Per() sub module execute the following macro:

- LPF_OpUpdate_f32_m ( <Input>, <LPF32KSV_Str>)

- The module may optionally call the following macro if the coefficient value K needs to be updated on the fly to support variable cutoff filtering.

- LPF_KUpdate_f32_m(<Fp>, <T>, <LPF32KSV_Str>)

- The filter topology HP-CF is as given:

- EMBED Visio.Drawing.11

- Low Pass Filter

- The low-pass filter aspect of the design uses the 1LP1-CF implementation as described in section

- REF _Ref323206819 \r \h

- CF Calculation

- The CF (correction factor) is calculated as follows:

- CF = (1 + exp(2PI * Fp * T)) / (2 * sqrt(1 + ((2 * Fp * T)^2)))

- The equation for the output is as follows:

- filt_Out = ( Input

- LPF_Output ) * CF

- Library Routine Design

- There will be three macros defined for this implementation: state variable and coefficient initialization, coefficient calculation, and filter output update. The interface for these macros will be similar to that of the 1LP1-CF low pass filter design.

- HPF_Init_f32_m

- HPF32KSV_Str

- REF _Ref323022551 \r

- Assignment returns initial output

- LPF_Init_f32_m(Input, Fp, T, &(SV_Ptr->LPF_Str))

- HPF_KUpdate_f32_m(Fp, T, SV_Ptr)

- HPF_KUpdate_f32_m

- Assignment returns correction factor

- SV_Ptr->CF = (1 + exp(2PI * Fp * T)) / (2 * sqrt(1 + ((2 * Fp * T)^2)))

- LPF_KUpdate_f32_m(Fp_f32, T_f32, &(SV_Ptr->LPF_Str))

- HPF_OpUpdate_f32_m

- Assignment returns filter output

- (Input - LPF_OpUpdate_f32_m(input_f32, &(SV_Ptr->LPF_Str))) * SV_Ptr->CF_Uls_f32

- Usable ranges for HPF32KSV_Str Structure

- For a module that executes a HPF, in its _Init() sub module execute the following macros:

- HPF_Init_f32_m(<Input>, <Fp>, <T>, <HPF32KSV_Str>)

- HPF_OpUpdate_f32_m ( <Input>, <HPF32KSV_Str>)

- The module may optionally call the following macro if the coefficient value K needs to be updated on the fly to support variable cutoff filtering:

- HPF_KUpdate_f32_m(<Fp>, <T>, <HPF32KSV_Str>)

- Added floating point low-pass filter

- Jared Julien

- Added floating point high-pass filter, fixed issues in FP LPF

- Correct output types for some filters (32 bits output instead of 16bits)

- no code change

- Added new parameter to functions NF_FullUpdate_f32 and NF_SvUpdate_f32

- NEXT GENERATION SOFTWARE DESIGN

- SOFTWARE LIBRARY DESIGN SPECIFICATION

- Filter Library

- SAVEDATE \@ "d-MMM-yy" \* MERGEFORMAT

- LASTSAVEDBY \* MERGEFORMAT

- Owen Tosh (nzx5jd)

- NEXTEER CONFIDENTIAL
