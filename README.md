----------
N570 SDS V5.02.000 SP2
----------
[Features]
+ Updating MIDI library:
  - Speed up release stage when receiving a note on with the same note number that is already playing.
  - The release stage of a note off should continue upon reaching the end of the track.

----------
N570 SDS V5.02.000 SP1
----------
[Features]
+ Supported quad mode SPI flash for SPIM interface: W25Q128FV and W25Q256FV.
+ Add \SampleCode\Storage\SDCard sample.

[Bug-Fixed]
+ Fix SD Card get info problem.
+ Fix SD Card failure to accurately determine the status at the end of the write command leads to an infinite loop in subsequent read commands.
+ Fix sample SPIFlash project, ASM define from N570F064 to N570H064.
+ Fix .uid file for AudioCodec samples .

----------
N570 SDS V5.02.000
----------
[Features]
+ Support "ARM Compiler" V6 project located in "KeilV6" folder.
+ Support "ARM Compiler" V5 project located in "KeilV5" folder.

----------
N570 SDS V5.01.000 SP7
----------
[Features]
+ Support "N570HC64" "N570J08AL" and "N570J16AL" on audio library.
+ Support dual and quad mode on SPIMFlash library.
+ Suuport NAND flash on AudioCode samples.
+ Revise SPIMFlash_NAND Bad Block management
+ Revise audio playback sample hang up at playing some MD4 file.
+ Add "SampleCode\Keypad\TouchKey_Wakeup" demo sample to supprot wakeup chip via cscan pin.

[Bug-Fixed]
+ Fixed Systick issue.
+ Change SPI_Master and SPI_Master_PDMA sample to use 1MHz SPI clock not 100KHz SPI clock.
+ ISP_UART update APROM will erase data in dataflash.
+ ISP_UART sample project setting not choose corret debugger.
+ TIMER_Open frequency setting has incorrect result.
+ AudioCodec samples sets wrong address mode when using 128M SPI-flash.
+ N570H needs pull-up mode setting in GPIO.
+ AudioPlayback sample has issue with equation loop.
+ Use TIMER_Open to set 200K frequency but the final frequency is incorrect.
+ SPI_SetBusClock & SPI_SetVarClock can not set to the highest possible clock rate.
+ Fixed bug about playback hardfault when NUONE & MIDI switch playback.
+ Fixed bug about playback channel control of the demo sample 'AudioPlayback'

[Note]
+ The revised SPI-Flash library can be used separately. Calling SPIMFlash
  - API does not need to add SPIFlash.c into project.
+ Recommend to predefine SPIFlash bit mode in project setting at using SPIMFlash.c.
  - Please add the following definition in 'Project'->'Options for target'->'C/C++'->'PreProcessor Symbols'->'Define'
     * SPIFLASH_INTERFACE_MODE - 0 // One-bit Mode
     * SPIFLASH_INTERFACE_MODE - 1 // Dual Mode
     * SPIFLASH_INTERFACE_MODE - 2 // Quad Mode
  - Supported quad mode SPI flash for SPIM interface: W25Q16BV, W25Q16DVS, W25Q64DW
+ If using NAND flash in AudioCodec samples, please set SPIMFlash_NAND - 1 in the project setting pre-define.
  - In beginning of the header files of SPIFlash and SPIMFlash, there are description of how to define the setting.

----------
N570 SDS V5.01.000 SP6
----------
[Features]
+ Add "SampleCode\Keypad\TouchKey_Wakeup" demo sample to supprot wakeup chip via cscan pin.

----------
N570 SDS V5.01.000 SP5
----------
[Features]
+ Revise SPIMFlash_NAND Bad Block management
+ Revise audio playback sample hang up at playing some MD4 file.

[Bug-Fixed]
+ Use TIMER_Open to set 200K frequency but the final frequency is incorrect.
+ SPI_SetBusClock & SPI_SetVarClock can not set to the highest possible clock rate.

----------
N570 SDS V5.01.000 SP4
----------
[Bug-Fixed]
+ TIMER_Open frequency setting has incorrect result.
+ AudioCodec samples sets wrong address mode when using 128M SPI-flash.
+ N570H needs pull-up mode setting in GPIO.
+ AudioPlayback sample has issue with equation loop.

----------
N570 SDS V5.01.000 SP3
----------
[Features]
+ Revise SPIMFlash library.
+ Revise AudioCodec samples for NAND flash support.
+ Revise Framework SPIFlashUtil for NAND support.

[Bug-Fixed]
+ ISP_UART update APROM will erase data in dataflash.
+ ISP_UART sample project setting not choose corret debugger.

[Note]
+ If using NAND flash in AudioCodec samples, please set SPIMFlash_NAND - 1 in the project setting pre-define.
+ In beginning of the header files of SPIFlash and SPIMFlash, there are description of how to define the setting.

----------
N570 SDS V5.01.000 SP2
----------
[Features]
+ Revise SPIMFlash library and samples to support dual and quad mode

[Bug-Fixed]
+ Change SPI_Master and SPI_Master_PDMA sample to use 1MHz SPI clock not 100KHz SPI clock.

