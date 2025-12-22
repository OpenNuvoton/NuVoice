-----------
N574 SDSV1.06.000 SP1
-----------
[Features]
+ Updating MIDI library:
  - Speed up release stage when receiving a note on with the same note number that is already playing.
  - The release stage of a note off should continue upon reaching the end of the track.

-----------
N574 SDSV1.05.000
-----------
[Features]
+ Support "ARM Compiler" v6 project located in "KeilV6" folder.
+ Support "ARM Compiler" V5 project located in "KeilV5" folder.
+ Rename SPI0 and I2C0 to SPI and I2C.
+ Remove DPD from clock driver and stdDriver\PMU_DPD sample.
+ Remove stdDriver\SYS_OscTrim sample.

[Bug-Fixed]
+ For stdDriver\PMU,BOD and SYS samples, will cause hard fault if return from main().
+ For keypad library, fix matrix key Port C not work problem.

-----------
N574 SDSV1.04.000 2023/12/12
-----------
[Features]
+ Support N574F128
+ New driver samples - SPIM_Master, SPI_Slave_SPIM_Master, SPIMFlash
+ Add Warning massage to inform about correct ADC MICBIAS init flow
+ New ADC_MIC_Init() function to execute correct ADC MICBIAS init flow
+ Rename UART register name from UMODE to MODE
+ Rename ADC register name from PGATL to PGCTL
+ Only "reference AVDD" option for ADC MIBIAS
+ Modify AudioCodec Samples to use NuAudio Tool
+ Modify regsiter function descriptions in N574.h

[Bug-Fixed]
+ For BOD sample, should clear NVIC IRQ before enable BOD interrupt.

-----------
N574 SDSV1.03.000
-----------
[Features]
+ Add SampleCode\StdDriver\I2C_Master.
+ Add SampleCode\Storage and driver.
+ Remove Select Target "N574F512".
+ Remove SampleCode\StdDriver\AED_WakeUp.

[Bug-Fixed]
+ N574F1K5 has the timer clock source will disappear sometimes.
  - Add enable 32KHz XTAL Oscillator then disable 32KHz XTAL Oscillator at chip reset.("\Library\Device\Nuvoton\N574\Source\system_N574.c")
+ SampleCode\AudioCodec can't power dowm.

-----------
N574 SDSV1.02.000
-----------
[Features]
+ Add 'Power Script' function.(framework & demo samples)
+ Remove 'AED' function.(driver & demo samples)
+ Refine the FMC's read/write process in the Codec demo samples.(without setting CONFIG)
+ Codec libraries check via FMC's CID.

-----------
N574 SDSV1.01.000
-----------
V1.01.000 Release.