All installers are zipped with password: 123456
-------------
N589 SDS V1.08.000 SP6
-------------
[Features]
+ PS compiler add function to check lib labels to ensure that kernel related labels will be allocated in bank 0.
+ FW Librart: Remove wake-up call PREPARE_FOR_SLEEP callback function. (only calls before entry STOP)

-------------
N589 SDS V1.08.000 SP5
-------------
[Features]
+ Support N589B345/B255/B205/B175/B125/B085 chips. 
+ Support NSD support loop + silence compression simultaneously. 

[Bug-Fixed]
+ Can’t build larger number of resource files due to string library bug
+ PS "call" command will have the chance to return to wrong location
+ Can’t use concatenation character ('\') to break PS command into several lines

-------------
N589 SDS V1.08.000 SP4
-------------
Based On N589_V1.08.000 SP3 and add the following issue
[Features]
+ Update Cap Touch library.
    Add cap key disable/enable function in normal mode.
    Add PS instructions for Enable/Disable cap touch keys.
    Add auto clear cap key status function.
    Add manual clear cap key status macro.
+ NSS/NSP support loop + silence compression simultaneously.
+ Add Rum-Time Envelope functions.
+ Add HWPWM control for C.
+ Disclose N589ABCD ROM size.
+ Create pre-code data after build project.
+ Programmable IR Parity. 
+ Add functions to control synthesizer.
+ N589E: SOP8 I/O pin number changed to 3.
     
[Bug-Fixed]
+ Resources added to resource window always be set as 16000 resample rate.
+ NSP decoder in PC(Rbf2Wav.exe) do not need to left shift 3 bits.
+ Correct N589ABCD I/O pin information of chip selector.
+ N589E: Direct trigger key should be pressed twice to get response after  executing "LD EN, OFF". 
+ N589E: HW PWM do not work after wakeup. 
+ N589E: Fix random bug.

-------------
N589 SDS V1.08.000 SP3
-------------
Based On N589_V1.08.000 SP2 and add the following issue
[Bug-Fixed]
+ MaskOption always be set to default after user changed.
+ Fix the issue that Ultra-IO Init/Stop value affects CapTouch wakeup pin change for ASM project.
+ Detect UltraIO event count in one frame and report error if overflow to avoid running hard fault at run-time for N589ABCD

-------------
N589 SDS V1.08.000 SP2
-------------
Based On N589_V1.08.000 SP1 and add the following issue
[Features]
+ Add addressable LED Power Script instructions.

[Bug-Fixed]
+ Cannot select 7 Output Pin when Direct Trigger is 1.
+ Fix Ultra-IO IO Init value issue for Assembly project.

-------------
N589 SDS V1.08.000 SP1
-------------
[Features]
+ IR wakeup without IR Tx/Rx function
+ Add check to LRC wakeup timer of PS instruction. If the time is not multiple times the length of 6.25ms, it shows error.
+ NSS codec format support loop mode.
+ Add support of overlapped channel playback. User can play midi file with 12 polyphony.
+ New C samples: PlaybckSpeech, PlaybackMIDI, PitchChanger, ColorFlyer

[Bug-Fixed]
+ D960 HW engine enters infinitely loop at stopping sound and doing volume ramp down.
+ Fix C bugs:
    1. Fix srand() hand up and LVD_Enable() problem for project of C language.
    2. Fix assembler to support 'a' -'A' operation.
    3. fix C TMG_Open() register setting error
+ Fix pattern event bugs
    1. Can't run pattern event convert
    2. User event should be kept if the event index in pattern event table is reserved type.
+ Wrong link statements in .loc but not report error line
+ Compile customer's project but can't completed

-------------
N589 SDS V1.08.000
-------------
[Features]
+ Add N589E chip series
+ Add N589[B/C/D][1K5/2K0]_[SOP14]
+ Add SPI clock rate UI setting and passed to FW lib
+ Support configurable I2C Pins
+ Make N589E BP05 set as input pin in PS project

[Modification]
+ All sections including free space after HW engine are treated as internal resources
+ Prevent user from calling TABLE_LOOkUP from different sections to avoid cross bank accessing and result in getting wrong value
+ Add success message after downloading to chip

[Bug-Fixed]
+ Correct chip selector information about [Voice Channel], [SPIO], [UART], [ADC]
+ [N589E] DPD_Rx in watch window do not reference to correct address
+ After resource was edit in resource window, the new resource list didn't updated
+ Correct procedure of command address table checking
+ FW - Fixed the bug that CAPKEYxT would be triggered twice when CapTouch was pressed
+ FW - Fixed the incorrect response of TG wake-up in the CapTouch wake-up check mechanism
+ FW – compiling error due to extra table
+ FW – [N589E] Update PS kernel for LVD wrong naming
