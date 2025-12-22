----------
N575 V5.05.000
----------
[Features]
+ Support "ARM Compiler" V6 project located in "KeilV6" folder.
+ Support "ARM Compiler" V5 project located in "KeilV5" folder.

----------
N575 V5.04.000
----------
[Add]
+ Update NuOneEx library(Format 0xA0 & 0xA2)
  - Reduce rom & ram size.
  - New library could backward compatible older version.
  - Add NuOneEx's equation-mode & list-play support new nuoneex format(0xA0,0xA2) in NuOneEx demo sample.
  - Add AudioPlayback demo sample support new nuoneex format(0xA0,0xA2).
+ Update MD4 library
  - Provide user API 'MD4_JumpToSecond' to jump seconds when audio playing.
  - Reduce MD4 work buffer.
+ Revise power-down process in all audio codec & voice effect demo samples.
+ Update Midi library -
  - Optimization for reduce ROM & RAM size and better computing.
  - Fixed some noise bug.
  - Fixed bug about MIDI library set volume value.
  - Refine APIs to make same with other codec(via working buffer, like NuOneEx,NuSoundEx etc)   
+ Add 'AudioPlayback' demo sample to show how to play audio in multi-channels.
  - Support New NuOneEx format(0xA0 & 0xA2).
+ Add Wrap interrupt & SoftReset API in PDMA's driver.
+ Update BNDetection library - 
  - Provide user new APIs.
  - Reduce work buffer used.
  - Fixed some issue.
+ Add EVO demo samples in Samples/AudioCodec.
   
[Bug-Fixed]
+ Revise SPIFlash initiate process to make sure SPIflash stable.
  - Audio Codec demo samples.
  - Voice effect demo samples.
  - Storage/SPIFlash demo sample.
+ Revise Playback & Recode process to synchronize N570 & N572 SDS.
  - Buffer control.
  - Playback interrupt process(one and multi channel).
  - Record interrupt process.
  - Fixed playback ussye abour dont provide change volume in pause state.
+ Modify "Nu_Link_Driver.ini" to configurate full chip erase in all demo samples.
+ Fixed bug about sample over counts in AudioMixer after making up samples.
+ Revis startup files in all samples to fix WIC state doesn't synchronize with NVIC when M0 is in standby domain.
 