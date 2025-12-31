----------
N572 SDS V6.00.000
----------
[Features]
+ Supports Eclipse IDE project located in "GCC" folders.
+ Updating MIDI library:
  - Speed up release stage when receiving a note on with the same note number that is already playing.
  - The release stage of a note off should continue upon reaching the end of the track.
+ Remove Audio libraries: NuVox_Ex.lib and NuLite_Ex.lib.
+ Remove Audio samples: NuVox53、NuVox63、NuLite、NuLiteEnc.
+ Remove stdDriver sample: SPI_Flash.
+ Remove USB samples: MSC_SDCard、MSC_SPIFlash.

----------
N572 SDS V5.05.000
----------
[Features]
+ Support "ARM Compiler" V6 project located in "KeilV6" folder.
+ Support "ARM Compiler" V5 project located in "KeilV5" folder.

[Bug-Fix]
+ Fix failure to determine the status at the end of SD card write command and lack read 2 bytes CRC in SD get chip info.

----------
N572 SDS V5.04.000 SP2
----------
[Features]
+ USB write tool supports "Windows 11".

----------
N572 SDS V5.04.000 SP1
----------
[Bug-Fixed]
+ Fixed bug about IR Carrier register bit.

----------
N572 SDS V5.04.000
----------
[Features]
+ Support N572H064.
  - All sample projects(Audio codec,Std driver etc).
  - Library.
  - Nulink downloader.
+ All audio library only verity PDID = 0x0b or 0x1d.

----------
N572 SDS V5.03.000 SP2
----------
[Bug-Fixed]
+ Fixed bug about playback hard-fault when NUONE & MIDI switch playback.
+ Fixed bug about playback channel control of the demo sample 'AudioPlayback'


----------
N572 SDS V5.03.000 SP1
----------
[Features]
+ Add definition about the 'mass storage protocol'.

[Bug-Fixed]
+ Fixed bug about the abnormal operation of the demo sample 'MSC_ImageWriter'.
+ Fixed bug about playback loop-play of the demo sample 'AudioPlayback'.
+ Fixed bug about parameters different between sysclk's header and source.

----------
N572 SDS V5.03.000
----------
[Features]
+ Revise all audio codec and voice effect demo samples to support high capacity size flash. 
+ StdDriver samples added “ConfigSysClk.h”, “SysClk” in projects for easier clock configuration.
+ Revise project's target order.

[Bug-Fixed]
+ Mic initial in N572F065 sereis would changes PA8~PA10 GPIO mode.

----------
N572 SDS V5.02.001
----------
[Features]
+ Powerdown.c be moved from framework folder into project folder. Powerdown features can be changed by application needs.
+ Fine tune power down procedure to reduce wake up time.
+ Support multi-pins trigger for GPIO wake up.

[Bug-Fixed]
+ Powerdown current decreased:
  - N572F072->8 ~ 12 μA.
  - N572F065->15 μA.
+ Voice effect added playback initiation.
+ Modify ADC stop procedure to avoid irregular current.
+ Update LP8, MD4, P16 decode library to fix handling silence problem.

[NOTE]
+ PreBuild.bat will not check audio tool version.  

----------
N572 SDS V5.02.000
----------
[Features]
+ Powerdown.c branced from framework layer. Powerdown feature will be set by application.
+ Adjust project setting of audio and vocie effect samples for powerdown.
+ Support multi-pins trigger for GPIO wake up.

[Bug-Fixed]
+ Modify "Lock"/"Un-Lock" checking scheme in driver layer.
+ Powerdown current decreased:
  - N572F072->8 ~ 12 μA.
  - N572F065->15 μA.
+ Voice effect added playback initiation.
+ Modify ADC stop procedure to avoid irregular current.

[NOTE]
+ PreBuild.bat will not check audio tool version.  
