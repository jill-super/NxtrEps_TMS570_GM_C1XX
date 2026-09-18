---
title: "Integration — HexView/ReferenceManual_HexView"
description: "Converted document ReferenceManual_HexView.pdf."
---

> **Converted document.** Source: `GM_C1XX_EPS_TMS570/Tools/HexView/ReferenceManual_HexView.pdf`.

## Page 1

### HexView

### Reference Manual

Version 1.6

Authors: Armin Happel

Version: 1.6

Status: in preparation (in preparation/completed/inspected/released)



## Page 2

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

2/  7 9

1 Document Information

1.1 History

### Author Date Version Remarks

Hp 2006-02-21 1.0 Creation

Hp 2006-07-14 1.1 Description of new features for V1.2.0

Main features are:

• Support for Ford-VBF and Ford-IHex in dialogs

• Compare-Feature

• Auto-detect file format on file open/save

Hp 2006-09-27 1.2 Description of new features for V1.3.0

• Merge and compare uses now the auto-filetype

detection

• Merge operation available from commandline

• Address calculation from banked to linear addresses

from commandline

• Checksum calculation feature from commandline

places results into file or data.

Hp 2006-12-07 1.3 Description of new features for V1.4.0

• Commandline: Checksum operates on selected

section. Multiple checksum areas can be specified

from the commandline.

• Postbuild operation added

• Fixing Ford IHex configuration problem for

flashindicator and File-Browse in the dialog

• Option /CR (cut-section) added to the commandline

• Delete and  Cut&paste with internal clipboard added.

• Description of the commandline processing order

added to the document

• Program returns a value depending on the status of

operation

• New option combination /XG with /MPFH to re-

position existing NOAM to adjusted NOAR-fields

• Goto start of a block (double-click to block descriptor)

• Find ASCII string in data was added

Hp 2007-07-09 1.31 Description of new features for V1.4.6

• Support part number in GM-f iles (option /pn) from the

commandline and reading the file

Hp 2007-09-19 1.4 Description of new features for V1.5

• Start CANflash from within Hexview

• Create partial datafiles for Fiat-export

• Support VBF V2.4 for Ford

• Support Align Erase (/AE)

• Use ranges instead of start and end address

• Creation of a va lidation structure

• New About-dialog with personalized license info

Hp 2008-01-31 1.5 Fixing wrong description of checksum calculation

for method 8 (see Table 4-3, index 8)

Hp 2009-05-19 1.6 Description of new features for V1.6

• Fixing problem when HEX-file contain addresses until

0xFFFF.FFFF

• Extend expdatproc interface to allow insertion of data



## Page 3

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

3/  7 9

processing results into HEX-file

• Now browse for data processing parameter file

• Intel-HEX record length now adjustable

• This document can now be opened from Help menu

• Allow to select multiple post build files

• Generate structured hex file from Eeprom data set

• C-array generation supports structured list, Ansi-C

and memmap.

Table 1-1  History of the Document



## Page 4

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

4/  7 9

1.2 Reference Documents

### Index Document

[1] Fiat-Specification 07284-01, dated 2003-05-15

[2] Ford: Versatile Binary Format V2.2

[3] Ford: Module programming and Design specification, V2003.0

[4] GM: GMW3110, V1.5, chapter 11

Table 1-2  Reference Documents

### Please note

### We have configured the programs in accordance with your specifications in the

questionnaire. Whereas the programs do support other configurations than the one

specified in your questionnaire, Vector´s release of the programs delivered to your

company is expressly restricted to the configuration you have specified in the

questionnaire..



## Page 5

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

5/  7 9

### Contents

1.1 History .......................................................................................................... 2

1.2 Reference Documents ................................................................................. 4

2.1 Important notes .......................................................................................... 10

2.2 Terminology................................................................................................ 10

3.1 With a Double Click to the Main Menu ....................................................... 12

3.1.1 Edit a HEX data line ................................................................................... 12

3.1.2 Changing the base address of a data block............................................... 12

3.2 Menu .......................................................................................................... 13

3.2.1 Menu: “File” ................................................................................................13

3.2.1.1 New ..................................................................................................... 13

3.2.1.2 Open ................................................................................................... 13

3.2.1.2.1 Auto-file format analysing process ............................................... 13

3.2.1.3 Merge .................................................................................................. 14

3.2.1.4 Compare ............................................................................................. 14

3.2.1.5 Save .................................................................................................... 15

3.2.1.6 Save as ............................................................................................... 15

3.2.1.7 Log Commands................................................................................... 16

3.2.1.8 Import .................................................................................................. 16

3.2.1.8.1 Import Intel-Hex/Motorola S-Record............................................. 16

3.2.1.8.2 Read 16-Bit Intel Hex ................................................................... 16

3.2.1.8.3 Import binary data ........................................................................ 17

3.2.1.8.4 Import GM data ............................................................................ 17

3.2.1.8.5 Import Fiat data ............................................................................ 17

3.2.1.8.6 Import Ford IHex data .................................................................. 17

3.2.1.8.7 Import Ford VBF data................................................................... 17

3.2.1.9 Export.................................................................................................. 17

3.2.1.9.1 Export as S-Record...................................................................... 17

3.2.1.9.2 Export as Intel-HEX...................................................................... 18

3.2.1.9.3 Export as CCP Flashkernel.......................................................... 20

3.2.1.9.4 Export as C-Array......................................................................... 21

3.2.1.9.5 Export Mime coded data .............................................................. 24

3.2.1.9.6 Export Binary data........................................................................ 24

3.2.1.9.7 Export binary block data............................................................... 24

3.2.1.9.8 Export Fiat Binary File.................................................................. 24

3.2.1.9.9 Export Ford Ihex data container ...................................................25

3.2.1.9.10 Export Ford VBF data container................................................... 26

3.2.1.9.11 Export GM data ............................................................................ 27

3.2.1.9.12 Export GM-FBL header info ......................................................... 28

3.2.1.9.13 Export VAG data container........................................................... 29



## Page 6

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

6/  7 9

3.2.1.9.14 Print / Print Preview / Printer Setup.............................................. 32

3.2.1.9.15 Exit 32

3.2.2 Edit............................................................................................................. 32

3.2.2.1 Undo.................................................................................................... 32

3.2.2.2 Cut / Copy / Paste ............................................................................... 32

3.2.2.3 Data Alignment.................................................................................... 34

3.2.2.4 Fill block data ...................................................................................... 34

3.2.2.5 Create Checksum ............................................................................... 35

3.2.2.6 Run Data Processing .......................................................................... 36

3.2.2.7 Edit/Create OEM Container-Info ......................................................... 37

3.2.3 View ........................................................................................................... 38

3.2.3.1 Goto address… ................................................................................... 38

3.2.3.2 Find record .......................................................................................... 39

3.2.3.3 Repeat last find ................................................................................... 39

3.2.3.4 View OEM container info..................................................................... 39

3.2.4 Info operation (?)........................................................................................ 39

3.3 Accelerator Keys (short-cut keys) .............................................................. 41

4.1 Command line options summary................................................................ 42

4.2 General command line operation order...................................................... 46

4.2.1 Align Data (/ADxx or /AD:yy)...................................................................... 47

4.2.2 Align length (/AL)........................................................................................ 47

4.2.3 Specify fill character (/AF:xx)...................................................................... 48

4.2.4 Address range reduction (/AR:’range’).......................................................48

