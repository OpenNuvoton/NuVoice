------------
NuVoiceFormGen 
------------

----------
NuVoiceFormGen V1.03.021
----------
Based on NuVoiceFormGen_V1.03.020 and add the following issues
[Features]
1. Support N574E129

----------
NuVoiceFormGen V1.03.020
----------
Based on NuVoiceFormGen_V1.03.019 and add the following issues
[Features]
1. Support N574F129

----------
NuVoiceFormGen V1.03.019
----------
Based on NuVoiceFormGen_V1.03.018 and add the following issues
[Features]
1. Add N574 chip series support
 
----------
NuVoiceFormGen V1.03.018
----------
Based on NuVoiceFormGen_V1.03.017 and add the following issues
[Features]
1. Add chipitem N572H16A
 
----------
NuVoiceFormGen V1.03.017
----------
Based on NuVoiceFormGen_V1.03.016 and add the following issues
[Features]
1. Add chipitem N572H064
 
----------
NuVoiceFormGen V1.03.016
----------
Based on NuVoiceFormGen_V1.03.015 and add the following issues
[Features]
1. Add chipitem N575A145
 
----------
NuVoiceFormGen V1.03.015
----------
Based on NuVoiceFormGen_V1.03.014 and add the following issues
[Features]
1. N570J01GR's SPI flash size changed to 1004Mb.
 
----------
NuVoiceFormGen V1.03.014
----------
Based on NuVoiceFormGen_V1.03.013 and add the following issues
[Features]
1. Customer code of N570J01GR changed to N570J1GR.
2. Form file generated in unicode encoding to support naming file in different languages.

----------
NuVoiceFormGen V1.03.013
----------
Based on NuVoiceFormGen_V1.03.012 and add the following issues
[Features]
1. Add chip support list:
  - N569: N569SDK2
  - N570: N570S01G, N570F064L48, N570C064L48, N570H064L, N570HC64L
  - N572: N572F065G, N572C072G, N572F072G, N572P072G
  - N575: N575F145FI, N575C145FI
 
----------
NuVoiceFormGen V1.03.012
----------
Based on NuVoiceFormGen_V1.03.011 and add the following issues
[Features]
1. Add chip support list: 
  - N569J502L,N569J1K0L,N569J2K0L,N569J4K0L
  - N570J32AL,N570J04DL,N570J32DL,N570J64DL,N570J131GL,N570J256GR,N570J512GR,N570J01GR,N570J08DF,N570J16DF
 
----------
NuVoiceFormGen V1.03.011
----------
Based on NuVoiceFormGen_V1.03.010 and add the following issues
[Bug Fixed]
1. N570J08AL/N570J16AL/N570J08DL/N570J16DL should have embedded SPI flash.
 
----------
NuVoiceFormGen V1.03.010
----------
Based on NuVoiceFormGen_V1.03.009 and add the following issues
[Features]
1. Add chip N570FW64L,N570J08DL, N570J16DL
 
[Bug Fixed]
1. APROM size of N572S series should be 72K.
 
----------
NuVoiceFormGen V1.03.009
----------
[Features]
1. Add chip N570C12, N570HC64, N570J08AL, N570J16AL.

[Bug Fixed]
1. N570H064 LD ROM size should be 6K.

