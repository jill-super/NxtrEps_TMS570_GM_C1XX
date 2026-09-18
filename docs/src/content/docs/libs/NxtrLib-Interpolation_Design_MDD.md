---
title: "NxtrLib — Interpolation_Design_MDD"
description: "Converted .doc document from NxtrLib/doc."
---

> **Conversion note:** this is a legacy binary `.doc` file. No high-fidelity converter was available in this environment, so the text below was recovered heuristically from the OLE `WordDocument` stream. Ordering, tables and images may be incomplete. For normative content, consult the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/NxtrLib/doc/Interpolation_Design_MDD.doc`.

- x = fixed X interval within which the input lies.

- y = interpolated output

- Determine the value of n, i.e the index into the table, n = truncate ( x /

- x ). Using this index n, determine the values of xn, yn and yn+1. The output y can then be ca

- TOC \o "1-3" \h \z

- HYPERLINK \l "_Toc336607717"

- Variable X Variable Y 2D Table Lookup function (with interpolation)

- PAGEREF _Toc336607717 \h

- HYPERLINK \l "_Toc336607718"

- PAGEREF _Toc336607718 \h

- HYPERLINK \l "_Toc336607719"

- Implementation:

- PAGEREF _Toc336607719 \h

- HYPERLINK \l "_Toc336607720"

- Unsigned X, Unsigned Y

- PAGEREF _Toc336607720 \h

- HYPERLINK \l "_Toc336607721"

- Signed X, Unsigned Y

- PAGEREF _Toc336607721 \h

- HYPERLINK \l "_Toc336607722"

- Signed X, Signed Y

- PAGEREF _Toc336607722 \h

- HYPERLINK \l "_Toc336607723"

- Unsigned X, Signed Y

- PAGEREF _Toc336607723 \h

- HYPERLINK \l "_Toc336607724"

- Fixed X Variable Y 2D Table Lookup function (with interpolation)

- PAGEREF _Toc336607724 \h

- HYPERLINK \l "_Toc336607725"

- PAGEREF _Toc336607725 \h

- HYPERLINK \l "_Toc336607726"

- PAGEREF _Toc336607726 \h

- HYPERLINK \l "_Toc336607727"

- PAGEREF _Toc336607727 \h

- HYPERLINK \l "_Toc336607728"

- PAGEREF _Toc336607728 \h

- HYPERLINK \l "_Toc336607729"

- PAGEREF _Toc336607729 \h

- HYPERLINK \l "_Toc336607730"

- PAGEREF _Toc336607730 \h

- HYPERLINK \l "_Toc336607731"

- Single X Multiple Y (Bilinear Interpolation)

- PAGEREF _Toc336607731 \h

- HYPERLINK \l "_Toc336607732"

- PAGEREF _Toc336607732 \h

- HYPERLINK \l "_Toc336607733"

- Syntax: BilinearXYM_s16_u16Xs16YM_Cnt (BS, input, *BSTbl, BSize, *XTbl, *YMTbl, Xsize)

- PAGEREF _Toc336607733 \h

- HYPERLINK \l "_Toc336607735"

- Syntax: BilinearXYM_u16_u16Xu16YM_Cnt(BS, input, *BSTbl, BSsize, *XTbl, *YMTbl, Xsize)

- PAGEREF _Toc336607735 \h

- HYPERLINK \l "_Toc336607736"

- Syntax: BilinearXYM_s16_s16Xs16YM_Cnt (BS, input, *BSTbl, BSize, *XTbl, *YMTbl, Xsize)

- PAGEREF _Toc336607736 \h

- HYPERLINK \l "_Toc336607737"

- Syntax: BilinearXYM_u16_s16Xu16YM_Cnt(BS, input, *BSTbl, BSsize, *XTbl, *YMTbl, Xsize)

- PAGEREF _Toc336607737 \h

- HYPERLINK \l "_Toc336607738"

- Multiple X Multiple Y (Bilinear Interpolation)

- PAGEREF _Toc336607738 \h

- HYPERLINK \l "_Toc336607739"

- Implementation

- PAGEREF _Toc336607739 \h

- HYPERLINK \l "_Toc336607740"

- Syntax: BilinearXMYM_u16_u16XMu16YM_Cnt( BS, input, *BSTbl, BSsize, *XMTbl, *YMTbl, Xsize)

- PAGEREF _Toc336607740 \h

- HYPERLINK \l "_Toc336607741"

- Syntax: BilinearXMYM_s16_u16XMs16YM_Cnt(BS, input, *BSTbl, BSsize, *XMTbl, *YMTbl, Xsize)

- PAGEREF _Toc336607741 \h

- HYPERLINK \l "_Toc336607742"

- Syntax: BilinearXMYM_u16_s16XMu16YM_Cnt( BS, input, *BSTbl, BSsize, *XMTbl, *YMTbl, Xsize)

- PAGEREF _Toc336607742 \h

- HYPERLINK \l "_Toc336607743"

- UnitTesting Range: Linear and Bilinear Interpolation

- PAGEREF _Toc336607743 \h

- HYPERLINK \l "_Toc336607744"

- Revision Control Log

- PAGEREF _Toc336607744 \h

- The Variable X Variable Y 2D table has the Variable X as the input (independent variable) and the Variable Y as the output (dependent variable). The lookup function with interpolation is used to interpolate the values of Y corresponding to the input value for X. This is implemented using the straight-line equation as given below:

- EMBED Equation.3

- n = index into the independent and dependent variable tables

- n+1 = next consecutive index into the tables.

- (yn+1 - yn) = interval in the dependent table within which the interpolated output is calculated.

- (xn+1 - xn) = interval in the independent table within which the input lies.

- y = interpolated output (dependent variable)

- x = input (independent variable)

- Note that yn+1 < yn or yn+1 > yn, for negative or positive slopes and xn+1 > xn.

- The index n and n+1, are determined using Straight-Forward Search method. Using the indices, the values of xn+1, xn, yn+1 and yn are determined.

- The difference (yn+1 - yn) is held in a signed variable to ensure that the interpolation can handle both positive and negative slopes.

- The Variable X VariableY interpolation function is defined as a function with the input x value and table name passed as parameters. The function will return the interpolated output y as its output.

- Note: Straight Forward Search method is used for calculating the index n.

- Syntax : IntplVarXY_u16_u16Xu16Y_Cnt ( *TableX, *TableY, Size, input)

- TableX: - The Variable X 2D table (independent table)

- TableY: - The Variable Y 2D table (dependent table)

- Size: - Size of the table

- input: - The input to the table

- output: The output from the table.

- Pseudo Code :

- input, output, Size

- diffY, diffX, diffXinput, tmpout2, sOutput

- diffY, diffX, diffXinput, tmpout1

- const UINT16

- TableX = [ x1, x2, x3, x4, x5,

- TableY = [ y1, y2, y3, y4, y5,

- /* Check for Range */

- if ( input <= TableX[0] )

- return TableY[0]

- else if ( input >= TableX[size-1] )

- return TableY[size-1]

- /* In range. Get Index */

- while ( TableX[index + 1] < input )

- index = index + 1

- /* Interpolate and get the output */

- diffY = TableY[index+1] - TableY[index]

- diffX = TableX[index+1] - TableX[index]

- diffXinput = input - TableX[index]

- /* Product in 32 bit */

- tmpout1 = diffY* diffXinput

- /* Check if Divide by zero */

- if (diffX == 0)

- /* Here, the lower 16 bits are assigned to tmpout2 */

- tmpout2 = tmpout1 / diffX

- output = tmpout2 + TableY[index]

- return output

- Syntax : IntplVarXY_u16_s16Xu16Y_Cnt (*TableX, *TableY, Size, input)

- output, Size

- const SINT16

- tmpout1 = diffY * diffXinput

- Syntax : IntplVarXY_s16_s16Xs16Y_Cnt (*TableX, *TableY, Size, input)

- input, output

- diffY, diffX, diffXinput, tmpout2

- Syntax : IntplVarXY_s16_u16Xs16Y_Cnt (*TableX, *TableY, Size, input)

- The Fixed X Variable Y 2D table has the Fixed X as the input (independent variable) and the Variable Y (dependent variable) as the output. The interpolation function is used to interpolate the values of Y corresponding to the input value for X. It is assumed that the independent axis (X) will always start from 0. This is implemented using the straight-line equation as given below:

- n = index into the Table

- lculated based on the straight line given above.

- Syntax : IntplFxdX_u16_u16Xu16Y_Cnt (DeltaX, *TableY, Size, input)

- DeltaX: - The Fixed X interval

- diffY, diffXinput, tmpout2, sOutput

- diffY, diffXinput, tmpout1

- if (DeltaX == 0)

- /* Cannot do interpolation. Return Y0 */

- if ( input <= 0 )

- else if ( input >= DeltaX * (size-1) )

- index = truncate (input / DeltaX)

- diffXinput = input - DeltaX * index

- tmpout2 = tmpout1 / DeltaX

- Syntax : IntplFxdX_u16_s16Xu16Y_Cnt (DeltaX, *TableY, Size, input)

- diffY, diffXinput , tmpout1

- Syntax: IntplFxdX_s16_s16Xs16Y_Cnt (DeltaX, *TableY, Size, input)

- diffY, diffXinput, tmpout2

- Syntax: IntplFxdX_s16_u16Xs16Y_Cnt (DeltaX, *TableY, Size, input)

- BS:- Bilinear Selector

- Input:-The input to the table

- BSTbl:- Bilinear Selector Table 2D

- BSize:- Bilinear Selector Table Size

- XTbl:- Table X 2D

- YMTbl:- Table Y with MxN dimension

- Xsize:- Size of XTbl

- Output:- The output from the table

- Pseudo Code:

- BSindex, Xindex

- ArrayIndex1, ArrayIndex2, ArrayIndex3, ArrayIndex4

- BSinputDiff, XInputDiff

- Numerator_f32, Denominator_f32, Output_f32

- Const UINT16 BSTbl = [z1,z2,z3,z4,

- Const UINT16 XTbl = [x1,x2,x3,x4,

- Const SINT16 YMTbl[mxn] = [(y1,y2,y3

- If (BS <= BSTbl[0])

- BS = BSTbl[0]

- Else if (BS >= BSTbl[BSize-1])

- BSindex = BSsize -2

- BS = BSTbl[BSsize -1]

- While ((BSTbl[BSindex] = = BSTbl[BSindex + 1] && (BSindex > 0)))

- BSindex = BSindex - 1

- While ( BSTbl[BSindex +1] < BS)

- BSindex = BSindex + 1

- If (input <= XTbl[0])

- Input = XTbl[0]

- Else if (input >= XTbl[XSize

- Xindex = Xsize

- Input = XTbl[Xsize -1]

- While ( XTbl[Xindex +1] < input)

- Xindex = Xindex+1

- ArrayIndex1 = (BSindex * Xsize) + Xindex

- ArrayIndex2 = (BSindex * Xsize) + Xindex + 1

- ArrayIndex3 = ((BSindex + 1) * Xsize) + Xindex

- ArrayIndex4 = ((BSindex + 1) * Xsize) + Xindex + 1

- BSInputDiff = BS

- BSTbl[BSindex]

- XInputDiff = input

- XTbl[Xindex]

- Numerator_f32 = ( YMTbl[ArrayIndex2]

- YMTbl[ArrayIndex1]) * ((BSTbl[BSindex+1]

- BSTbl[BSindex]) * XInputDiff) +

- (YMTbl[ArrayIndex3]

- YMTbl[ArrayIndex1]) *

- (BSInputDiff * (XTbl[Xindex+1]

- XTbl[Xindex])) +

- (XInputDiff * BSInputDiff ) *

- ((YMTbl[ArrayIndex4])

- (YMTbl[ArrayIndex3])

- (YMTbl[ArrayIndex2]

- YMTbl[ArrayIndex1]))

- Denominator_f32 = (BSTbl[BSindex +1]

- BSTbl[BSindex]) * (XTbl[Xindex+1]

- XTbl[Xindex])

- If (Denominator_f32 <= FLT_EPSILON)

- Output_f32 = YMTbl[ArrayIndex1]

- Output_f32 = YMTbl[ArrayIndex1] + Numerator_f32 / Denominator_f32

- If (Output_f32 >= 0)

- Output_f32 = Output_f32 + 0.5

- Output_f32 =Output_f32

- /*Float to SINT16 typecast*/

- Output_s16 = Output_f32

- return Output_s16

- input:-The input to the table

- BSInputDiff, XInputDiff

- Numerator_f32, Denominator_f32

- Const UINT16 YMTbl[mxn] = [(y1,y2,y3

- Else if (BS >= BSTbl[BSsize

- BS = BSTbl [ BSsize

- While (( BSTbl [BSindex] == BSTbl [ BSindex+1] && (BSindex > 0)))

- BSindex = BSindex

- While (BSTbl[BSindex +1]<BS)

- BSindex = BSindex +1

- Else if (input >= XTbl[XSize -1])

- Xindex = Xsize -2

- input = XTbl[Xsize -1]

- While ( XTbl[Xindex + 1] < input)

- Xindex= Xindex + 1

- ArrayIndex3 = ((BSindex + 1)* Xsize) + Xindex

- ArrayIndex4 = ((BSindex + 1)* Xsize) + Xindex + 1

- ((BSTbl [ BSindex + 1]

- (YMTbl [ ArrayIndex3]

- (XInputDiff * BSInputDiff) *

- Denominator_f32 = (BSTbl[BSindex+1]

- Output_u16 = YMTbl[ArrayIndex1] + 0.5

- Output_u16 = YMTbl[ArrayIndex1] + (Numerator_f32 / Denominator_f32) + 0.5

- return Output_u16

- XTbl:- Table X with [MxN] dimension

- YMTbl:- Table Y with [MxN] dimension

- UINT16 BSindex, X1index, X2index,

- UINT16 ArrayIndex1, ArrayIndex2, ArrayIndex3, ArrayIndex4

- SINT32 BSInputDiff, XInputDiff1, XInputDiff2

- SINT32 Mult1_s32, Mult2_s32

- FLOAT32 Numerator_f32, Denominator_f32

- UINT16 Output_u16

- SINT32 Den1_s32, Den2_s32, Den3_s32

- UINT16 input2 = input

- Const UINT16 XTbl[mxn] = [(x1,x2,x3

- If ( BS <= BSTbl[0] )

- BS = BSTbl [0]

- Else if (BS >= BSTbl[BSsize -1])

- BSindex = BSsize

- BS = BSTbl [ BSsize-1]

- while (BSTbl[BSindex] == BSTbl[BSindex+1] && (BSindex > 0))

- BSindex = BSindex -1

- while ( BSTbl [ BSindex +1] < BS)

- If ( input <= XMTbl [ BSindex * Xsize])

- Input = XMTbl [BSindex * Xsize]

- Else if (input >= XMTbl [ (BSindex * Xsize) + Xsize -1])

- X1index = Xsize

- input = XMTbl [ (BSindex * Xsize) + Xsize

- while ((XMTbl[(BSindex * Xsize)+X1index] == XMTbl[(BSindex * Xsize) + X1index +1]) && (X1index >0))

- X1index = X1index

- while (XMTbl[(BSindex * Xsize)+X1index+1] <input)

- X1index = X1index + 1

- If (input2 <= XMTb1 [(BSindex+1) * Xsize])

- input2 = XMTbl[(BSindex + 1) * Xsize ]

- Else if (input2 >= XMTbl [ ((BSindex +1) * Xsize) + Xsize -1])

- X2index = Xsize -2

- input2 = XMTbl[((BSindex +1)*Xsize) + Xsize -1]

- while ((XMTbl[((BSindex+1)*Xsize)+X2index]==XMTbl[((BSindex+1)*Xsize)+X2index+1]) && (X2index >0))

- X2index = X2index

- while ( XMTbl[((BSindex+1)*Xsize)+X2index+1]<input2)

- X2index = X2index +1

- ArrayIndex1 = (BSindex * Xsize) + X1index

- ArrayIndex2 = (BSindex * Xsize) + X1index + 1

- ArrayIndex3 = ((BSindex +1)* Xsize) + X2index

- ArrayIndex4 = ((BSindex +1)*Xsize)+X2index+1

- XInputDiff1 = input

- XMTbl[ArrayIndex1]

- XInputDiff2 = input2

- XMTbl[ArrayIndex3]

- Mult1_s32 = XInputDiff1 * (XMTbl[ArrayIndex4]

- XMTbl[ArrayIndex3])

- Mult2_s32 = BSInputDiff * (XMTbl[ArrayIndex2]

- XMTbl[ArrayIndex1])

- Den1_s32 = (XMTbl[ArrayIndex4]-XMTbl[ArrayIndex3])

- Den2_s32 = (XMTbl[ArrayIndex2]

- Den3_s32 = (BSTbl[BSindex +1]-BSTbl[BSindex])

- Numerator_f32 = Mult1_s32 * (BSTbl[BSindex+1]-BS) *

- (YMTbl[ArrayIndex2]-YMTbl[ArrayIndex1]) +

- Mult2_s32*(XMTbl[ArrayIndex4]

- XMTbl[ArrayIndex3]) *

- YMTbl[ArrayIndex1]) +

- Mult2_s32 * XInputDiff2*(YMTbl[ArrayIndex4]

- YMTbl[ArrayIndex3])

- Denominator_f32 = (Den1_s32 * Den2_s32) * Den3_s32

- UINT16 BSindex, X1index, X2index

- SINT16 Output_s16

- FLOAT32 Output_f32

- If ( BS <= BSTbl[0])

- While ( BSTbl[BSindex] == BSTbl[BSindex + 1] && (BSindex >0))

- While (BSTbl[BSindex +1] < BS)

- If (input <= XMTbl[BSindex * Xsize ] )

- input = XMTbl[BSindex * Xsize]

- else if (input >= XMTbl[(BSindex * Xsize) + Xsize -1])

- X1index = Xsize -2

- input = XMTbl[(BSindex * Xsize) + Xsize -1]

- while (( XMTbl[(BSindex * Xsize) + X1index] == XMTbl[(BSindex * Xsize) +X1index+1]) && (X1index > 0))

- X1index =X1index

- While (XMTbl[(BSindex * Xsize)+X1index+1] < input)

- X1index = X1index +1

- If (input2 <= XMTbl[(BSindex+1) * Xsize])

- Input2 = XMTbl[(BSindex+1)* Xsize]

- Else if (input2 >= XMTbl[(BSindex+1) * Xsize) + XSize-1])

- X2index = Xsize

- input2 = XMTbl[((BSindex +1)*Xsize)+Xsize

- while ((XMTbl[((BSindex+1)*Xsize)+X2index] == XMTbl[((BSindex+1) * Xsize)+X2index+1]) && (X2index >0))

- While (XMTbl[((Bsindex+1)* Xsize) + X2index +1] < input2)

- X2index= X2index+1

- ArrayIndex3 = ((BSindex+1)*Xsize)+X2index

- ArrayIndex4 = ((BSindex + 1)*Xsize) + X2index+1

- Mult2_s32 = BSinputDiff * (XMTbl[ArrayIndex2]

- Den1_s32 = (XMTbl[ArrayIndex4] - XMTbl[ArrayIndex3])

- Den3_s32 = (BSTbl[BSindex+1]

- BSTbl[BSindex])

- Numerator_f32 = Mult1_s32 * ((BSTbl[BSindex+1]-BS) * (YMTbl[ArrayIndex2]

- Mult2_s32 * (XMTbl[ArrayIndex4]-XMTbl[ArrayIndex3])*

- YMTbl[ArrayIndex3]

- Mult2_s32*XInputDiff2*(YMTbl[ArrayIndex4]-YMTbl[ArrayIndex3])

- Output_f32 = YMTbl[ArrayIndex1]+Numerator_f32/Denominator_f32

- Output_f32 = Output_f32 +0.5

- Output_f32 = Output_f32 -0.5

- /*float to SINT16 typecasting*/

- 4.1.3 Syntax: BilinearXMYM_s16_s16XMs16YM_Cnt(BS, input, *BSTbl, BSsize, *XMTbl, *YMTbl, Xsize)

- BSindex, X1index, X2index

- BSInputDiff, XInputDiff1,

- Mult1_s32, Mult2_s32

- Den1_s32, Den2_s32, Den3_s32

- input2 = input

- Const SINT16 XTbl[mxn] = [(x1,x2,x3

- Else if (BS >= BSTbl[BSsize-1]

- BS = BSTbl[BSsize

- While ( BSTbl[BSindex] == BSTbl[BSindex+1] && (BSindex >0))

- While (BSTbl[BSindex+1] < BS)

- If (input <= XMTbl[BSindex * Xsize])

- else if (input >= XMTbl[(BSindex * Xsize) + Xsize

- X1index = Xsize-2

- input = XMTbl[(BSindex*Xsize)+Xsize-1]

- while ((XMTbl[(BSindex*Xsize)+X1index] = = XMTbl[(BSindex * Xsize)+X1index+1]) && (X1index > 0))

- X1index = X1index-1

- While ( XMTbl[(BSindex * Xsize) + X1index+1] < input)

- X1index = X1index+1

- If (input2 <= XMTbl[(BSindex+1)*Xsize])

- input2= XMTbl[(BSindex+1)*Xsize]

- else if (input2 >= XMTbl[((BSindex+1)*Xsize)+Xsize-1])

- X2index = Xsize-2

- input2 = XMTbl[((BSindex+1)*Xsize)+Xsize-1]

- while (( XMTbl[(BSindex+1)*Xsize) + X2index] == XMTbl[((BSindex+1)*Xsize)+X2index+1]) && (X2index > 0))

- X2index = X2index-1

- While ( XMTbl[((BSindex+1)*Xsize)+X2index+1] < input2)

- X2index = X2index+1

- ArrayIndex3 = ((BSindex +1)*Xsize)+X2index

- ArrayIndex4 = ((BSindex + 1)*Xsize)+X2index+1

- XInputDiff2 = inpu2

- Den1_s32 = (XMTbl[ArrayIndex4]

- Den3_s32 = (BSTbl[BSindex + 1]

- Numerator_f32 = Mult1_s32 * ((BSTbl[BSindex+1]-BS)* (YMTbl[ArrayIndex2]-YMTbl[ArrayIndex1])+

- Mult2_s32 * (XMTbl[ArrayIndex4]-XMTbl[ArrayIndex3]) *

- Mult2_s32 * XInputDiff2 * (YMTbl[ArrayIndex4]

- Output_f32 = Output_f32

- /*float to SINT16 typecast*/

- For unit testing consider Ranges as FULL based on the data type of the tables and Input. Note a limitation for all interpolation functions is that the X tables and the BS Tables are assumed to be always increasing in value (or equal). The tables should never be decreasing in values as the index increases.

- Change Description

- Author Initials

- Interpolation MDD

- Added remaining bilinear interpolation functions

- Changed divide by zero logic in bilinear interpolation to prevent floating point exceptions

- Updated pseudo code for the corrections for anomalies EA3#530 and EA3#191

- NEXT GENERATION SOFTWARE DESIGN

- MODULE DESIGN SPECIFICATION

- Table Interpolation Library Function

- Owen Tosh (nzx5jd)

- DELPHI CONFIDENTIAL