[Note]
+ The revised SPI-Flash library can be used separately. Calling SPIMFlash
   API does not need to add SPIFlash.c into project.
+ Recommend to predefine SPIFlash bit mode in project setting at using SPIMFlash.c.
  - Please add the following definition in 'Project'->'Options for target'->'C/C++'->'PreProcessor Symbols'->'Define'
    * SPIFLASH_INTERFACE_MODE - 0 // One-bit Mode
    * SPIFLASH_INTERFACE_MODE - 1 // Dual Mode
	* SPIFLASH_INTERFACE_MODE - 2 // Quad Mode
  - Supported quad mode SPI flash for SPIM interface: W25Q16BV, W25Q16DVS, W25Q64DW

----------
N570 SDS V5.01.000 SP2
----------
[Update]
+ Revise SPIMFlash library and samples to support dual and quad mode

[Fix]
+ Change SPI_Master and SPI_Master_PDMA sample to use 1MHz SPI clock not 100KHz SPI clock.

[Note]
+ The revised SPI-Flash library can be used separately. Calling SPIMFlash
   API does not need to add SPIFlash.c into project.

+ Recommend to predefine SPIFlash bit mode in project setting at using SPIMFlash.c.
  - Please add the following definition in 'Project'->'Options for target'->'C/C++'->'PreProcessor Symbols'->'Define'
	* SPIFLASH_INTERFACE_MODE - 0 // One-bit Mode
	* SPIFLASH_INTERFACE_MODE - 1 // Dual Mode
	* SPIFLASH_INTERFACE_MODE - 2 // Quad Mode
  - Supported quad mode SPI flash for SPIM interface: W25Q16BV, W25Q16DVS, W25Q64DW

----------
N570 SDS V5.01.000 SP1
----------
[Revise]
+ Revise "N570F.h" to fix Systick issue.
+ Revise Audio library for "N570HC64", "N570J08AL", and "N570J16AL".

----------
N570 SDS V5.01.000
----------
[Features]
+ N570H064 supported driver and demo samples.

[Bug-Fixed]
+ Revise DPWM & DPWM_DAC demo sample to resolve issue about noise at ending section.
+ Revise HW register naming(in N570F.h/N570H.h) to synchronous TRM.
+ Fixed NuOneEx library issue about API 'NuOneEx_EndEncode' didnt restore recording size. 
+ Fixed encode libraries's(NuOneEx/NuLiteEx/ImaAdpcm) volume smaller issue. 

----------
N570 SDS V5.00.001 SP8
----------
[Revise]
+ Revise "SoftI2C.c" and "SoftI2C.h" to work in Timer and GPIO interrupt.
+ Revise "SoftI2C_Master" and "SoftI2C_Slave" sample code to match the new driver.
+ Revise "N570.h". Add hardware register for PDMA backward compatible.

----------
N570 SDS V5.00.001 SP7
----------
[Features]
+ Add "sp version.txt" file in SDS folder to provide user know current service packet's version.
+ SPIMFlash library support high capacity function(>-128Mbits).
+ Revise all audio codec and voice effect demo samples to support high capacity size flash. 

[Bug-Fixed]
+ Revise DPWM & DPWM_DAC demo sample to resolve issue about noise at ending section.
+ Fixed PDMA HW register bits name(in N570.h) to synchronous TRM.
+ Revise SPI_Master_PDMA/SPI_Slave_PDMA/PDMA StdDriver demo samples to fit redefinition HW register and make user more readable .
+ Fixed NuOneEx library issue about API 'NuOneEx_EndEncode' didnt restore recording size. 
+ Revise GPIO demo sample to call GPIO APIs synchronous with N572.
+ Fixed encode libraries's(NuOneEx/NuLiteEx/ImaAdpcm) volume smaller issue because N570 ADC input PCM is 13 bits. 

----------
N570 SDS V5.00.001 SP6
----------
[Features]
+ Update NuOneEx library to add A2 format.
+ Add speaker output to DAC(in ConfigIP.h to configurate).
+ Add EVO demo samples in Samples/AudioCodec.
+ Add SoftI2C driver & demo samples(include master & slave).

[Bug-Fixed]
+ Revise MD4 library for reduce MD4 work buffer.
+ Revise SYS demo sample(feedback from RW).
+ Revise project setting of audio-codec & voice-effect demo samples to full APROM '0xFF'.
+ Modify "Nu_Link_Driver.ini" to configurate full chip erase in all demo samples.
+ Fixed bug about FIFO threshold API in DPWM.h.
+ Revise DPWM demo sample.

----------
N570 SDS V5.00.001 SP5
----------
[Features]
+ Update NuOneEx library to reduce rom & ram size.
  - New NuOneEx format type is 0xA0 & 0xA1
  - New library could backward compatible older version.
  - Add NuOneEx's equation-mode & list-play support new nuoneex format(0xA0,0xA1) in NuOneEx demo sample.
  - Add AudioPlayback demo sample support new nuoneex format(0xA0,0xA1).