4.2.5 Cut out data from loaded file (/CR:’range1[:’range2’:…] ............................49

4.2.6 Checksum calculation method

(/CSx[:target[;limited_range][/no_range]) ................................................... 49

4.2.7 Run Data Processing interface

(/DPn:param[,section,key][;outfilename]) ................................................... 52

4.2.8 Create error log file (/E:errorfile.err) ........................................................... 54

4.2.9 Create single region file (/FA)..................................................................... 54

4.2.10 Fill region (/FR:’range1’:’range2’:…) ..........................................................54

4.2.11 Specify fill pattern (/FP:xxyyzz…)............................................................... 54

4.2.12 Execute logfile (/L:logfile) ........................................................................... 55

4.2.13 Merging files (/MO, /MT) ............................................................................ 55

4.2.14 Run postbuild operation (/pb=postbuild-file)............................................... 56

4.2.15 Specify output filename (-o outfilename).................................................... 58

4.2.16 Run in silent mode (/s) ............................................................................... 58

4.2.17 Specify an INI-file for additional parameters (/P:ini-file) ............................. 58

4.2.18 Remapping address information (/remap).................................................. 59

4.3 Output-control command line options (/Xx)................................................ 61

4.3.1 Output a Fiat specific data file (/XB)........................................................... 62



## Page 7

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

7/  7 9

4.3.2 Output data into C-Code array (/XC).......................................................... 63

4.3.3 Output a Ford specific data file (/XF, /XVBF).............................................. 64

4.3.3.1 Output Ford files in Intel-HEX format .................................................. 64

4.3.3.2 Output Ford files in VBF format........................................................... 67

4.3.4 Output a GM-specific data file.................................................................... 70

4.3.4.1 Manipulating Checksum and address/Length field within an

existing header (/XG) .......................................................................... 70

4.3.4.2 Creating the GM file header for the operation software

(/XGC[:address]) ................................................................................. 72

4.3.4.3 Creating the GM file header for the calibration software

(/XGCC[:address])............................................................................... 72

4.3.4.4 Creating the GM file header with 1-byte HFI

(/XGCS[:address])............................................................................... 73

4.3.4.5 Specify the SWMI data (/SWMI=xxxx) ................................................ 73

4.3.4.6 Specify the DLS values (/DLS=xx) ......................................................73

4.3.4.7 Specify the Module-ID parameter (/MODID=value)............................. 74

4.3.4.8 Specify the DCID-field (/DCID=value) .................................................74

4.3.4.9 Specify the MPFH field (/MPFH[=file1+file2+…] ................................. 74

4.3.5 Output a VAG specific data file (/XV) ......................................................... 75

4.3.6 Output data as Intel-HEX (/XI) ................................................................... 75

4.3.7 Output data as Motorola S-Record (/XS[:reclinelen])................................. 75

4.3.8 Outputs to a CCP/XCP kernel file (/XK) ..................................................... 75

5.1 Interface function for checksum calculation ............................................... 76

5.2 Interface function for data processing ........................................................ 77

5.3 Software licenses ....................................................................................... 78



## Page 8

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

8/  7 9

### Illustrations

Figure  3-1 Main Menu of HexView.................................................................................... 11

Figure  3-2 Edit-Line dialog ............................................................................................... 12

Figure  3-3 Change the base address of a segment......................................................... 12

Figure  3-4: Customizing merge data in the merge dialog ................................................. 14

Figure  3-5 Overlapping data when merging a file ............................................................ 14

Figure  3-6 Export data in the Motorola S-Record format ................................................. 18

Figure  3-7 Export dialog for the Intel-Hex output ............................................................. 18

Figure  3-8 Export flashkernel data for CCP/XCP............................................................. 20

Figure  3-9 Export data into a C-Array .............................................................................. 22

Figure  3-10: Export dialog for the FIAT binary file............................................................... 25

Figure  3-11: Export dialog for Ford I-Hex output file ........................................................... 26

Figure  3-12: Export dialog fort he Ford-VBF data file ormat ............................................... 27

Figure  3-13: The output information for the GM data export............................................... 27

Figure  3-14: Export dialog to generate the GM-FBL header information for GENy ............ 28

Figure  3-15 Exports data into a VAG-compatible data container .......................................29

Figure  3-16: Example of 'Copy window' when Ctrl-C or "Paste" pressed using start-

and end-address............................................................................................. 33

Figure  3-17: Example of cut-data using start-address and length as a parameter ............. 33

Figure  3-18: Pasting the clipboard data into the document specifying the target address.. 34

Figure  3-19 Data alignment option..................................................................................... 34

Figure  3-20 Dialog that allows to fill data ........................................................................... 35

Figure  3-21 Dialog to operate the checksum calculation ................................................... 36

Figure  3-22 Dialog for Data Processing ............................................................................. 36

Figure  3-23: Jump to a specific address in the display window .......................................... 39

Figure  3-24: Find a string or pattern within the document................................................... 39

Figure  4-2: Example on how to select the checksum calculation methods in the

"Create Checksum" operation ........................................................................ 49

Figure  4-3: Calling sequence of the post-build  functions ................................................. 56

Figure  4-4: Mapping pysical to linear address spaces ...................................................... 59

Figure  5-1 Build the list box entries for the GUI ............................................................... 76

Figure  5-2 Function calls when running checksum calculation ........................................ 77



## Page 9

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

9/  7 9

### Tables

Table 1-1  History of the Document ................................................................................... 3

Table 1-2  Reference Documents ...................................................................................... 4

Table  3-1: Auto-file format detection................................................................................ 13

Table  3-2: Currently available commands in the log-file .................................................. 16

Table  3-3: Description of the elements for the VAG SGML output container ...................31

Table  3-4: Accelerator keys (short-cut keys)  available in Hexview................................. 41

Table  4-1: Command line options summary .................................................................... 44

Table  4-2: Checksum location operators used in the commandline ................................ 50

Table  4-3: Functional overview of checksum calculation methods in “expdatproc.dll”.....52

Table  4-4: Functional overview of data processing methods in “expdatproc.dll” .............54

Table  4-5: INI-file information fort he Fiat file container generation ................................. 63

Table  4-6: INI-File definition fort he C-Code array export function .................................. 63

Table  4-7: INI-file description for Ford I-Hex file generation ............................................ 65

Table  4-8: INI-File description for Ford VBF export configuration.................................... 67

Table  4-9: Example of INI-files fort he Ford VBF export .................................................. 69



## Page 10

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

10 / 79

2 Introduction

This document describes the usage of the PC-T ool “HexView”. Originally a study of the

usage of the MFC library to display the contents of  Intel-HEX or Motorola S-Record files, it

has been enhanced to create data containers for some OEMs used for flash download.

Another purpose is to m anipulate this data or file contents to adapt it to the specific needs

for a flash download.

An open interface has been designed to allow data processing and checksum calculation.

Some of the features of He xview can be used by the graphica l user interface. But there

are also powerful features available via a command line interface. Some features are even

just accessible via the command lines.

Thanks to André Caspari for his Icon.

2.1 Important notes

### Caution

The application of this product can be dangerous. Please use it with care.

Note that this tool may be used to alter the program or data in tended to be downloaded

into an ECU for series production. The result s of this data manipulation must be observed

very carefully and thoroughly tested.

Vector Informatik GmbH is furnishing this item "as is" and free of charge. Vector Informatik

GmbH does not provide any warranty of the item whatsoever, whether express, implied, or

statutory, including, but not limited to, any warranty of merchantability or fitness for a

particular purpose or any warranty that the contents of the item will be error-free.

### In no respect shall Vector Informatik GmbH  incur any liability for any damages,

including, but limited to, direct, indirect, special, or consequential damages arising

out of, resulting from, or an y way connected to the use of  the item, whether or not

based upon warranty, contract, tort, or otherwise; whether or not injury was

sustained by persons or property or ot herwise; and whether or not loss was

sustained from, or arose out of, the results of, the item, or any services that may be

provided by Vector Informatik GmbH.

2.2 Terminology

### Item Description

 Address Region

###  PMA

 Section

 Block

 Segment

### Area of coherent data that can be described by a start address and

length of data.



## Page 11

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

11 / 79

3 User Interface

This chapter describes the user interface and menu items of the program.

To understand the user interface, some basics of file contents need to be clarified.

First, an Intel-HEX or Motorola S-Record cons ists of data assigned to specific addresses.

The data can be continuous from a specific start address. A continuous data block is

named as a section or segment. Such files can contain one or more data sections.

Figure 3-1 Main Menu of HexView

The figure above shows the main menu of HexVie w after a HEX-.File has been loaded. In

the upper part of the tool  the sections of the file are list ed. In the example above, the file

consists of 2 section2, named “Block 0..1”. For each block the start and end address is

given, as well as the length in hexadecimal and decimal value.

After the block section description, the data it self are displayed. Tw o adjacent blocks are

separated by a blank line (between 00000190 and 0009000).

A HEX-display line consists of the start address and its data. On the right side, the data is

partly interpreted as characters if possible (i f the data is lower 32, the character is shown

as a ‘.’).

Any mouse click with the left button restores the display in the window.

On the bottom of the window some status information is displayed.

From left to right:

• Information about the selected menu option

• Total number of bytes (decimal) of the currently loaded file (Size=Xxxxx)

• The file format of the data file t hat is currently loaded (see section 3.2.1.2.1 for

possible values).



## Page 12

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

12 / 79

3.1 With a Double Click to the Main Menu

To edit a hex-line, make a double click on the corresponding line you want to edit. This will

open the Edit-Line dialog.

3.1.1 Edit a HEX data line

You can edit the line in two different modes. In the upper line the data can be entered in

hexadecimal mode. In the lower line, the data can be entered as ASCII-characters. The left

field shows which base address the line is assigned to.

Figure 3-2 Edit-Line dialog

If only a few characters or hex values are en tered, HexView will onl y change these lines.

All others will remain.

3.1.2 Changing the base address of a data  block or jump to the block start

It is also possible to make a double click onto the block info which is on top of the main

menu. This opens the block shift address menu:

Figure 3-3 Change the base address of a segment

This dialog allows you to change the address of a block. Simply enter the new base

address.

You can also jump to the beginning of the spec ified block to display the data by selecting

the “Goto”-button (Note that it may also shift the address if another value in “New Address

will be specified).



## Page 13

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

13 / 79

It is also possible to delete the whole block from the list by pushing the button “Erase

entire block” button.

3.2 Menu

### The main menu is grouped into the categories

 File

 View

 Edit

 Flash

The file menu operates directly on complete files. The view menu allows searching for

options and the Edit menu can operate on the data.

Each of the elements of the menu will be described now.

3.2.1 Menu: “File”

3.2.1.1 New

### Closes the current file and restarts a new session

3.2.1.2 Open

This dialog allows to open a data file. Hexv iew analyses the data container and checks for

a known format. The resulting data format is displayed in the status line in the bottom area.

3.2.1.2.1 Auto-file fo rmat analysing process

The format analyse process uses the following method and order:

### File-format detection Scan process and order during file-read operation

 Fiat File Check the filename extension if it is a “.prm” - file, and try to read it as as a

Fiat parameter and BIN-File combination.

 GM binary files

### (GBF)

Check the filename extension if it is a “.gbf” - or “.bin” – file, and try to load

it in the GM-binary file format.

 Binary file, if no

### ASCII is found

### Read the first line with non-zero length and check if it contains non-ASCII

characters. If so, read the file as a binary block

 I-Hex if the line

begins with ‘:’

If the first 25 lines of the file corresponds to an ASCII string and starts with

a ‘:’, the data are read as Intel-HEX.

 S-Rec if the line

begins with ‘S’

If the ASCII-string starts with the character ‘S’ it  will be read as Motorola

### S-Record

 Ford VBF-File Check, if the contains the string “vbf_version”. Load it as VBF-file in that

case.

 Ford I-Hex Check if the file contains one of the Ford’s Intel-HEX header information

and read it as Ford-IHex file.

 Binary file in all other

cases

### In all other cases, read the file as a binary data input with the base

address of 0.

Table 3-1: Auto-file format detection



## Page 14

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

14 / 79

3.2.1.3 Merge

This item reads a file and adds the data to t he current document data. After selecting this

item, a file-select dialog will open. You can select any of the files in the format of the

autofile-type selections (see section 3.2.1.2.1). After selsecti ng the file and pressing OK,

the following dialog will appear:

Figure 3-4: Customizing merge data in the merge dialog

The specified range shows the area of data fr om the merge file. A smaller range can be

selected that shall be merged to  the current document. An offset  can be specified that will

be applied to each segment that will be merged. The offset can be positive or negative and

will be added or subtracted. Use a minus-sign to subtract the offset from the base address

of each segment.

If the data of the merged file overlaps with the file data, a warning will be displayed.

Figure 3-5 Overlapping data when merging a file

If “Overwriting existing data” is accepted, the newly read data will overwrite the data that is

internally present. If this is not accepted, the in ternal data is kept and just the surrounding

data is read into the internal memory.

All filetypes can be merged that  are also supported with the au tomatic filetype detection

method.

3.2.1.4 Compare

This item provides the means to compare the in ternal data against the data in an external

file. The compare option can load the same filetypes as supported with “File open”.



## Page 15

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

15 / 79

After selecting this item, a file select dial og will open. Select  the file that contains the data

you want to compare. Afterwards, the file compare dialog will be opened.

The left window displays the internal data, whereas the right window displays the data from

the external file. All differences are marked in colors. Data sections that are not present in

the internal or external document are marked with ‘-‘.

The green up- and down arrows  in the upper middle can be used to search for further

differences in the file. The next/previous sear ch procedure starts always from the first line

displayed in the window.

As mentioned above, the next/prev search algorithm starts from the top line of the window.

It uses the next/previous line and searches for the next equal data. If equal data found, it

searches for the next differen ce or non-presence of data. If  this is found, the first

appearance will be displayed on top of the window.

3.2.1.5 Save

After any modification of the data (e.g. modifying a hexline or the base address of a block),

the save option will be enabled. This indicate s, that the file has been modified. In that

case, the “Save” option enables you to store the data to the current file name. Hexview

writes the data in the current f ile format. The current file format is displayed in the status

line.

3.2.1.6 Save as

Enables you to store the inter nal data to a file with a different filename. Hexview uses the

current file format displayed in the status li ne. If a file format cannot  be stored (e.g. the

Intel-Hex/Motorola S-Record “Mixed” file type), a warning will be shown and no data can

be saved. Use the export function of Hexview to store the data in a different format.



## Page 16

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

16 / 79

3.2.1.7 Log Commands

This option is reserved for future use. It is  intended as a certain kind of macro recorder. If

selected, the “save as” dialog will open. Within it, a log file can be selected. HexView will

create a new file or delete the contents of an existing file. Once this has been selected,

some commands will be stored within it.

The following commands are implemented at the moment:

### Command name Command option Description

FileOpen filename Opens a file.

### FileClose - Close the file

### FileNew - Deletes the current file and

creates a new object

Table 3-2: Currently available commands in the log-file

This might be extended in the future.

The LOG-File commands can be executed through the command line options.

3.2.1.8 Import

The Import option allows to read  files in different other file formats. The following file

formats are supported:

 Motorola S-Record or Intel-Hex data

 Binary data

 GM data

 Fiat data

 Ford Intel-HEX data

 Ford VBF-Data

3.2.1.8.1 Import Intel-Hex/Motorola S-Record

This item is used to provide backward compatib ility to the File->Open function available in

previous versions of Hexview (V1.1.2 or lower). It scans a textfile and analyses each line if

it is an Intel-HEX or a Motorola S-Record line and reads the data.

The resulting file type will be displayed in the filetype-area of  the status line (‘S-Record’,

‘Intel-Hex’ or ‘Mixed’)

3.2.1.8.2 Read 16-Bit Intel Hex

This option reads an Intel-hex file and treat s the address and data as  16-bit values. Every

address information is multiplied by two. Then the data is read into the buffer.



## Page 17

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

17 / 79

3.2.1.8.3 Import binary data

Reads a data file content as a binary. The data is treated as  one binary block starting at

address 0. The base address can be changed by a double click to the block info line at the

top of the file.

3.2.1.8.4 Import HEX ASCII

This option provides the ability to read te xt information in HEX ASCII format. Every byte

will be represented as a pair or  single HEX characters, e.g. 34, 5, F3. All non-HEX-ASCII

characters like spaces or carriage returns will be dropped and treated as separators.

The base address of the read operation will be address 0.

3.2.1.8.5 Import GM data

Reads a binary file that contains the GM header information. Since the header should

contain address and length information, all sections can be restored from the file. Note that

this option can only be used if the file actually contains a GM binary header.

3.2.1.8.6 Import Fiat data

This option reads the file in t he Fiat binary format. The Fiat file s are split into two files, the

parameter file (*.prm) and the binary file (*.bin). The para meter file contains section

information, the checksum, etc. The binary file contains the actual data. HexView reads the

PRM file and interprets the section information.  Then it reads the ac tual data from the

binary file.

3.2.1.8.7 Import Ford IHex data

### Reads the header container information us ed by Ford and the following Intel-HEX

information from the file.

All information from the Ford header will be stored in an INI-file.

3.2.1.8.8 Import Ford VBF data

Reads the Ford VBF data file. This version of Hexview manages the vbf-version V2.2.

All information from the header will be stored in an INI-File.

3.2.1.9 Export

This item groups a number of diff erent options to store the inte rnal data into different file

formats. Each export can contain some options to adjust the output information.

3.2.1.9.1 Export as S-Record

This item exports the data in the Motorola S-Record format.



## Page 18

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

18 / 79

Figure 3-6 Export data in the Motorola S-Record format

The record type will be select ed automatically d epending on the length of the highest

address information.

The default values for start and end address will be the lowest respectively the highest

address of the file. The Output range specifier c an be used if just a portion of the internal

data shall be exported. The ra nge can be specified usi ng the start and end address

separated by a ‘-‘, or can be specified using the start addr ess and length separated by a

comma. Several ranges can be separated by  a colon ‘:’. Address and length can be

specified in hexadecimal with a preceding ‘0x’. Otherwise it is treated as a decimal value.

Examples:     0x190,0x20:0x9020-0x903f

The option “Max. bytes per record line” specifies the number of bytes per block for the S-

Record file. The [Browse] option allows to locate the file with the file dialog.

3.2.1.9.2 Export as Intel-HEX

Figure 3-7 Export dialog for the Intel-Hex output



## Page 19

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

19 / 79

Exports the data in Intel-HEX record format. This opens the following dialog for the export:

The address range of the out put can be limited (see 3.2.1.9.1 for a description on the

format and how to use the range specifier).

Hexview supports two different types of output on the Intel-H EX file format, the extended

linear segment and the extended segment. T he extended linear segment can store data

with address ranges up to 20 bits, whereas the extended linear segment format can

support address ranges with up to 32 bits ( address ranges with up to 16 bit length of

addresses are not using any extended segments).

In the auto-mode, the used s egment mode depends on the address length of each line. If

the address length of a line that shall be written exceeds 16 bits, but is lower or equal than

20 bits, the extended segment will be used. If the size of the address is larger than 20 bits,

the extended linear segment type will be used.

Sometimes it is necessary to restrict the number  of bytes per record line in the output file.

This can be adjusted with the “Max bytes per record line” parameter.

3.2.1.9.3 Export as HEX-ASCII

The internal data will be exported as HEX-ASC II. Each byte will be written as a pair of

characters. A separator between bytes can be sp ecified as well as the number of bytes

that shall be written per line before a newline will be inserted.

Figure 3-8 Export flashkernel data for CCP/XCP



## Page 20

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

20 / 79

3.2.1.9.4 Export as CCP Flashkernel

This option generates the internal data into an Intel-HEX file, including the data section

necessary for the CCP/XCP flash kernel.

Figure 3-9 Export flashkernel data for CCP/XCP

The section information is directly copied into the FKL-header section.

### The kernel header contains a few information about the kernel file name, both the

addresses of the RAM and the start address of the main application in the flash kernel.

### Info

The main application of each flash kernel starts with the function:

ccpBootLoaderStartup(), ensure FLASH_KERNEL_RAM_START has got the right

function address. Sometimes the flash kernel location is at the same address like a

vector interrupt table, to prove this, the developer must add the size of the kernel to the

FLASH_KERNEL_RAM_START address. For Example here

FLASH_KERNEL_RAM_START + FLASH_KERNEL_SIZE = 1533. That mean the RAM

area from 0x1000 – 0x1533 must be clear.

FLASH_KERNEL_NAME="xxxxx.fkl"

FLASH_KERNEL_COMMENT="Flash Kernel for xxxxxx"

FLASH_KERNEL_FILE_ADDR=0x1000

FLASH_KERNEL_SIZE=0x0533

FLASH_KERNEL_RAM_ADDR=0x1000

FLASH_KERNEL_RAM_START=0x1000



## Page 21

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

21 / 79

The parameters of the flash kernel reflects directly the input of the dialog.

These parameters are also written to an INI-f ile, so that it can be retrieved the next time

when this dialog will be opened. An example of the INI-file is shown below:

### [FLASH_KERNEL_CONFIG]

;FLASH_KERNEL_NAME="S12D64kernel.fkl"

FLASH_KERNEL_COMMENT="CCP Flash Kernel for Star12D64@16Mhz Version 1.0.0"

;FLASH_KERNEL_FILE_ADDR=0x039A

;FLASH_KERNEL_SIZE=0x0426

;FLASH_KERNEL_RAM_ADDR=0x039A

FLASH_KERNEL_RAM_START=0x039A

; or: FLASH_KERNEL_RAM_START=@S12D64Kernel.map:  ccpBootLoaderStartup                      %lx

Hint:

FLASH_KERNEL_NAME: If omitted, HexView will use the filename of the loaded file.

FLASH_KERNEL_ADDR: If omitted, HexView will use the lowest address of the block

FLASH_KERNEL_SIZE: If omitted, HexView will use the total size of the block

FLASH_KERNEL_RAM_START: If omitted, HexV iew will use the lowest address of the

block. See also description below.

Usually, the value of FLASH_KERNEL_RAM_START must specify the address location of

the function ccpBootLoaderStartup() in the flash kernel. Since this value can change

after changing the CCP-kernel files, a s pecial feature has been added to extract the

address information from a MAP-file. Even though t he implementation is very basic, it can

be very helpful. A special syntax enables th is feature. The line  must start with the ‘@’

followed by the MAP-file. A ‘:’ separates this information from the following line. This line is

used for a scan process of the MAP-file. HexView reads every line and tries to interpret the

MAP-file line by using the remaining parameter in an SSCANF function call. The

parameter “%lx” must represent the address value of  the function ccpBo otLoaderStartup.

If the scan process was not successful, HexV iew will add the complete line to the

parameter.

The example above extracts successfully the information from the following map-file

(extract of a Metrowerks compiler output):

MODULE:                 -- boot_ccp.obj --

### - PROCEDURES:

ccpBootLoaderStartup                      38EB      1E      30       0   .text

3.2.1.9.5 Expor t as C-Array

This option writes the data into a C-style file format:



## Page 22

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

22 / 79

Figure 3-10 Export data into a C-Array

The array size can be either 8-, 16- or 32-bit. If 16-bit or 32-bit is selected, the output can

be chosen as either Motorola (big-endian) or Intel (little-endian) style.

The array can be exported as pl ain C-data. But it is also possible to encrypt it. The

encryption will be an XOR operation with t he specified parameter. The decryption

parameter is also given in C-style.

The data is written into a C-array. The array name will use the prefix given from the dialog.

If the block contains several blocks, the data will be written into several C-Arrays. Each

block will contain the block number as a postfix.

Example for the C-File:

/****************************************************************

*  Filename:      D:\Usr\Armin\VC\HexView\_page4a.C

*  Project:       C-Array of Flash-Driver

*  File created:  Sun Jan 15 20:59:35 2006

****************************************************************/

#include <fbl_inc.h>

#include <_page4a.h>

#if (FLASHDRV_GEN_RAND!=1739)

# error "Generated header and C-File inconsistent!!"

#endif

V_MEMROM0 MEMORY_ROM unsigned char flashDrvBlk0[FLASHDRV_BLOCK0_LENGTH] = {

0x00, 0x01, 0x02, 0x03, 0x04, 0x05, 0x06, 0x07, 0x08, 0x09, 0x0A, 0x0B, 0x0C, 0x0D, 0x0E, 0x0F,

0x10, 0x11, 0x12, 0x13, 0x14, 0x15, 0x16, 0x17, 0x18, 0x19, 0x1A, 0x1B, 0x1C, 0x1D, 0x1E, 0x1F,

0x20, 0x21, 0x22, 0x23, 0x24, 0x25, 0x26, 0x27, 0x28, 0x29, 0x2A, 0x2B, 0x2C, 0x2D, 0x2E, 0x2F,

0x30, 0x31, 0x32, 0x33, 0x34, 0x35, 0x36, 0x37, 0x38, 0x39, 0x3A, 0x3B, 0x3C, 0x3D, 0x3E, 0x3F,

0x40, 0x41, 0x42, 0x43, 0x44, 0x45, 0x46, 0x47, 0x48, 0x49, 0x4A, 0x4B, 0x4C, 0x4D, 0x4E, 0x4F,

0x50, 0x51, 0x52, 0x53, 0x54, 0x55, 0x56, 0x57, 0x58, 0x59, 0x5A, 0x5B, 0x5C, 0x5D, 0x5E, 0x5F,

0x60, 0x61, 0x62, 0x63, 0x64, 0x65, 0x66, 0x67, 0x68, 0x69, 0x6A, 0x6B, 0x6C, 0x6D, 0x6E, 0x6F,

0x70, 0x71, 0x72, 0x73, 0x74, 0x75, 0x76, 0x77, 0x78, 0x79, 0x7A, 0x7B, 0x7C, 0x7D, 0x7E, 0x7F,

0x80, 0x81, 0x82, 0x83, 0x84, 0x85, 0x86, 0x87, 0x88, 0x89, 0x8A, 0x8B, 0x8C, 0x8D, 0x8E, 0x8F,



## Page 23

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

23 / 79

0x90, 0x91, 0x92, 0x93, 0x94, 0x95, 0x96, 0x97, 0x98, 0x99, 0x9A, 0x9B, 0x9C, 0x9D, 0x9E, 0x9F,

0xA0, 0xA1, 0xA2, 0xA3, 0xA4, 0xA5, 0xA6, 0xA7, 0xA8, 0xA9, 0xAA, 0xAB, 0xAC, 0xAD, 0xAE, 0xAF,

0xB0, 0xB1, 0xB2, 0xB3, 0xB4, 0xB5, 0xB6, 0xB7, 0xB8, 0xB9, 0xBA, 0xBB, 0xBC, 0xBD, 0xBE, 0xBF,

0xC0, 0xC1, 0xC2, 0xC3, 0xC4, 0xC5, 0xC6, 0xC7, 0xC8, 0xC9, 0xCA, 0xCB, 0xCC, 0xCD, 0xCE, 0xCF,

0xD0, 0xD1, 0xD2, 0xD3, 0xD4, 0xD5, 0xD6, 0xD7, 0xD8, 0xD9, 0xDA, 0xDB, 0xDC, 0xDD, 0xDE, 0xDF,

0xE0, 0xE1, 0xE2, 0xE3, 0xE4, 0xE5, 0xE6, 0xE7, 0xE8, 0xE9, 0xEA, 0xEB, 0xEC, 0xED, 0xEE, 0xEF,

0xF0, 0xF1, 0xF2, 0xF3, 0xF4, 0xF5, 0xF6, 0xF7, 0xF8, 0xF9, 0xFA, 0xFB, 0xFC, 0xFD, 0xFE, 0xFF

};

Example of the Header-File:

/****************************************************************

*

*  Filename:      D:\Usr\Armin\VC\HexView\_page4a.h

*  Project:       Exported definition of C-Array Flash-Driver

*  File created:  Sun Jan 15 20:59:35 2006

*

****************************************************************/

#define FLASHDRV_GEN_RAND 1739

#define FLASHDRV_DECRYPTDATA(a)   (unsigned char)a

#define FLASHDRV_BLOCK0_ADDRESS 0x9000

#define FLASHDRV_BLOCK0_LENGTH 0x100

#define FLASHDRV_BLOCK0_CHECKSUM 0x7F80u

extern V_MEMROM0 MEMORY_ROM unsigned char flashDrvBlk0[FLASHDRV_BLOCK0_LENGTH];

The macro [Prefix-name]_DECRYPTDATA() can be used to extract and encrypt the data. It

will be generated according to the encryption option and value.

The output can also generated via t he command line. Refer to section 4.3.2 for further

information.

The declaration of the C-arrays are dedicated to  the Vector bootloader. In some cases, it

might be necessary to use these structures  in a pure C-environment without compiler

abstraction used by Vector’s naming convention. Use the “Use strict Ansi-C declaration” in

this case.

Another option is to use so-called memmap-st atements. Hexview will generate statements

to delare a define and then include the file memmap.h:

### Example

Memmap declarations generated by Hexview:

#define FLASHDRV_START_SEC_CONST

#include "memmap.h"

The file memmap.h may look like this:

#ifdef FLASHDRV_START_SEC_CONST

#undef FLASHDRV_START_SEC_CONST

#pragma section .flashdrv

#endif



## Page 24

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

24 / 79

3.2.1.9.6 Export Mime coded data

This item exports the data file in MIME-coded format.

3.2.1.9.7 Export Binary data

This item will write all data contents in the order of their appearance into a binary file.

### All segments will be written linear into the data block

3.2.1.9.8 Export binary block data

This item will export the data into a binary file. Ho wever, if the internal data file contains

several blocks, the data is written to differ ent files. Each filename will have the base

address as a postfix.

File output names:

 _page3_overlap_fe2.bin

 _page3_overlap_4020.bin

 _page3_overlap_9000.bin

3.2.1.9.9 Export Fiat Binary File

This exports data in the FIAT file format.



## Page 25

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

25 / 79

Figure 3-11: Export dialog for the FIAT binary file

The dialog shown above can only be underst ood if the Fiat file format is known. This

document does not intend to explain this f ile format. Refer to 07284 01.pdf for further

explanation.

During the export, an INI-file will be updated or generat ed. If the INI-File was specified by

the commandline, this file will be used. Ot herwise, an existing file  will be updated or new

file will be generated with the same name and location as t he export filename. For the INI-

file format, refer to section 4.3.1, “Output a Fiat specific data file (/XB)”.

3.2.1.9.10 Export Ford Ihex data container

The file format generated with this output is based on the Ford-specification “Module

Programming & Configuration Design Specification”, V 2003.0, dated: 25 April 2005, Annex

### C.

Besides the download data itself, there are some optional and mandatory values added to

the output file. The optional fields can be selected/unselected with the option checkbox.

All values entered in the dialog below will be written to the INI-File. The INI-file can also be

used for the command line option to generate the output without the needs of a user input.

For detailed description of each item of the data fields, refer to the document mentioned

above. Further information can be found in section 4.3.3.1, “Output Ford files in Intel-HEX

format”.



## Page 26

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

26 / 79

Figure 3-12: Export dialog for Ford I-Hex output file

3.2.1.9.11 Export Ford VBF data container

The VBF file format is the Versatile Binary Forma t used by Ford. The output of this file is

based on the specification “Versatile Binary Format”, V2.2.

All values entered in the dialog below will be written to the INI-File. The INI-file can also be

used for the command line option to generate the output without the needs of a user input.

Refer to section 4.3.3.2, “Output Ford files in VBF format” for further information.



## Page 27

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

27 / 79

Figure 3-13: Export dialog fort he Ford-VBF data file ormat

3.2.1.9.12 Export GM data

This item is just present to in dicate, that the tool also supports GM-data export. In fact, the

GM data preparation must be done through the commandline option. More information can

be found in section 4.3.4ff,”Output a GM-specific data file”.

The GM data container is simply a binary file stream. It can be exported through the binary

export.

Figure 3-14: The output information for the GM data export



## Page 28

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

28 / 79

3.2.1.9.13 Export GM-FBL header info

This option provides the possibility to expor t the address and length information of each

segment into an XML-File. Also, the number of segments and the c hecksum value will be

written into the XML-file. If the checksum ta rget address is locat ed within the segment

array, the tool will automatically split this region into two to spare the location of the

checksum. Thus, the checksum can be re-calculated.

The purpose of this output is to read the XML-file into the configuration and generation tool

“Geny”. It is used to generate the GM-header info for the GM flash Bootloader. It allows the

Bootloader to calculate the checksum on its own data.

It may require two rounds (gener ate the configuration, comp ile and link the Bootloader,

generate the XML-file with Hexview) for a valid header.

Figure 3-15: Export dialog to generate the GM-FBL header information for GENy

The XML-file has the following format:

<!—Created by HexView v2006 (Vector Informatik GmbH) Æ

<ECU xmlns:xsi=”http://www.w3.org/2001/XMLSchema-instance”

xsi:noNamespaceSchemaLocation=”FBLConfiguration.xsd”>

<FBLConfiguration>

### <PMA ID=”1”>

<Checksum Value=”51434”/>

<NumberOfPMA Value=”2”/>

<PMAField>

<Address Value=”8380416”/>

<Length Value=”1932”/>

</PMAField>

<PMAField>

<Address Value=”8388368”/>

<Length Value=”240”/>

</PMAField>

### </PMA>

</FBLConfiguration>

### </ECU>



## Page 29

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

29 / 79

3.2.1.9.14 Export VAG data container

This item exports the data into a VAG-compatible data container format.

Figure 3-16 Exports data into a VAG-compatible data container

### Info

The generated VAG data file is NOT compatible with the ODX-F format used for UDS.

The VAG data container is a SGML-file that can be divided into five sections. Three

sections are merged from external files, two others are generated.

Section 1:

“SGM pre-header file”.

### HexView parses this

file and checks, if the

<!DOCTYPE SW-CNT PUBLIC “-//Volkswagen AG//DTD Datencontainer fuer die SG-

Programmierung V00.80:MiniDC08.DTD//GE” “minidc08.dtd”>

### <SW-CNT>

### <IDENT>

### <CNT-DATEI>  [1] </CNT-DATEI>

<CNT-VERSION-TYP>cvt_pfu_01</CNT-VERSION-TYP>

### <CNT-VERSION-INHALT>0.80</CNT-VERSION-INHALT>



## Page 30

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

30 / 79

fields in [1], [2] or [3]

are blank. If not blank,

it will copy the contents

as is from the file. But if

the fields are left blank,

it will be filled with

parameters from the

dialog box:

[1] = filename from

“destination file”

without the path

[2] = the value from

“S/W version”

[3] = the value from

“Part number”

<CNT-IDENT-TEXT>MyProject</CNT-IDENT-TEXT>

### <SW-VERSION-KURZ> [2] </SW-VERSION-KURZ>

### <SW-VERSION-LANG> [3] </SW-VERSION-LANG>

### </IDENT>

### <INFO>

### <ADRESSEN>

### <ADRESSE>

<FIRMENNAME>S/W-Development GmbH</FIRMENNAME>

<ROLLE>Entwicklung VAG-Software</ROLLE>

### <ABTEILUNG>ESVG</ABTEILUNG>

<PERSON>Klaus Mustermann</PERSON>

<ANSCHRIFT>Gewerbestrasse 40, D-03421 Ingolsheim</ANSCHRIFT>

### <TELEFON>+49-6234-123-456</TELEFON>

### <FAX>+49-6234-123-200</FAX>

<EMAIL>Klaus.Mustermann@sw-develop.de</EMAIL>

### </ADRESSE>

### </ADRESSEN>

### <REVISIONEN>

### <REVISION>

### <WANN></WANN>

### <WER></WER>

### <WAS></WAS>

### <WARUM></WARUM>

### <VERSION></VERSION>

### </REVISION>

### </REVISIONEN>

### </INFO>

### <ABLAEUFE>

### <ABLAUF>

<ABLAUF-NAME>abn_pfu</ABLAUF-NAME>

### <KWP-2000>

<KWP-2000-TGT>0x62</KWP-2000-TGT>

### <KWP-2000-REI>

### <KWP-2000-PSTAT-BIT0>255</KWP-2000-PSTAT-BIT0>

### <KWP-2000-PSTAT-BIT1>6</KWP-2000-PSTAT-BIT1>

### <KWP-2000-PSTAT-BIT2>10</KWP-2000-PSTAT-BIT2>

### <KWP-2000-PSTAT-BIT3>0</KWP-2000-PSTAT-BIT3>

### <KWP-2000-PSTAT-BIT4>0</KWP-2000-PSTAT-BIT4>

### <KWP-2000-PSTAT-BIT5>0</KWP-2000-PSTAT-BIT5>

### <KWP-2000-PSTAT-BIT6>0</KWP-2000-PSTAT-BIT6>

### <KWP-2000-PSTAT-BIT7>0</KWP-2000-PSTAT-BIT7>

### </KWP-2000-REI>

### <KWP-2000-ACP>

<KWP-2000-P2MIN>0xFF</KWP-2000-P2MIN>

<KWP-2000-P2MAX>0xFF</KWP-2000-P2MAX>

<KWP-2000-P3MIN>0xFF</KWP-2000-P3MIN>

<KWP-2000-P3MAX>0xFF</KWP-2000-P3MAX>

<KWP-2000-P4MIN>0xFF</KWP-2000-P4MIN>

### </KWP-2000-ACP>

<KWP-2000-SA2>0x12,0x23,0x23,0x34,0x45,0x56C</KWP-2000-SA2>

### </KWP-2000>

Section 2:

Generated “Data

Reference section”

### The reference section

contains a reference to

each segment or block.

### An external Hex-file

can be added for

reference, e.g. a HIS-

flash driver.  It is

necessary that this hex

field contains only one

segment or block.

### <DATEN-VERWEISE>

### <DATEN-VERWEIS>FLASHDRV</DATEN-VERWEIS>

<DATEN-VERWEIS>dav_pfu_01</DATEN-VERWEIS>

### </DATEN-VERWEISE>

Section 3:

“SGM post-header

### </ABLAUF>

### </ABLAEUFE>



## Page 31

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

31 / 79

file”.

Section 4:

Generated “data

section”.

### This section contains

the current data. On

the right side an

example of the output

is shown.

### Start and end address

is taken from the block

information. The

checksum is calculated

with the given

checksum method (see

section 3.2.2.5 or 4.2.7

for further details on

checksum calculation).

### The erase section is

calculated out of the

section length. The

value of

### <DATENBLOCK-

FORMAT> is taken

from the “Data Format

ID” field in the dialog

box.

The <DATENBLOCK-

DATEN> contains the

data of the block or

segment in a MIME-

coded format.

<DATENBLOCK-NAME>dav_pfu_01</DATENBLOCK-NAME>

<DATENBLOCK-FORMAT-NAME>dfn_mime</DATENBLOCK-FORMAT-NAME>

<START-ADR>0x9000</START-ADR>

<DATENBLOCK-FORMAT>0x00</DATENBLOCK-FORMAT>

<GROESSE-DEKOMPRIMIERT>0xFA2</GROESSE-DEKOMPRIMIERT>

### <LOESCH-BEREICH>

<START-ADR>0x9000</START-ADR>

<END-ADR>0x9FA1</END-ADR>

### </LOESCH-BEREICH>

### <DATENBLOCK-CHECK>

<START-ADR>0x9000</START-ADR>

<END-ADR>0x9FA1</END-ADR>

<CHECKSUMME>0xA866</CHECKSUMME>

### </DATENBLOCK-CHECK>

### <DATENBLOCK-DATEN>

MIME-Version: 1.0

WflaW1xdXl9gYWJjZGVmZ2hpamtsbW5vcHFyc3R1dnd4eXp7fH1+f4CbgoOE

hYaHiImKi4yNjo+QkZKTlJWWl5iZmpucnZ6foKGio6SlpqeoqaqrrK2ur7Cx

srO0tba3uLm6u7y9vr/AwcLDxMXGx8jJysvMzc7P0NHS09TV1tfY2drb3N3e

### </DATENBLOCK-DATEN>

### </DATENBLOCK>

### </DATENBLOECKE>

### </DATEN>

Section 5:

### Appending file contents

from „SGM footer file“

### </SW-CNT>

Table 3-3: Description of the elements for the VAG SGML output container

It should be noted, that the filename is automatically generated out of the part number and

the S/W-version fields whenever the fields are changed. You can overwrite the name if the

filename is changed at last. When editing the filename or [Browse] for a file, the name will

not automatically adapted.

It is also possible to preprocess the data before  it is MIME-coded. Th is process is done

after the checksum calculation. It is intended to be used for e.g. Data Encryption.

It uses the standard interface functions from  the EXPDATPROC.DLL (refer to section 5.2,

3.2.2.6 and 4.2.8 for further details).

3.2.1.9.14.1 INI-File info for VAG export

The dialog information is stored in an INI-file. Th is file has the same name as the HEX-file,

but with the file extension INI. Every time this  dialog will be opened, CANflash checks for



## Page 32

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

32 / 79

such an INI-file and retrieves the information from there. Th is allows to store project

information in separate files. It is a prerequisite that the INI-file resides in the same folder

as the HEX-file.

This INI-File can then also be used in the command line option.

The following list file shows an example of the INI-file:

### [SGMDATA]

DATENBLOCKNAME=dav_pfu

### FLASHDRVSECTION=FLASHDRV

FLASHDRV=D:\Usr\Armin\VC\HexView\FLASHCODE_SH70XXF_704.hex

SGMHEADERPRE=header1.txt

SGMHEADERPOST=header2.txt

SGMFOOTER=footer.txt

### CHECKSUMTYPE=2

### DATAPROCESSINGTYPE=0

### DATAPROCESSINGPARAMETER=1234567890

PARTNUMBER=123456789ab

SW_VERSION=cdef

### FLASHDRV_DLID=12

### DATA_DLID=24

MAXBLOCKLEN=0x400

### Info

This INI-file is automatically created when executing this dialog.

3.2.1.9.15 Print / Print Preview / Printer Setup

There is no special support for printer output ot her than that from the MFC. Thus, the view

output will directly sent to the printer.

3.2.1.9.16 Exit

Leaves the program.

3.2.2 Edit

This menu item collects some options that can be used to manipulate data in HexView.

3.2.2.1 Undo

This option is currently not supported by HexView.

3.2.2.2 Cut / Copy / Paste

Hexview uses an internal clipboard. Cut and Copy  can put data into this clipboard. Even if

files are closed and others are opened, the data remain in clipboard.

It allows, to cut or copy data regions and put it  into the data section. As a new challenge,

another syntax to specify range has been intr oduced. Different from the other regions,

where start and end address must be specif ied as HEX-values, the range can now

specified in one single string. The range can be specified in two ways: Using start- and end

address or with startaddress and length.



## Page 33

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

33 / 79

Start and end address is separated with a ‘-‘ sign. Startaddress and length are separated

with a ‘,’.

Example:

0x10000-0x1 ffff

This specifies start- and end-address in hexadecimal value. A ‘0x’ is required to

preceed. If ‘0x‘ is omitted,  the value is treated as a decimal value. This allows to use

the parameters in both hexadecimal or decimal values.

Figure 3-17: Example of 'Copy window' when Ctrl-C  or "Paste" pressed using start- and end-address

0x20000,256

This specifies a range from 0x20000 with length of 256 bytes (0x100 bytes). It is the

range of 0x20000-0x201FF.

The standard short-cuts (acceleration keys) are introduced.

Figure 3-18: Example of cut-data using start-address and length as a parameter

Cut or paste can only be used if data has been loaded into the file.

The paste-operation is activated when something is present in the clipboard.

When ‘Paste’  (Ctrl-V) is entered, a window will o pen where the target  paste address can

be specified. By default, the clipboard’s start address will be shown as a default value. This

can be overwritten. An addr ess offset will be applied to  the pasting range from the

clipboard.



## Page 34

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

34 / 79

Figure 3-19: Pasting the clipboard data into the document specifying the target address

3.2.2.3 Data Alignment

Data Alignment operates on the block start addr ess and its length. This can be used to

adjust the start address and length on all blocks/segments.

Figure 3-20 Data alignment option

This option ensures, that the start address of a ll blocks is a multiple  of the segment size

alignment value. E.g., if this  parameter is 2, then HexView ensures that all addresses are

even (dividable by 2 without remainder). If an odd address is detected, HexView fills bytes

with the “Fill character” at the beginning of a block until the address is even.

If “Align size” is selected, too, the size of all blocks is a multiple of the given segment

alignment value. If a lengt h of a block is not a multiple of  the segment alig n value, a fill

pattern will be added until the size meets this condition.

Some export file formats contain separate address and length information used to specify

the erasable ranges of a flash memory. These address ranges require different alignment

definition. This align va lue can be specified in the “Erase segment alignment”. It is mainly

used with Ford-VBF and Fiat binary/parameter f iles. This value can also specified through

the commandline option /AE.

3.2.2.4 Fill block data

This option provides the ability to fill data r egions. This is possible with either random data

or with a pattern that will be added repetitively.



## Page 35

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

35 / 79

Within the dialog, one or more  block ranges must be given. This parameter is used to

generate the block base address and its size.

The overwrite method specifies how to treat t he fill data with the existing data. If the new

data overlaps, the new data may ov erwrite it or will be weaved into the existing data as a

fill pattern.

The data pattern can either be a random data value or can be filled with a given pattern..

Figure 3-21 Dialog that allows to fill data

3.2.2.5 Create Checksum

There are two different methods to allow to operate on the data set of the loaded file info:

 data processing

 checksum calculation.

Data processing operates directly on the data set and change it. The checksum calculation

operates on the data without changing them. The resulting value can be added to the data

set.

The dialog above shows the method to operate on the data. The checksum range can

limit the data section where the checksum calculation operates  on. Please note, that you

can specify only one range. If several ranges are specified using the colon separator, only

the first one will be used to limit the data area.



## Page 36

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

36 / 79

Figure 3-22 Dialog to operat e the checksum calculation

The checksum type depends on the capability of the underlying checksum DLL. For the

interfaces, refer to section 5.1. Also, section “ Checksum calculation method

(/CSx[:target[;limited_range][/no_range])” provides further details on checksum calculation.

The button [Calculate] will run the calculation and sh ows the result in the field checksum

value. If [Insert] is selected, the checksum calculation will be performed and the result will

be added to the internal data blocks on the given address.

3.2.2.6 Run Data Processing

The second method that uses the EXPDATPRO C.DLL functions is the data processing

field. As already mentioned in the Checksum  calculation section,  the data processing

directly operates on the inter nal data. Most of these operations requires a parameter for

this operation. Typically, the resulting data is the manipulated data. Therefore, no result of

the data processing can be inserted or added to the data sections.

Figure 3-23 Dialog for Data Processing

The data processing allows to operate on the data. Typical applications are data

decryption/encryption or compression/decompression.



## Page 37

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

37 / 79

The string value given in the Parameter field is passed to the routines for the data

processing.

The Data processing range  can limit the data range, w here the data processing will

operate on. The parameter will be stored in the registry, to retrieve the information the next

time this option is activated. Please note, that you can specify only one range. If several

ranges are specified using the colon separato r, only the first one will be used to limit the

data area.

See also section 5.2 for further details on the DLL-interface. Pl ease, read also section

“Run Data Processing interface (/DPn:param [,section,key][;outfilename])” for more details

on available data processing functions.

Some data processing options allow to use a file that contains the parameter. You can

browse for the specific file using the “Browse” button.

3.2.2.7 Edit/Create OEM Container-Info

This option is currently not available.

3.2.2.8 Remap S12 Phys->Lin

This option is used to remap all blocks fr om physical paged addressing to the linear

address mode. It is dedicated to be used with HEX-files with paged address information for

the Motorola Star12 (MC9S12 family). The Star12 paged addressing mode uses 24-bit

addresses, where the upper 8-bit specifies t he bank address in the range from 0x30 to

0x3F. The lower 16-bit address is the physica l bank address in the range from 0x8000-

0xBFFF. These address ranges are shifted to the linear addresses starting from

0x0C.0000 for Bank 0x30 up to the highest address 0xF.FFFF.

The non-banked addresses from 0x4000-0x7 FFF and 0xC000-0xFFFF are mapped to the

linear address range of the corresponding p ages (0x4000-0x7FFF mapped to 0x0F.8000-

0x0F.BFFF [Bank 0x3E] and 0xC000-0xF FFF mapped to 0x0F.C000-0x0F.FFFF (Bank

0x3F]). See also chapter 4.2.19 for further explanations.

3.2.2.9 Remap S12x Phys->Lin

This option is used to remap all blocks fr om physical paged addre ssing to the linear

address mode. It is dedicated to be used with HEX-files with paged address information for

the Motorola Star12X (MC9S12X family). The Star12X paged addressing mode uses 24-bit

addresses, where the upper 8-bit specifies t he bank address in the range from 0xE0 to

0xFF. The lower 16-bit address is the physica l bank address in the range from 0x8000-

0xBFFF. These address ranges are shifted to the linear addresses starting from 0x78.0000

for Bank 0xE0 up to the highest address 0x7F.FFFF.

The non-banked addresses from 0x4000-0x7 FFF and 0xC000-0xFFFF are mapped to the

linear address range of the corresponding p ages (0x4000-0x7FFF mapped to 0x7F.4000-

0x7F.7FFF [Bank 0xFD] and 0xC000-0xF FFF mapped to 0x7F.C000-0x7F.FFFF (Bank

0xFF]). See also chapter 4.2.19 for further explanations.

3.2.2.10 General Remapping

This option can be used to remap any bank ed address information in to a linear address

range, e.g. for the Motorola MCS08 or NEC 78k0.

Detailed information about banked and linear addresses can be found in chapter 4.2.19.



## Page 38

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

38 / 79

Figure 3-24: Configuration window for general remapping

3.2.2.11 Run Postbuild

This option allows to scan for postbuild files. Typically, a postbuild file contains address

and length information as well as data information which shall be used to overwrite the

current contents within a hexfile. With Hexview V1.6 and higher it is even possible to

create segment blocks based on the information in a postbuild file.

Note, that the postbuild option is only available if the pbuild.dll is avai lable. After selecting

the item Edit -> Run postbuild , you can select one or more XM L files that follows the data

scheme for postbuild. Normally, the postbuild files will be generated by Geny. If you need

further information about the postbuild options, please contact Vector.

3.2.3 View

This menu item provides some features to control the view.

3.2.3.1 Goto address…

This item allows to jump to a specific address within the view.



## Page 39

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

39 / 79

Figure 3-25: Jump to a specific address in the display window

The address value is entered in a hexadecimal form.

If the address is valid, the slider  will be moved to the beginni ng of the address. Thus, the

address information will be shown on the top of the display. The line is not highlighted.

A way to jump to the beginning of an address block can be done by jump to the beginning

of the file (press POS1 or Ctrl-Pageup button)

3.2.3.2 Find record

This option allows to search for a pattern within the file.

Figure 3-26: Find a string or pattern within the document

The format of the pattern can be selected on the right side of the window. By default, the

data pattern is given as a hexadecimal data byte stream. The search algorithm searches

from the beginning until the pr esence of this pattern is found. HexView tries to display the

value on the top of the screen.  If a pattern has been found, the search can be repeated

from the last position where the pattern has been found.

If the “Find-string format” is changed to “ASCII-string”, the pattern entered in “Find what”

will be treated as an ASCII pattern and will search for the ASCII values.

3.2.3.3 Repeat last find

This option is only present after a successful search operation. This item will continue the

search given from “View -> Find record”.

3.2.3.4 View OEM container info

This option was implemented to  present some OEM-specific in formation available in the

file. However, at the moment only the GM header information will be shown.

This may be extended in the future.

3.2.4 Flash

This menu item is directly related to the flash process.



## Page 40

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

40 / 79

3.2.4.1 CANflash

This item provides the option to select one of the installed CANflash programs.

Once the CANflash has been se lected, Hexview automatically checks for previously used

databases. After selecting the database(s) all nodes pre-selected by previous execution of

CANflash can be selected. If all items are se lected successfully, the flash process can be

started directly for this ECU. If “Auto flash”  is selected and the “Flash ECU” button is

pushed CANflash is started immediately. The flash process will be started and CANflash

will close automatically after the flash process has been concluded successfully.

At least, it is possible to start the select ed the CANflash program. Here, you need to make

all selections to start the flash process.

Figure 3-27: Select an installed version of CANflash and may start it.

3.2.5 Info operation (?)

This option contains the About information of HexView. It shows the version of the tool and

displays also the copyright information.



## Page 41

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

41 / 79

3.3 Accelerator Keys (short-cut keys)

Some of the menu items mentioned above can be entered by hotkeys or accelerator keys.

This can be helpful to activate functions from the keyboard without using the menu and the

mouse.

The following table provides a list of available accelerator keys:

### Accelerator key Description

Ctrl+A Align data

Ctrl+B Run postbuild configuration

Ctrl+C Copy data to the internal clipboard

Ctrl+D Data Processing

Ctrl+F Find record

Ctrl+G Goto address

Ctrl+K Open checksum calculation dialog

Ctrl+L Opens the fill data dialog

Ctrl+N File new

Ctrl+O Open file

Ctrl+P Print file

Ctrl+S Save current file

Ctrl+T Generate validation structure information

Ctrl+V Paste data from clipboard into the currently loaded document

Ctrl+X Remove data from current document and put them into the

internal clipboard

Alt+A Export as HEX-ASCII

Alt+B Export Fiat binary

Alt+C Export C-Array

Alt+E Export Ford Intel-HEX format

Alt+F Export Ford VBF format

Alt+G Export GM file format

Alt+I Export Intel-HEX

Alt+L Export GM-FBL data

Alt+M Export MIME-Data

Alt+N Export Binary data

Alt+S Export S-Record

Alt+V Export VAG-Data

Alt+Y Export splitted binary file.

F3 Repeat last find

Alt+F4 Exit application

### DEL Delete a range from the currently loaded document

Table 3-4: Accelerator keys (short-cut keys)  available in Hexview



## Page 42

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

42 / 79

4 Command line

HexView cannot only be used as a PC-program with a GUI to display information. It is also

possible to manipulate the data via command line. There are even some options only

available through command lines.

The following section describes the usage of the command line.

The command line can be grouped r oughly into two groups: genera l options that operates

generally and OEM-related command line options. The OEM command line options control

the generation of files in OEM specific file formats.

4.1 Command line options summary

This section provides a summary of all comm and line options. An option must start either

with a ‘/’ or a ‘-‘. In this description, a slash is used. The switches are not case-sensitive.

Some options require additional parameter information. Some parameters are followed

directly by the option, some others require a separator. The separator can either be the

equal-sign or a colon.

Hexview infile  [options] [-o outfile]

### Command line option Description

### Infile This is the input filename either in Intel-HEX or Motorola

### S-Record format

/Ad:xx

/ADyy

Align data. Xx is specified in standard-C notation, e.g.

0xFF, whereas yy are only hex-digits. Format is

distinguished by the separator ‘:’ or ‘=’.

/AL Align length.

/Afxx Specifies the fill character for /AL, /AD and /FA

/AR:’range’1 Load a limited range of data.

The ‘range’ is an address range, that can be specified in

two ways: either with start address and length, separated

by a comma, or with start address and end address,

separated by a minus-sign.

/CR:’range1’:’range2’:… Cut out data ranges from the loaded file

/CSxx:target[;limited_range]

[/exclude_range1]

[/exclude_range2]

[:target[;limited_range]

[/exclude_range1]

[/exclude_range2]]…

This option specifies the checksum calculation method. If

the optional location parameter is added, the checksum

value is written into this file. The result can also placed

into the file using the @ operator.

Note: ‘location’ is a pre-requisit in most cases.

/DLS=AA or /DLS=ABC This option is used in combination with the /XG group

option to specify the DLS code and length.

The DLS code can be 2 or 3 characters. A ‘=’ is required

between the option and the characters itself.

/DCID=0x8000 This option is used in combination with the /XG group



## Page 43

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

43 / 79

/DCID:32238 option to specify the DCID code. The value can be

represented in integer or hexadecimal. In the latter case,

a ‘0x’ must preceed the value. The value is treaded as a

16-bit value and will be added to the header when

creating the GM-header.

/DPn:param Run the data processing interface from expdatproc.dll.

The value ‘n’ specifies the method, ‘param’ is sued as the

string parameter to the DoDataProcessing function.

/E=errorfile

/e:errorfile

This specifies an error log file. HexView can run in silent

mode. In that case, no error will be displayed to the GUI.

However, error messages are also suppressed. This

option allows an error report to the file in the silent mode.

/FA Create a single region file (fill all)

/FR:’range1’:’range2’:… 1 Fill regions.

/FP:11223344 Fill pattern in hex. Used by the /FR parameter

/II2=filename.hex Special import for 16-bit addressed Intel-HEX files

/L:logfile.log Load and execute a commandfile

/MPFH[=cal1.hex+cal2.hex+…] Special option fo r /XG. Sets the MPFH flag and optionally

adds the address, length and DCID-info to the GM-

header.

/MPFH must be specified if an existing NOAM-field shall

be re-positioned adjacent to the new NOAR-field.

/MODID:value Special option for GM -header creation. Sets the Module-

ID for this header.

/MO:file1[;offset]

[+file2][;offset]

Merges the file(s) from the filelist into the memory in

Opaque mode (existing data will be overwritten). The

optional offset may be added to all addresses of the file

that is merged.

/MT:file1

[;offset][:range 1]

[+file2][;offset][:range 1]

Merges the file(s) or portions of it from the filelist into the

memory in transparent mode (existing data not

overwritten). The optional offset will be applied to all

addresses of the file that is merged. The range limits the

before the offset

-o outfilename Specifies the output filename.

/P:ini-file Specifies the path and file for the INI-information partly

used by some conversion routines.

/PB:”PostbuildXML-file1”;”XML-File2”;… Applie s Postbuild operation to the specified file.

/PN Add part number to the GM-header. This option is only

useful in combination with /XGC or /XGCC. The part

number must not be specified and will be taken from the

SWMI value.

/remap

[:range,bankbase,banksize,linearbase]

### This option was intended to be used for controllers using

a memory banked addressing scheme. The option

calculates from physical banked addressing to a linear

addressing scheme.

### One of the most popular controllers using banked

method, the Star12 and Star12x, is directly supported with



## Page 44

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

44 / 79

the special option /s12map resp. /s12xmap (see below).

/swmi:value Specifies the SWMI parameter when creating the GM-

header

/s Run HexView in silent mode.

/s08map Re-maps the physical address spaces of the Freescale

Star08 to its linear address spaces, e.g. maps segments

in the range of 0x4000-0x7FFF to 0x104.000 or from

0x02.8000-0x02.BFFF to 0x10.8000-0x10.BFFF and so

on.

/s12map Re-maps the physical address space to the linear

address space of the Freescale Star12 to its linear

address spaces, e.g. maps segments in the range of

0x4000-0x7FFF to 0xF8000 or from 0x308000-0x30BFFF

to 0xC0000-0xC3FFF and so on.

/s12xmap Re-maps the physical address space to the linear

address space of the Freescale Star12x to its linear

address spaces, e.g. maps segments in the range of

0x4000-0x7FFF to 0x7F4000-0x7F7FFF or from

0xE08000-0xE0BFFF to 0x780000-0x783FFF and so on.

/vs Create validation structure

/XB Outputs the data in the Fiat binary format including the

PRM- and BIN-file .

/XC Outputs the data into a C-like array

/XF Exports data in the Ford-specific file format. Generates

header information  and data in the  Intel-HEX file format.

/XG[:header-address] Completes the information in an existing GM-header

/XGC[:header-address] Generates the GM-file header and completes the

information.

/XGCC[:header-address] Generates the header information for a single-region

calibration file.

/XGCS Generates the header, but with a 1-byte HFI information

(backward compatibility with previous “SAAB”-specific

header).

/XGMFBL Exports the GM-FBL XML-data file

/XI[:reclinelen] Exports in Intel-HEX format

/XK Outputs the data into an FKL-file for CCP/XCP kernel

/XN Exports data into the binary file format

/XP Exports data into a single region binary file and appends

a checksum. Typically used by a Porsche download

### (KWP2000).

/XS[:reclinelen] Exports in Motorola S-Record format

/XV Outputs the VAG-compatible SGML file format.

/XVBF Generates the Ford-specific VBF file format.

Table 4-1: Command line options summary



## Page 45

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

45 / 79

1 A range defines a section area.  It can be entered in two ways,  either with start address

and length or with start address and end addre ss. Examples are: 0x1000,0x200 or

0x1000-0x11FF. Both parameters spans the same range and will be treaded the same

way. Note that the end address must be higher than the start address.

### Info

Parameter /Xx cannot be combined. /Xx can be specified only once in the parameter list.

/Mt and /MO cannot be combined as well.



## Page 46

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

46 / 79

4.2 General command line operation order

The commandlines can be specified in any order. Hexview will first summarize the

### Read data from input file using the auto-

filetype detection

Apply /E. Open log-file

Apply /S. Suppress messages

Apply /II2. Import Intel-Hex 16-Bit

Apply /S12map or /s12xmap (only one of

the options can be applied)

Apply /remap.

Apply /FR: Fill ranges operation

Apply /CR. Cut ranges

Apply /MT or /MO, merge operation. Only

one of them can be applied.

### Apply /AR to load only a limited range

Apply /L. Execute the LOG-file.

Apply /FA: Create a single-region file

Apply /PB. Load the post-build parameter

Apply /ADxx and /AL. Align address and

length.

Apply /DP. Execute data processing

Apply /CS. Run checksum calculation

Apply /Xx. Export data. Since only one

/Xx can be applied, only the last /Xx

option will execute.

Figure 4-1: Order of commandline operations within Hexview.



## Page 47

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

47 / 79

commandline operations and will then execut e them. Since some operations may have

influences to subsequent operations, the commandline operation sequence within hexview

is important to know. The following commandline sequence will be applied (if specified):

This section describes command line options of HexV iew, that can be used in general.

There is no restriction or limitation in the co mbination of the options (as long as they are

useful).

4.2.1 Align Data (/ADxx or /AD:yy)

The start address of each block will be aligned to multiples of the given parameter xx. If the

separator ‘:’ or ‘=’ is omitted, the parameter xx is a hexadecimal value. If the separator is

used, the value xx is interpreted in C-style,  e.g. /AD:0xFF is t he same as /AD:255 or

/AD:11111111b. This value can only be an unsigned char value.

### Example

### /AD2

Aligns address to be a multiple of 2.

If a block starts at 0xFE01 a fill byte will be inserted at 0xFE00. The inserted character

will be 0xFF by default. The default character can be overwritten with the /AF parameter.

An address starting at 0xE000 will be left unchanged. No characters are inserted.

/AD:0x80

Align the addresses of all sections to a multiple of 128

If an address starts at e.g. 0xE730, the address will be aligned to 0xE700.

4.2.2 Align length (/AL)

This option is only useful in combination with the /AD parameter. It aligns also the length of

all blocks to be a multiple of the parameter given in the /ADxx option. The option

corresponds to the “Align size” option in section 3.2.2.3: “Data Alignment”.

### Example

### /AD4 /AL

A block 0xE432-0xE47E will be aligned to 0xE430-0xE47F. All characters will be

filled with 0xFF or the value specified by /AFxx.

4.2.3 Specify erase alignment value (/AE:xxx)

This parameter specifies the erase alignment pa rameter. This value is used to align data

blocks that specifies erase blocks for certain output file formats for Ford and Fiat.



## Page 48

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

48 / 79

### Example

/AF:0xEF

Fill character is 0xEF

### /AFCD

Fill character is 0xCD

4.2.4 Specify fill character (/AF:xx)

This option specifies the fill character used for t he align options (/AL, /A D or /FA). If the fill

parameter is located directly after the option, it is treaded as a hex- string. If the parameter

is separated by a colon, the parameter must  use the C-convention for characters, e.g.

0xCC for hexadecimal values.

This option corresponds to the “Fill character” in section 3.2.2.3: “Data Alignment”.

### Example

/AF:0xEF

Fill character is 0xEF

### /AFCD

Fill character is 0xCD

4.2.5 Address range reduction (/AR:’range’)

This option can limit the range of data to be loaded into the memory. This is useful if only a

reduced range of data shall be processed within HexView.

An address range is specified by its block start address and its length. Address and length

are separated by a comma. You can also s pecify the  range wit h the start and end

address. Then, the two values must be  separated by ‘-‘.

### Example

/AR:0x1000,0x200

Only the data between 0x1000 and 0x11 FF are loaded to the memory and then

further processed.

/AR:0x7000-0x7FFF

This loads the data from 0x7000 to 0x7FFF



## Page 49

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

49 / 79

4.2.6 Cut out data from loaded  file (/CR:’range1[:’range2’:…]

The parameter option /CR is used to cut out a range from the loaded data file. It removes

any data within the specified ranges. More than one range can be spec ified. Each range

must be separated by a colon ‘:’.

### Example

/CR:0x1000,0x200

If a data section in the range from 0x1000-0x11FF exist, the data will be removed

from the file. All successive operations will operate on data that don’t include this

section. All other sections remain uncha nged. If this section is located within a

segment or block, it will be splitted into two.

/CR:0x7000-0x7FFF

This removes the data from 0x7000 to 0x7FFF if present.

4.2.7 Checksum calculation method (/ CSx[:target[;limited_range][/no_range])

This option is used to specify the checksu m calculation method provided by the checksum

calculation feature. The checksum calculation

### When using, The parameter x in the option /CSx denotes the i ndex to the checksum

calculation algorithm. The function in t he EXPDATPROC.DLL will be called that

corresponds to this parameter value. The inde x can be calculated by counting the list of

checksum methods in the checksum dialog starting with index 01.

Example:

Figure 4-2: Example on how to select the checksu m calculation methods in the "Create Checksum"

operation

### Examples

/CS6:csum.txt

Runs the checksum calculation method “Wordsum LE into 16-Bit, 2’s Compl LE-

Out (GM new style)” and writes the results into the file CSUM.TXT.

This example uses the checksum method “Wordsum LE into 16-Bit, 2’s Compl

LE-Out (GM new style)”, as this is the 7 th option in the checksum dialog menu

shown above.

1 Newer versions of expdatproc.dll (V1.3 and higher) shows the function index in the dialog.



## Page 50

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

50 / 79

/CS1:@append;0x1000-0x7FFF  or  /CS1:@append;0x1000,0x7000

Runs the checksum calculation method “Bytesum into a 16-Bit LE-out” and

appends the checksum at the very end of the internal file. The checksum is

calculated over the limited range from 0x1000-0x7FFF as specified.

### A range within the checksum range can be ex cluded, if for example a data array

shall not be used for checksum calcul ation, Such an ex cluded range can be

specified with a preceding ‘/’.

/CS7:@upfront;0x2000-0x3fff/0x2800-0x29ff/0x3000,0x200

The option above calculates the checksum using method 7 (the 8 th) on data

within the range from 0x2000-0x3ffff. The range from 0x2800-0x29ff and 0x3000-

0x31ff will be excluded for the checksum ca lculation. The exclude has no affect

to the real data. The result of the che cksum calculation will be written before the

very beginning of the file data (Note: it will be written not up front to 0x2000, but

to the very beginning of the loaded file. This applies to all ot her labelled address

specifier, such as ‘upfront’, ‘begin’ and ‘append’).

With HexView version V1.2.0 and higher, the results of the checksum can now also be

written into an output file or placed into a loca tion within the internal data. The location is

separated by a ‘:’ or ‘=’ sign, followed by the target where the resulting checksum value

shall be placed in. The example above shows how  to write the results of the checksum

calculation into the file “csum.txt”.

The following target IDs can be used:

### Target Description

Filename (e.g. csum.txt) Writes the result into a file. The value is written from high to low byte

in hexadecimal form. Each byte is separated by a comma.

@append The results of the checksum will be added at the very end of the file.

@begin Writes the contents at the very beginning of the file.

Note: It will overwrite the first bytes of your data. The number of

bytes that will be overwritten depends on the checksum method.

@upfront Write the checksum results prior to the beginning of the first block. No

data will be overwritten.

@0x1234 Writes the checksum result into the address location given after the

@ operator.

### Caution

Whenever using the @ operator to write the results into the file, make sure that the

checksum is at the proper location and is not  overwriting accidentally any imported data!

Table 4-2: Checksum location operators used in the commandline

The available checksum met hods depends on the ex pdatproc.dll. Version 1.05.00 of the

DLL provides the following methods:



## Page 51

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

51 / 79

### Index Method Description

0 ByteSum into 16-Bit, BE-out Sums the bytes of all segments into a 16-bit value. The

result is a 16-Bit value in Big-Endian order (high byte first).

1 ByteSum into 16-Bit, LE-out Sums the bytes of all segments into a 16-bit value. The

result is a 16-Bit value in Little-Endian order (low-byte first)

2 Wordsum BE into 16-Bit, BE-Out Sums the data of every segment as 16-bit words. The result

is a 16-bit value.

The input stream is treaded as big-endians (high-byte first),

the 16-bit checksum result is given in big-endian format

(high-byte first).

Note that this routine requires aligned data. The number of

bytes per segment and the start address of each segment

must be a multiple of two. If not, Hexview/expdatproc will

generate the errors “Base address mis-alignment” or “Data

length mis-alignment”

3 Wordsum LE into 16-Bit, LE-Out Same as above, but the data are treaded as 16-bit values

with low byte first. The 16-bit result is also stored with low-

byte first

4 ByteSum w/ 2s complement into

16-Bit BE (GM old-style)

Each byte of the segments are complemented with its 2’s

complement and then added to a 16-bit sum value. The

result is stored in big-endian format (high-byte first).

5 Wordsum BE into 16-Bit, 2's Compl

BE-Out (GM new style)

Sums the data of every segment as 16-bit words. The result

is the 2’s complement of the  16-bit sum.

The input stream is treaded as big-endians (high-byte first),

the 16-bit checksum result is given in big-endian format

(high-byte first).

Note that this routine requires aligned data. The number of

bytes per segment and the start address of each segment

must be a multiple of two. If not, Hexview/expdatproc will

generate the errors “Base address mis-alignment” or “Data

length mis-alignment”

6 Wordsum LE into 16-Bit, 2's Compl

LE-Out (GM new style)

### Same as above, but the input data is managed in little-

endian format. The result is also given as 16-bit little-

endian.

7 CRC-16 (Standard) Calculation of a CRC-16 using the polynomial:

### 2 15+214+27+26+20 ($C0C1)

8 CRC-16 (non-standard) This is a 16-bit checksum algorithm that can easily

implemented in a microcontroller. The used algorithm is as

follows:

CS = 0xffff;  // pre-initialize CS

Foreach 8-bit data byte do

Swap(CS)     // swap upper and lower bytes

CS = CS XOR data-byte

CS = CS XOR  ((CS AND 0xFF) SHR 4)

### CS = CS XOR  ((CS SHL 8) SHL 4)

CS = CS XOR (((CS AND 0xFF) SHL 4) SHL 1)

### Endeach

CS = NOT CS   // Inverse CS after operation

9 CRC-32 Calculation of the CRC-32 using the polynomial:

$77073096

10 SHA-1 Hash Algorithm Creatingf a 20-byte hash value based on the SHA-1



## Page 52

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

52 / 79

algorithm.

11 RIPEMD-160 Hash Algorithm Dto for RIPE-MD 160

12 Wordsum LE into 16-Bit, 2's Compl

BE-Out (GM new style)

Same as method 6, but the resulting 16-bit value will be

represented as 16-bit big-endian.

13 CRC-16 (CCITT) LE out 16-Bit CRC usi ng the non-reflected CCITT polynomial:

211 + 25 + 20   ($1021)

The function returns the 16-bit checksum in Little-Endian

format (low-byte first)

14 CRC-16 (CCITT) BE out Same as method 13, but result is in Big-Endian format.

Table 4-3: Functional overview of checksum calculation methods in “expdatproc.dll”

4.2.8 Run Data Processing interface (/ DPn:param[,section,key][;outfilename])

This option will run the data processing interf ace. This method is called right before the

data export commands are executed.

The parameter ‘n’ specifies the method. The value ‘n’ can be calculated in a similar way to

the checksum calculation method. The number can be found from the lis t box in the Edit-

>Run Data processing” option dialog. Count the number of entries in this dialog starting

from 0. The number of processing methods depends on the EXPDATPROC.DLL.

The data processing interface can take over a parameter. This parameter is separated by a

colon directly after the command line option.

### Example

HexView testfile.dat /DP1:CC

This option runs the second data proce ssing method in the list. It passes the

parameter string “CC” to the function.

### The EXPDATPROC that comes with this deliv ery of Hexview can manage the following

data processing methods:

Index Method Description Parameter2

0 No action Does no modification on the

data

-

1 XOR data with byte

parameter

### Runs XOR operation on the

data

### If no parameter is given, all data will

be inverted (XOR by 0xFF).

### Otherwise, it will run a byte-wise

operation with a HEX-string passed

as a parameter

2 AES-128 encryption Encrypts the data with the

AES-128 standard encryption

method

A 16 byte hex string

00112233445566778899aabbccddee

ff

3 AES-128 decryption Decrypts data with the AES-

128 method

A 16 byte hex string

00112233445566778899aabbccddee

2 The parameter can either passed as a HEX-string, or a filename can be passed that contains the HEX-

string. It is also possible to provide an INI-file with  section and keynames. The default output file can also

overwritten, if the method stores output data to an external file.



## Page 53

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

53 / 79

ff

4 HMAC (ANSI-X9.71) with

### SHA-1

### Creates a signature based

on Runs the HMAC using

### SHA-1.

### By default, the signature is

written to a file

signd_sha1.txt.

### The key-parameter as HEX-string or

an ASN-formatted string

### The ASN-string must be preceeded

by the tag bytes FF59 or FF5B

5 HMAC /w SHA-1 on

addr+len+data

### Creates a signature based

on HMAC using SHA-1

including the address and

length information for each

segment

### By default, the signature is

written to the file

signdal_sha1.txt.

### The key-parameter as HEX-string or

an ASN-formatted string.

### The ASN-string must be preceeded

by the tag bytes FF59 or FF5B

6 HMAC (ANSI-X9.71) with

### RIPEMD-160

### Creates a signature based

on HMAC using RIPEMD160

including the address and

length information for each

segment.

### By default, the signature is

written to the file

SignD_Ripemd160.HMAC.

### The key-parameter as HEX-string or

an ASN-formatted string.

### The ASN-string must be preceeded

by the tag bytes FF59 or FF5B

7 HMAC /w RIPEMD-160 on

addr+len+data

### Creates a signature based

on HMAC using

### RIPEMD160.

### By default, the signature is

written to the file

SignDAL_Ripemd160.HMAC

.

### The key-parameter as HEX-string or

an ASN-formatted string.

### The ASN-string must be preceeded

by the tag bytes FF59 or FF5B

8 RSA-Signature /w SHA-1

on data

### Creating the hash-value

using the SHA-1 algorithm

the data (only) for every

segment and encrypt the

result with the RSA

algorithm. By default, the

output is written to

SignD_SHA1.RSA.

### The private key as an ASN formatted

string. The string must be preceeded

by the tag FF49 or FF4B. The tag for

the exponent is 0x91 and the tag for

the modulo is 0x81.

9 RSA-Signature /w

RIPEMD160 on

Addr+Len+Data

### Creating the hash-value

using the RIPEMD160

algorithm on address, length

and data for every segment

and encrypt the result with

the RSA algorithm. By

default, the output is written

to

SignDAL_RIPEMD160.RSA.

### The private key as an ASN formatted

string. The string must be preceeded

by the tag FF49 or FF4B. The tag for

the exponent is 0x91 and the tag for

the modulo is 0x81.

10 RSA-Signature /w SHA-1

on Addr+Len+data

### Creating the hash-value

using the RIPEMD160

algorithm on address, length

and data for every segment

and encrypt the result with

the RSA algorithm. By

default, the output is written

to SignDAL_SHA1.RSA

### The private key as an ASN formatted

string. The string must be preceeded

by the tag FF49 or FF4B. The tag for

the exponent is 0x91 and the tag for

the modulo is 0x81.



## Page 54

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

54 / 79

11 AES-CBC Encryption 128-

Bit

### Encrypts the data with AES in

### CBC-mode using an

initialisation vector (IV).

By default, the IV will be set to 0. The

IV will be taken from the first 16 bytes

of the data stream. The data for the

### IV will be skipped for encprytion

operation.

12 AES-CBC Encryption 128-

Bit

Table 4-4: Functional overview of data processing methods in “expdatproc.dll”

With EXPDATPROC.DLL, V1.02, it is also possible to pass the parameters not only

directly but through a file or an INI-file. The parameter must be passed as follows:

Passing the parameter thorugh a file:

/DP:input-filename[;output-filename]

Passing the parameter through an INI-file:

/DP:input-filename,secti onname, keyname[;out-filename]

The INI-file has the format:

[sectionname]

keyname=’0011223344’

In every case, an output-filenam e can be optionally entered, preceeded by a “;”. This

output-filename will overwrite the default output filename.

The output is always written relative to the location of the Hex-File loaded by HexView.

4.2.9 Create error log f ile (/E:errorfile.err)

This specifies an error log file. HexView can run in silent mode (see 4.2.17). In that case,

no error will be displayed to the GUI. However, error messages are important to know. This

option allows to re-direct the output to a file.

4.2.10 Create single region file (/FA)

This option can be used to create a single blo ck file. In that case, HexView will use the

start address of the first block and the end address of the last bl ock and will fill all

remaining holes in-between with the fill character given with the /AFxx parameter.

Note that some files should be a single region file, e.g. the fl ashdrivers are not allowed to

have more than 1 region. This option can ensure that the file is a single region file.

4.2.11 Fill region (/FR:’range1’:’range2’:…)

This option is used to create and fill memory r egions. If the /FP parameter is not provided,

HexView will create random data to fill the blocks or regions. Otherwise, the value given by

the /FP parameter will be used repetitively. T he fill-operation does not touch existing data.

Thus, it can even be used to fill data between segments. Ranges are either specified by its

start and length, separated by a coma, or by  start and end address, separated by the

minus sign (e.g. /FR:0x1000,0x200:0x2000-0x2FFF).

4.2.12 Specify fill pattern (/FP:xxyyzz…)

This option can be used to specify a fill pattern that’s been used to fill regions. This option

is only useful in combination with the /FR pa rameter. The parameter for /FP is a list of

(see /FR option). The parameter will be treaded as a data stream in hexadecimal format.



## Page 55

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

55 / 79

4.2.13 Execute logfile (/L:logfile)

This option is intended to load a logfile comm and. Similar to a macro recorder, actions in

the GUI can be logged and later on re-execut ed using this command line option. Refer to

section 3.2.1.7 for further description).

4.2.14 Merging files (/MO, /MT)

One or more files can be merged into the inte rnal data memory of the program. The files

are read using the auto-detect file type mechanism described in chapter 3.2.1.2.1. The

commandline operation has some optional parameters to control the merge operation.

First, the type of merge operation need to  be chosen. The merge can done in a

transparent (/MT) or opaque (/MO) mode. Both cannot be mix ed. Only one can be chosen

in one commandline operation.

In the transparent mode, the l oaded filedata will not overwrite data in the internal memory.

The opaque mode does not check if data al ready exist and will load the data from the

merged file unconditionally. Already existing data may be overwritten.

Option extensions: file1[;offset][:’range’][+file2;offset][:’range’]

The filename must be followed directly to the option, separated by either a ‘: or the ‘=’ sign

(/Mx:file or /Mx=file). An optional offset parameter can be added. The offset can be positive

or negative, specified in hexadecimal or integer. In addi tion, a data range that’s been

loaded from the merge-file c an be specified. This can be gi ven with or without the offset.

Note, that the range will be applied on the un shifted data, then the address shift operation

will be applied.

Further files to merge can be added using the ‘+’ character to separate the next file to load.

### Example

/MT:cal1.hex;-0x1000+cal2.s19;128

HexView will merge the file “cal1.hex” with address offset -0x1000, then loads

“cal2.s19” with address offset 128. Existi ng address information  in the internal

memory will not be overwritten.

/MO:testfile.hex:0x2000-0x3FFF

Simply reads the address range from 0x2000- 0x3FFF from the file “testfile.hex”

into the memory. No offset will be added  or subtracted. Existing data on the

same address will be overwritten.

/MT:testfile1.hex;0x2000:0x1000,0x4000+cal2.s19;-0x3000:0x1000-0x1FFF

Merges the address range 0x1 000-0x4FFF of testfile1.hex and shifts all block

addresses of these ranges by the offset 0x2000. Afterwards, merges the address

range 0x1000-0x1FFF of f ile cal2.s19 and changes the block start addresses by

-0x3000.

Note: /MT and /MO cannot be combined in one commandline. Only the last in the

commandline-list will be used, in that case.



## Page 56

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

56 / 79

### Caution

### Since this operation can manipulate data in a post process, make sure HexView

creates the resulting file containing the desired data and applies the correct

changes..

4.2.15 Run postbuild operation (/pb=postbuild-file)

This option applies the postbu ild operation. This option r equires a valid PBUILD.DLL to

read the data from a postbuild file. The results will be applied to the internal document.

Originally, it is used to r ead the generated postbuild  XML-file using the PBUILD.DLL that

comes along with Hexview. However, it can also be used to appl y your own postbuild

configuration or to apply data changes to the currently loaded document.

The only pre-requisite is that the DLL provides the correct interface functions.

The DLL interface functions will be called in the following sequence:

OpenPBFile(Filename)

GetPBSegmentInfo(Address[], Length[],

maxNoOfSegments)

GetPBData(srcAddress, dstAddress,

length)

ClosePBFile( )

Figure 4-3: Calling sequence of the post-build  functions

The following function interface will be applied:

### OpenPBFile

### Prototype

Long __declspec(dllexport) __cdecl OpenPBFile  ( LPCSTR filename )

### Parameter

Filename Pointer to the location of the file that shall be opened. This is the full-path

of the file that has been selected in the file dialog when slecting the “Apply

postbuild options”.

### Return code

Long Number of segments found in the postbuild file and shall be applied to.

### Functional Description

Requests to open a file used for the postbuild operation process. Typically, it is the XML file generated by

GENy to apply the postbuild configuration data.

### Particularities and Limitations

 The function must return the number of segments that shall be applied to the postbuild operation



## Page 57

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

57 / 79

### ClosePBFile

### Prototype

Void __declspec(dllexport) __cdecl ClosePBFile  ( void )

### Parameter

- -

### Return code

- -

### Functional Description

Closes the previously opened file. Concludes all operations within the DLL.

### Particularities and Limitations

### GetPBSegmentInfo

### Prototype

Long __declspec(dllexport) __cdecl GetPBSegmentInfo  ( DWORD address[], DWORD

length[], long maxSegments )

### Parameter

### Address

### Length

### Long maxSegments

Pointer to a list of addresses. Will be filled by the operation.

Pointer to a list of length values. Each field for one segment. The index

corresponds to the address field.

Size of the fields where Address and Length points to. The interface

function shall not place more address and length information into the list as

specified by maxSegments (will exceeds internal data structures within

Hexview).

### Return code

### Long Number of segments found in the postbuild file and loaded to the segment

arrays of Address[] and Length[]..

### Functional Description

Provides all segments from the postbuild file that shall be loaded.-

### Particularities and Limitations

 The function must return the number of segments that has been loaded to the arrays.

 Segments provided in the list of address[] and length[] shall not overlap, length shall be greater than 0 in

all cases (otherwise, the element in the list should be omitted).

### GetPBData

### Prototype

Long __declspec(dllexport) __cdecl GetPBData  ( DWORD srcAddress, char

*dstBuffer, DWORD length)

### Parameter



## Page 58

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

58 / 79

srcAddress

### Length

### Long maxSegments

Pointer to the segment that shall be read. Corresponds to at least one of

the Addresses  of addresses. Will be filled by the operation.

Pointer to a list of length values. Each field for one segment. The index

corresponds to the address field.

Size of the fields where Address and Length points to. The interface

function shall not place more address and length information into the list as

specified by maxSegments (will exceeds internal data structures within

Hexview).

### Return code

Long Number of bytes read for post-building.

### Functional Description

Reads the segment data from the postbuild file and applies it to the current document.

### Particularities and Limitations

 The function must return the number of bytes read from the segment.

 The number of bytes read from the segment must correspond to the size previously specified for the

segment that belongs to the address given in the parameter.

4.2.16 Specify output filename (-o outfilename)

This option is used to overwrite the default output filename when exporting data to a file.

4.2.17 Run in silent mode (/s)

This option is used to suppress any output to the GUI. After executing all commands given

in the command line options, HexView will be closed.

4.2.18 Specify an INI-file for a dditional parameters (/P:ini-file)

Some output control functions require comple x parameters that cannot be given through

command lines. These output controls reads parameters from the INI-file. By default, if the

/P parameter is not given, HexView will extrac t the path and file information from the input

file and will search for the same file and locati on, but with the INI-extension. It will read the

contents from there. However, it could be useful to specify the IN I-file explicitly. This is for

example useful, if several output controls shall be used with the same parameters.

The path and filename for the INI-file must fo llow directly the /P parameter, but separated

either with a colon or an Equal sign. No blank character is allowed for separation or within

the file and path name.

### Example

/P:testfile.ini

HexView will read the data from  the path of the input file . If no explicit path is

used for the input file, HexView will search for the file in its current path.

/P=c:\testpath\testfile.ini

HexView reads the INI-file from the specified path and filename.



## Page 59

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

59 / 79

4.2.19 Remapping address information (/remap)

The remap option is used to shift the start addr ess of block. This can be useful to remap

several address blocks from physi cal to logical addresses. A us e-case for that is the re-

mapping of address spaces in banked mode to a contiguous linear address space3.

Figure 4-4: Mapping pysical to linear address spaces

The parameters to this option are as follows:

/remap:BankStartAddress-BankEndAddress,LinearBaseAddress,BankSize,BankIncrement

Figure 4-4 gives a reference to the parameters of the memory map. The BankStartAddress

and BankEndAddress spans a range of the me mory region, where the remap shall be

applied to. The LinearBaseAddress is the base address, wher e the first BankStartAddress

shall be mapped to. The BankSize is the maximu m size of a block that shall be remapped

and the BankIncrement is the difference of address between two banks, e.g. the difference

between BankStartAddress of bank #1 and BankStartAddress of bank #2.

Please note, that just blocks can be remapped,  that fits within the BankStartAddress and

BankEndAddress or multiples of BankIncrement. That is to say, only blocks with maximum

size of BankSize can be remapped. A conti nuous block section c annot be splitted and

3 Such linear address spaces are also called „virtual “ addresses, because the addr ess itself does cannot

directly used for a read operation on the micro. An addr ess calculation of the virtual address is necessary to

split it to a banked and a physical address.

### Bank start

address

### Bank end

address

Bank no.

#1

Bank no.

#2

Bank no.

#3

### Physical address space Virtual, linear address space

### Non-

banked

section #1

### Non-

banked

section #2

Bank no.

#1

Bank no.

#2

Bank no.

#3

„Peep-

Hole“

### Linear base

address

### Bank size

### Non-

banked

section #2

### Non-

banked

section #1



## Page 60

### User Manual HexView

©2009, Vector Informatik GmbH Version: 1.6

based on template version 1.9

60 / 79

remapped into linear addresses (this is not nece ssary. In that case, only the whole base

address of a block may be shifted).

The following example shows, how address shift operations are applied:

Assuming, the input file contains the following data sections:

Non-Banked addresses from 0x0000 – 0x7FFF.

Banked addresses:  0x018000-0x01BFFF; 0x028000-0x02BFFF.

In this example, the address mapping cons ists of a non-banked section and two bank

sections. The bank numbers are 0x01 and 0x02. The physical bank addresses are from

0x8000-0xBFFF.  The bank size is 0x4000.

The following option will remap the addresses to a linear address space:

/remap:0x018000-0x02B FFF,0x008000,0x4000,0x010000

This remaps the address space in the example above to 0x0000-0xFFFF.

4.2.20 Create validation structure

This item is used to create an information structure intended to be used for application

validation. It is typically used for flash download systems where it  is difficult or impossible

to determine if all elements necessary for a download are available and complete.

There are some flash download procedures, where it is impossible to verify if the download

is completed. For example, if partial do wnload is used without an information in the

download procedure, where the complete down load can be verified, or where a download

can be interrupted at a certain state that appears like a completed download.

For a successful usage of the validation stru cture, it is necessary, some important

precautions must be considered. To use the st ructure it is necessary to be able to re-

program it with every dow nload, even if it is just a partia l download. Before the validation

structure itself can be used, it is necessary  to determine if the va lidation structure is

present and complete. There are three options that can be used in  combination to verify if

the structure is complete. A magic value at the beginning and the e nd can be added to the

structure In addition, a simple byte checksum can be inserted that is added at the very end

to the structure.

The key information for the validation is the bl ock structure containi ng the segment start

address and length for each segment or block.  The data information is not only (and not

necessarily) taken from the internal data but also  from external files. A list of files can be

provided in the list blox. An  optional checksum per blo ck can be added. The checksum

method can be chosen from the available checksum methods from EXPDATPROC.DLL.

Instead or in addition to the block checksum a total checksum that is calculated over all

segment and block data can be added. The tota l checksum method can be different from

the block checksum.



> Note: this PDF has 79 pages; only the first 60 were extracted. See the original file `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/GM_C1XX_EPS_TMS570/Tools/HexView/ReferenceManual_HexView.pdf` for the remainder.

*Source PDF: `/workspaces/ElectricPowerSteering_TMS570_GM_C1XX/GM_C1XX_EPS_TMS570/Tools/HexView/ReferenceManual_HexView.pdf` — 79 page(s), text-extracted automatically.*
