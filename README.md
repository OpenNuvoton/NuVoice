-------------
NuAudioTool_V1.01.006
-------------
Based on NuAudioTool V1.01.000 SP5.

[Features]
+ Support for per-file Addressable LED sample frequency setting according to "UioSampleFrequency.cfg".
  - Reference document section "Individual UltraIO Curve Sampling" for more information.
+ Clean up temporary .sld and .sldp files after ROM generation

[Bug Fixes]
+ Fixed an issue where converting WIO files containing ALED data could cause abnormal termination due to conversion failures
+ Fixed an issue where the build process could fail when ALED was enabled but no ALED data was present in the WIO file

-------------
NuAudioTool_V1.01.005
-------------
Based on NuAudioTool V1.01.000 SP4.

[Features]
+ Added support for individual UIO curve sample configuration
  - MUST create UioSampleFrequency.cfg and place it in the same project folder with NuAudio Project file.
+ Added support for setting a default wavetable
+ Added support for Ultra IDT timbre table files
+ Added MP3 format support in the Resource window
+ Added support for configuring the resampling rate of speech audio in the Resource window
+ Added support for copying Debug and Output messages to the clipboard via the right-click context menu
+ Updated the list of supported audio file extensions in the Resource window

[Bug Fixes]
+ Fixed a crash issue caused by excessively long ‘defequ’ strings in .uid file
+ Fixed a crash issue caused by excessively long input strings in the Equation Editor

-------------
NuAudioTool_V1.01.004
-------------
Based On NuAudioTool V1.01.000 SP3.

[Features]
+ Support General chip across the General series
+ Support for opening the UltraIO Setting and Addr. LED Setting pages independently
+ Support for N574F129 chip

[Bug Fixes]
+ The mapping of pitch names and values should be adjusted based on the Middle C setting during IDT file reading
+ Fixed crash issue when importing a UID file containing unsupported format information

-------------
NuAudioTool_V1.01.000 SP3
-------------
Based On NuAudioTool V1.01.000 SP2.

[Features]
+ Support for NSC128L42, N577F512, and N577C512 chips
+ Support for command-line parameters to build resources using a selected AudioTool version
+ Support for color palette mode in the SLED Settings window
+ Modify resource and equation of EXT column support Internal, data flash and external flash

[Bug Fixes]
+ Fixed issue where playing a "wax" file failed in the MIDI Wave Table window
+ Fixed issue where disabled instrument or drum items disappeared when switching from Text mode to UI mode in the MIDI Wave Table window
+ Fixed issue where disabled resource or equation items disappeared when switching from Text mode to UI mode in the Resource window
+ Fixed issue where the bitrate of MD4 format resources should not be generated into the UID


-------------
NuAudioTool V1.01.000 SP2
-------------
Based On NuAudioTool V1.01.000 SP1.
[Bug Fix]
+ fail to open UltraIO to edit on resource window
+ fail to preview resource and equation on resource window

-------------
NuAudioTool V1.01.000 SP1
-------------
Based On NuAudioTool V1.01.000.

[Features]
+ delete chip NSC74128

-------------
NuAudioTool V1.01.000
-------------
Based On NuAudioTool V1.00.000 SP2.

[Features]
+ Support chip NSC74128/NSC74256/NSC74512/NSC741K0/NSC741K5
+ Create "C:\Nuvoton\NuAudioTool\Workbench" to map current install folder
+ Support command mode to build [*.nat] project using for Keil project post-build
  - example:
    "C:\Nuvoton\NuAudioTool\Workbench\Bin\NuAudioTool.exe" ".\NuProj.nat" -rebuild
    "C:\Nuvoton\NuAudioTool\Workbench\Bin\NuAudioTool.exe" ".\NuProj.nat" -build

-------------
NuAudioTool V1.01.000
-------------
[Features]
+ support to edit audio resources, equations, and related global setting in resource window
+ support to edit instruments, drums, and related global setting in MIDI wave table window
+ support the UID and IDT text editor like AudioTool
+ support UltraIO setting
+ support addressable LED setting
+ support build/rebuild/stop build project functions
+ support new the project management function
  - Import project
  - Duplicate project
+ support project name in multi-langue
+ support folder name in multi-langue
+ support long project and folder name