+ Add MD4 library's API 'MD4_JumpToSecond' to provide user jump data.
+ Add NHS-570F064-EVB_V0.3_UserGuide_EN_A3.1.pdf to provide user reference.

[Bug-Fixed]
+ Fixed bug about SPIMFlash process of waiting stable. 
+ Revise WDT demo sample. 
+ Fixed bug about MIDI library set volume value.

----------
N570 SDS V5.00.001 SP4
----------
[Features]
+ Add correct process about power-down into every audio codec & voice effect demo samples.
+ Add all user guild(*.chm), include: codec demo samples, driver reference, library reference, voice effect demo sample, NuVoice sample framework.
+ Add Uart function
  - Add uart driver to control ip interface.
  - Add clock enable module to enable/disable uart clock source.
  - Modify N570.h to add uart hardware ip register control.
  - Make std driver demo sample for user.
  - No Support revA chip.
  - FIFO trigger driver APIs.
+ Add DPWM DAC control driver APIs
+ Add OSCFM hardware register definition & driver & reference guild.
+ Add Keypad demo sample
  - Trigger key demo sample.
  - Matrix key demo sample.
+ Update Midi library -
  - Optimization for reduce ROM & RAM size and better computing.
  - Fixed some noise bug.
  - Refine APIs to make same with other codec(via working buffer, like NuOneEx,NuSoundEx etc)   

[Bug-Fixed]
+ Modify Appfunction in "AudioPlayer demo sample" to fix bug which is playing list audio id fail(function return value wrong).
+ Rollback midi library & MidiSynther demo sample to be same with other chips(N575,N572 etc
+ Cancel full APROM to '0xFF' in 'project setting' of audio-codec & voice-effect demo samples.
+ Modify audio playback clip value in one channelto fix 'pop' sound when volume adjust to 'eVOLUMETRL_VOLUME_10_DB'.
+ Modify audio application(MD4Appc,L8pApp.c etc) about fill up PCM value when decode data wasnt fit a frame to fix 'pop' sound in end frame.
+ Update 'Application_Keil.ld' in all demo samples to fix 'C3912W: Option 'device' is deprecated' warning
+ Fixed bug about sample over counts in AudioMixer after making up samples.
+ Fixed bug about playback will not provide change volume in pause state.
+ Modify hardware register definition about deep power-down. 

----------
N570 SDS V5.00.003 SP3
----------
[Features]
+ Add correct process about power-down into every audio codec & voice effect demo samples.
+ Add all user guild(*.chm), include: codec demo samples, driver reference, library reference, voice effect demo sample, NuVoice sample framework.
+ Add Uart function
  - Add uart driver to control ip interface.
  - Add clock enable module to enable/disable uart clock source.
  - Modify N570.h to add uart hardware ip register control.
  - Make std driver demo sample for user.
  - No Support revA chip.
  - FIFO trigger driver APIs.
+ Add DPWM DAC control driver APIs

[Bug-Fixed]
+ Modify Appfunction in "AudioPlayer demo sample" to fix bug which is playing list audio id fail(function return value wrong).
+ Rollback midi library & MidiSynther demo sample to be same with other chips(N575,N572 etc
+ Cancel full APROM to '0xFF' in 'project setting' of audio-codec & voice-effect demo samples.
+ Modify audio playback clip value in one channelto fix 'pop' sound when volume adjust to 'eVOLUMETRL_VOLUME_10_DB'.
+ Modify audio application(MD4Appc,L8pApp.c etc) about fill up PCM value when decode data wasnt fit a frame to fix 'pop' sound in end frame.

----------
N570 SDS V5.00.002 SP2
----------
[Features]
+ Add correct process about power-down into every audio codec & voice effect demo samples.
+ Add all user guild(*.chm), include: codec demo samples, driver reference, library reference, voice effect demo sample, NuVoice sample framework.
+ Add Uart function
  - Add uart driver to control ip interface.
  - Add clock enable module to enable/disable uart clock source.
  - Modify N570.h to add uart hardware ip register control.
  - Make std driver demo sample for user.
  - No Support revA chip.

[Bug-Fixed]
+ Modify Appfunction in "AudioPlayer demo sample" to fix bug which is playing list audio id fail(function return value wrong).
+ Rollback midi library & MidiSynther demo sample to be same with other chips(N575,N572 etc
+ Cancel full APROM to '0xFF' in 'project setting' of audio-codec & voice-effect demo samples.

----------
N570 SDS V5.00.001 SP1
----------
[Features]
+ Add correct process about power-down into every audio codec & voice effect demo samples.
+ Add all user guild(*.chm), include: codec demo samples, driver reference, library reference, voice effect demo sample, NuVoice sample framework.
+ Add Uart function
  - Add uart driver to control ip interface.
  - Add clock enable module to enable/disable uart clock source.
  - Modify N570.h to add uart hardware ip register control.
  - Make std driver demo sample for user.

[Bug-Fixed]
+ Modify Appfunction in "AudioPlayer demo sample" to fix bug which is playing list audio id fail(function return value wrong).
