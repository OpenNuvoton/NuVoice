-------------
NuAudioTool_V1.01.000 SP3
-------------
Based On NuAudioTool V1.01.000 SP3.

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

