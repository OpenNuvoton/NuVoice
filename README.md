----------
ICP tool, Nulink Keil driver and command tool 
----------
V7946r
1. Added supported microcontroller:
   – Nuvoton M0 Family: Nano100NC2BN, TX110VE3BN.
   – Nuvoton M23 Family: M2003G and KM1M2 series.
   – Nuvoton M33 Family: M3351 series.
   – Nuvoton M4 Family: N577 series.
   – Nuvoton M7 Family: KM1M7C series.
   – CM2052/CM2053 series.
2. Support Nu-Link2 V3.
3. Support Nu-Link3.
4. Nu-Link USB Driver update version to v1.12.

V7873b
1. Fixed an issue where the security bit set in offline mode could not be erased using the chip erase command on the I94100/I941A00 series.

V7872b
1. Add NSC family for NSC-related series
2. Renaming from ISD Series to Audio SoCs Series.

V7830
1. Support NSC23LA series.
2. Fix the problem that Offline mode cannot program files over 4KB.
3. Fix the N574 SPI Nor Flash >32MB can't program/erase and read issue.

V7829
1. Add N574E129 and N574F129 Series
2. Fix the N570H SPI Nor Flash >32MB can't program/erase and read issue.

V7724
1. Fix the NSC128L42 issue of incorrect flash size when no SPI Flash is connected.

V7715
1. Support NSC128L42 series.

V7694
1. Support chip N570H and N574F program high-capacity SPI Flash(Winbond W25Q01JV:1Gbits and W25Q02JV:2Gbits).
2. Fix Keil Driver N574F128 can’t change "Dowloand Function" and "Enable Flash BP" state in Flash download dialog.
3. Fix Offline program chip info shown on GUI for N572 chip series.

V7693
1. Support N574F129.
2. Fix fail to erase whole chip by manual when connect to ICP tool fail for N574F1K5
3. Fix fail to clear I94 config2 at erase whole chip for both online and offline mode.

V7624
1. Support offline mode to detect chip then program accordding to PDID.
   If PDID is unknown then program according to DID.

V7623
1. Remove NSC74128 supporting.
2. Fix semihosting can't free run problem.
3. Delete ICP tool SPIM interface from N574F1K5 series.
4. Fix ICP tool can't read SPI Flash with SPI0 for I91200 series.
5. Fix can't program data flash at off-line mode for N574 series.
6. Fix wait too long in erase verfiy stage at off-line for N574 series.

V7594
1. Delete "After performing "Erase Whole Chip Erase," check for non-FF values in the flash content."

V7593
1. Support N589 dongle off-line programing light signal at connect Nulink2 dongle MCU PB.7 to ground
2. Support log programming state to excel file (excel file location: "C:\Users\account_name\ProgramExcelLog\ICP Tool")
3. Fix N572 can't refresh SPI Flash status after select same SPI port.
4. Delete NSC74 SPIM Flash option.
5. Rename I9160/I9300/I91300 series SPI0 name from "SPI0(PA1, 0, 3, 4)" to "SPI0(PA1, 0, 3, 2)".

V7540
1. Fix can't erase/programing SPI Flash Device1/2 by N574/NSC74.
2. Fix show SPI flash size "2048MBytes" without SPI Flash.
3. Fix ISD9160 can't be programmed in batch mode from second run. 
4. Add N574 command line.

V7537
1. Support NSC74 chip series.
2. Support NSC74 SPI flash by SPI/SPIM(bypass mode).
3. Support N574 SPI flash by SPI/SPIM(bypass mode).
4. Fix can't erase/programing N574 SPI flash.

V7513
1. Support N574F chip series.
2. Support N574F SPI flash by SPI/SPIM.

V7444
1. Fix N570H064/N575F145 APROM is erased at enable erase whole chip and select external flash only.
2. Fix connect N570H064 but not detect SPI flash at SPIM ALT3_2 at first time.
3. Correct SPI flash menu options for each ISP chips

v7386
1. Fix set security bit but can't be erased with chip erase command on NuVoice/ISD chip series
2. Change these chip groups from "N569S/N569J" and "N570/N570S/N570J" to "N570F/N570S/N569S" and "N570H/N570J/N569J"
3. Set default SPI flash interface as "SPIM" for "N570F/N570S/N569S" chip series. 
4. Set default SPI flash interface as "SPIM ALT3_2" for "N570H/N570J/N569J" chip series.
5. Fix N570F menu [peripherals | system view | TMR] show all TIMER0~TIMER3 as TIMER0

v7384
1. Change SPI flash device setting(SPIM ALT3_2) for N570J/N570H

v7383
1. Fix N570 program internal flash fail if enable whole chip erase before program
2. Fix N570 offline programm fail
3. Set SPI flash device to SPIM ALT ALT3_2 for N570J

V7382
1. ICP tool supports N572H16A
2. Can select N572H064 device in keil project options

V7375
1. Support N572H064

V7274
1. Fix N572F065 can't be erased at security bit is locked.
2. Revise N574 reset debounce time in configuration register GUI
3. Support ZBit and Boya 16Mbits~64MBits SPI flash

v7175
1. Add I91500 and N574 series

v7084
ICP tool:
1. Add N569J spi flash option (same as N570H)
KEIL:
1. Add N569J device list cdb file and NuVoice_ISD_DFP pack v1.06

v7052
1. Fix data flash enable option of configuration dialog
2. Fix I96000 SPI flash offline download
3. Add SPI flash multi-channel offline download
4. Disable flash size checking while offline programming
5. Modify UI display of SPI flash programming condition
6. Add N569J and N570J

v7051
1. Popup SPI flash warning message when SPI flash size = 0 

v7013
ICPTool:
Keil:
1. Remove brown out voltage option and add LVR option for I91200 series
2. Support I96000 series

