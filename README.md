---------------------
NuVoice Gang Writer V1.03.000 
---------------------
[Features]
+ Add "Whole Chip Erase" and "Program Config" option on new Gang Writer board
+ revise the UI position to fit the notebook size (1366x768)
+ update f/w file [M487_USBD_Mass_Storage_CDROM_Version_20210126.bin]
+ update supported series chip list (N569/N570/N572/N575/N570H/I94000/NPCx/N569J/N570J)
+ cancel to check and update firmware on new Gang Writer Board

[Note]
+ If the user need to update firmware for ne

---------------------
NuVoice Gang Writer V1.02.000 SP1
---------------------
[Features]
+ Delete the support temporary N570H series chip
  - N570J08/16/32/64 C
+ Support the by-pass mode on N570H series chip
  - N570J08/16/32 AL 
  - N570J04/08/16/32/64 DL 
  - N570J256/512/01 GR

---------------------
NuVoice Gang Writer V1.02.000
---------------------
[Features]
+ Support Chip Series: N569、N570、N575、I94000、NPCX、N570H
+ Pop "Current chip is not match with this board." warning message if selected old chip series(N569、N570、N572、N575) on the new board(I94000 & N570H)
+ Update firmware and code to support firmware code size is bigger more than 64k. (PS: Backward compatibility problem, the firmware need to use Nu-Link and ICP-Tool to write APROM first.)
+ Support I94000 and N570H series chip the erase, program, verify function

---------------------
NuVoice Gang Writer V1.01.003
---------------------
[Features]
+ Support JNK561F064 Chip

---------------------
NuVoice Gang Writer V1.01.002
---------------------
[Features]
+ Update F/W File

---------------------
NuVoice Gang Writer V1.01.001
---------------------
[Features]
+ Support N572F065 and N572U130 Configuration Setting

---------------------
NuVoice Gang Writer V1.01.000
---------------------
[Features]
+ Supported chips
  - N569S502,N569S1K0,N569S2K0,N569S4K0,N569S8K0,N569SAK2,N569S1K1,N570F064,
  - N570C064,N570S08A,N570S08B,N570S16A,N570S32A,N570S64A,N570S130,N570SC08,
  - N570SC16,N570SC32,N570SC64,N572F072,N572C072,N572F065,N572S08A,N572S16A,
  - N572S32A,N572S64A,N572U130,N575S64A
+ Update SPI-Flash ID
+ Use ChipProperty.cfg to load chip information

---------------------
NuVoice Gang Writer V1.00.000
---------------------
[Features]
+ Supported chips : N570S,N570SC,N570F,N570C,N569S,N572S,N575S