----------
NuVoiceFormGen V1.03.008
----------
Based on NuVoiceFormGen_V1.03.007 and add the following issues
[Bug Fixed]
1. Fix AP ROM size of N572P072.(#1838)
2. Data flash start address operation modified to be the same with ICP tool.(#1577)

----------
NuVoiceFormGen V1.03.007
----------
Based on NuVoiceFormGen_V1.03.006 and add the following issues
[Bug Fixed]
1. Size of embedded SPI flash was wrong which will cause file size checked incorrectly.
 
----------
NuVoiceFormGen V1.03.006
----------
Based on NuVoiceFormGen_V1.03.005 and add the following issues
[Features]
1. Add chip N570H064, N572C065

----------
NuVoiceFormGen V1.03.005
----------
Based on NuVoiceFormGen_V1.03.004 and add the following issues
[Features]
1. Add chip  N570B12
2. Keep file's original name in archive file
    
----------
NuVoiceFormGen V1.03.004
----------
Based on NuVoiceFormGen_V1.03.003 and add the following issues
[Feature]
1. Add chip JNK561F064
    
----------
NuVoiceFormGen V1.03.003
----------
Based on NuVoiceFormGen_V1.03.002 and add the following issues
[Features]
1. Remove I94 Series.
2. Allow user to select .rom file by default
3. Update document

[Bug Fixed]
1. Some new line character didn't show correctly if opened by notepad

----------
NuVoiceFormGen V1.03.002
----------
Based on NuVoiceFormGen_V1.03.001
[Features]
1. Make CRC32 and Checksum to be the same among main window, configuration dialog, form file and ICP tool.
2. Improve performance at startup.
3. Automatically open folder containing request form file after generated successfully.
4. Add user name/password dialog during installation and auto fill customer name in configuration dialog.
5. Multi-Level Chip Selection
6. N572 series chip compress .bin file to one 7z file.
7. Add I94 series, including I94124,I94123,I94121,I94120,I94114,I94113,I94111,I94110,I94134,I94133,I94131,I94130
8. For N572 series, add chips N572S08A,N572S16A,N572S32A,N572U130
9. For N570 series , add chips N570S08B,N570S130, remove chip N570SC04
10. For N569 series , add chips N569S502,N569S1K1,N569SAK2, remove chips N569S250,N569S500,N569S750,N569S1K5,N569S3K0
    
[Bug Fixed]
1. Fix : split button cannot be shown in WinXP.
 
-----------
NuVoiceFormGen V1.03.001
----------
Based on NuVoiceFormGen_V1.03.000
[Features]
1. Add M4 series, including I94124,I94123,I94121,I94120,I94114,I94113,I94111,I94110,I94134,I94133,I94131,I94130
2. For N572 series, add chips N572S08A,N572S16A,N572S32A,N572S08B,N572S16B,N572S32B,N572S64B,N572U08A,N572U16A,N572U32A,N572U64A,N572U128,N572U08B,N572U16B,N572U32B,N572U64B,N572U129
3. For N570 series , add chips N570S04A.N570S128,N570S04B,N570S08B,N570S16B,N570S32B,N570S64B,N570S129,N570S130,N570SCA2,N570SC05,N570SC09,N570SC17,N570SC33,N570SC65,N570SCA3
4. For N569 series , add chips N569SAK0,N569S251,N569S501,N569S751,N569S1K1,N569S1K6,N569S2K1,N569S3K1,N569S4K1,N569S8K1,N569SAK1,N569SAK2
5. For N575 series, add chips N575S08A,N575S16A,N575S32A,N575S08B,N575S16B,N575S32B,N575S64B
6. N572 series chip compress .bin file to one 7z file.

----------
NuVoiceFormGen V1.03.000
----------
Based on NuVoiceFormGen_V1.02.003
[Features]
1. Add Chips
   - For N572 series : N572S64A
   - For N570 series : N570S08A,N570S16A,N570S32A,N570S64A,N570SC04,N570SC08,N570SC16,N570SC32,N570SC64
   - For N569 series : N569S250,N569S500,N569S750,N569S1K0,N569S1K5,N569S2K0,N569S3K0,N569S4K0,N569S8K0
   - For N575 series : N575S64A
    
----------
NuVoiceFormGen V1.02.003
----------
Based on NuVoiceFormGen_V1.02.002
[Bug Fixed]
1. For N572 series chip, add r2 information in form file.
 
----------
NuVoiceFormGen V1.02.002
----------
[Bug Fixed]
1. Change behavior to always pad 0xFF in the end of the file if ROM is not full.
2. Checksum doesn't update correctly.
3. Allow specify data flash base address without specifying data flash file.
4. Change Icon
    
----------
NuVoiceFormGen V1.02.000
----------
[Bug Fixed]
1. Allow user to set data flash base address in 512 bytes alignment for N570
 
----------
NuVoiceFormGen V1.01.000
----------
[Features]
1. Supported chips : N572F072,N572C072,N572P072,N572F065,N570F064,N570C064,N575F145,N575C145
2. Add NuVoiceFormGen user guide.
3. Add option to pad or not if APROM is not full
    