v6962
1. Support JNK561H part no.
2. Show SPI flash size to zero if SPI flash size value is abnormal.
3. Show warning message if programming bin file exceed SPI flash size of N571 series.
4. Add N570J and NPCA121 FLM SVD SFR Database
5. Update N570H SPI flash algo. file
6. Update software pack 1.04

v6951
ICPTool:
1. Fix I94000 offline download very slow

v6929b
ICPTool:
1. Fix N570 and I91200 offline download with Nu-Link2 in no SPI flash connection case
2. Blocking burning offline data to Nu-Link if file data size is greater than flash size
3. Add N570 and N570H 6 SPI device channel option
NuCMDTool:
1. Add I94000 SPI flash programming
2. Add N570 NAND flash programming
3. Add N570 and N570H 6 SPI device channel option

v6949
ICPTool:
1. Hide NAND option and modify NOR flash option UI for N570 and N570H series
Keil:
1. Update v1.0.3 ISD pack

v6928b
1. Fix I94000 and N570 offline download
2. Fix N570H LDROM erase and verify issue with chip erase case

v6927b
1. Support I94000 SPI flash
2. Support N570 NAND flash

v6911b
ICPTool:
1. Fix Nu-Link2 offline download
2. Support Nu-Link2 offline download SPI flash of NuLink2 for I94000 series

v6877b
ICPTool:
1. N570 LDROM 6K offline dowanload
2. Some N572 part no. connection problem (lock)
3. UI stuck while erasing APROM and SPI flash of N572 series
4. N572 SPI flash reading problem
5. N572S SPI flash size display for multi-cheannal
6. refresh SPI flash issue

v6876b
ICPTool:
1. base on v6875r + N572 offline SPI flash + N570H UCID

v6858
ICPTool:
1. Add mfc100.dll, msvcp100.dll and msvcr100.dll to installer
2. Fix offline download failed
3. Add NPCX series and update dll to V29 (b3 version)

v6846
ICPTool:
1. Update NuVoice Library dll v27
2. N572 OTP programFrom checkbox default value = false
3. Support Nu-Link2 direct programming SPI flash

v6836
ICPTool:
1. Add N570H SPIM flash algorithm
2. Update NuVoice Library dll v25
3. Support N570H
KEIL:
1. Support N570H
2. Update NuVoice Library dll v25
3. Update NuVoice database and SFR
4. Update NuVoice_ISD_Pack to v1.0.1

v6816
KEIL
1. Fix N570 can't set sofware breakpoint
2. Update NuVoice Library dll v24
ICPTool:
1. can get PDID from NuLibrary then use the default PDID
NuCMDTool:
1. Update NuVoice Library dll v24
2. N570H
v6815_DID
1. v6815 release1 + NuLibrary DID dll flow

v6785
Nu-Link command tool:
1. Add offline programming for N57x series
2. fix wrong SPI flash size with multi channel
3. Add direct programming SPI flash flow
4. Add N571 SPI flash programming
5. Add I94000 series part no. library
ICPTool tool:
1. fix wrong SPI flash size with multi channel
2. N571P032 part no. display

v6747
Nu-Link command tool:
1. Add offline programming with serial number for N570
2. NuLibrary test
3. fix spi flash verifying
4. fix update firmware stuck
ICP tool:
1. Modify default dialog size
2. Detect data flash size in offline download
3. NuLibrary test

v6726
Nu-Link command tool:
1. Add offline programming with limit count and password for N570

v6676
IAR:
1. Add I94000 ddf
KEIL:
1. Fix I9160 config programming
2. Disable Memory Verify Option
ICPTool:
1. Add I94000 special part no. (3/12 request)

v6675
1. Update N57x FLM file (256Mb SPI flash issue)

v6674
1. program offline data without connecting chip problem
2. taskbar block ICP tool dialog
3. Add IAR I91200 flash loader file
4. Add N569SCK2(SPI flash 256Mbits) and N570S256(SPI flash 256Mbits)
5. Add JNK561 series ICP tool

v6637
1. Add JNK561F064 (N570 series)
2. Support 2 SPI flash interfaces of N570 seriies ICP tool
3. Modify data flash display of I94000 series

v6636
1. Add N569S502, N569SAK2, N572U130, I94120ARI

v6635
1. New part (N569S, N570S, N572S, N575S)
2. Renew N572(S) SPI flash programming size 燒寫限制判斷
3. Fix N570S, I91000, I91200 flash page size incorrect and LDROM erase fail
4. Add new chip name
   New chip name of I91032: I91032C, I91032T
   New chip name of I91260: I91260B, I91260C, I91230, I91230C.
   New chip name of N570S, N569S, N572U
5. Add CRC32 function in loading file
6. I94000 config1 display
7. keep dialog size setting
8. Update N572 SPI flash algorithm file(Support high capacity and ext 32K clock)

v6613
1. Add Lock2 config bit of I94000 series
2. Add chip erase flow without connecting by using whole chip erase menu item
3. grayed the SPI flash option and button of I9200 series
4. disable N571 chip erase option
5. Add SPI flash size of special rule series
6. Fix SPI flash programming to use little-endian
7. fix offline download I94000 series
8. whole chip erase stuck problem
9. check file size before programming of I94000 series

v6609
1. Add I94000 new PID
2. N570 offline download
3. SPI flash size display
4. ISD series menu
5. KEIL FLM name compatible

v6570
1. Support I9200 series
2. new chip series group:NuVoice series including N570, N571, N572, N575, N576, I9000 series including I9000, I9100, I9200, I9300
3. N571E000 checksum is calculated from decrypted data not encrypted data
4. N570, N575/N576, I9000, I9100, I9200, I9300 series use little-endian data format.

