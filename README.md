All installers are zipped with password: 123456

N589 SDS V1.09.000
-------------
[Features]
  + Add N589L340 chip series
  + N589B085|125|175|205|255|345 support software-based one-wire ALED function by HW Engine via SPIM.
  + N589D081|121|171 support software-based two-wire ALED function.
  
[Modification]
  + Extend maximum output LED count of software-based ALED from 8 to 12.
  + New IR implementation for N589L340 chip series.
  + Modify display of selectable value of Fcpu and Fsys options, and have these values consistent among UI, FRM file, and *.p file.
  + Adjust check of instrument maximum loop range to 64K PCM sample count.

[Bug-Fixed]
  + Add run-time variable - LVD_EXT_REF which is used to set input type to floating for LVD Reference External Voltage.

-------------
N589 SDS V1.08.000 SP10
-------------
[Features]
  + Support more than 256 entries of long jump/call.
  + For PowerScript project, remove the restriction of period for LRC wakeup timer and extends it to about 14 hours.
  + Add online help about "get sub index" into "Asm Instrunciton Window" and "PowerScript Instruction Window"

[Bug-Fixed]
  + After expanding PS macro, the JP/CALL to auto label (“label_name#”) will always convert them to LJP/LCALL.
-------------
N589 SDS V1.08.000 SP9
-------------
[Features]
  + Add N589D485 chip series
  + Add N589B965 chip series
  + Support 1 Foreground and 2 Background
  + N589D340 support SW-ALED
  + New chip duration calculation scheme which take 6502 program code size and UltraIO into calculation
  + Output audio 1KHz sinewave for some defined periods
  + Allow user to customize UltraIO event handler
  + Extends UltraIO output pin number to 64
  + Output audio 2.5KHz sinewave for some defined periods
  + Calculate external checksum
          
[Modification]
  + Allow number of labels called by LJP/LCALL can have at most 256
  + Remove debugger memory window about program rom size limitation
  + Adjust IDT checking mechanism of root-key-range
  + Adjust checking of LoopEnd sample of timbre
  + Modify available protection page size for User Data from 510 bytes to 508 bytes
  + In PowerScript project, no matter we enable touch key (LD EN xxx), we are requested to get status of cap sensor by calling CAP_SENSOR_ACTION_SUM
        
[Bug-Fixed]
  + Memory layout window display incorrectly
  + SoundFontTool might crash uncertainly
  + NuIDE crashed when certain wav file was being encoded to NSD format
  + Ultra IO LED effect is incorrect while we use NSD with enabling loop
  + Correct initialization of pre-emphasize function
  + Correct IR obstacle detection timer count value
  + While converting long speech file, pre-emphasize function will output zero after a specific timestamp

-------------
N589 SDS V1.08.000 SP8
-------------
[Features]
  + Add N589D175 chip series
  + Add N589E081/N589E061/N589E041
  + Add minima memory requirement check for NSD codec
  + NSP_O support loop + silence compression simultaneously
  + Add C language API(s) to get raw cap touch value
  + Add option to enable/disable ISP for N589E
  + Add support to 256Mbits and 512MBits SPI flash
  + Extend keypad, trigger key, mode key de-bounce time to 400ms(#3545)
  + Assembler support assign value into predefined symbols
  + Change Ouput Init GUI "Wakeup Init" name to "Sleep State"

[Modification]
  + N589E FW – Remove calling PREPARE_FOR_SLEEP from wakeup procedure
  + Display IR Wakeup period description with a range(#0003535)
  + Allow user to use read/write/erase ISP function depends on ISP option enable or not
  + Add SynLibSize and BitRate parameters of NSS and MD4
  + SDS always output build target to Project_Folder\Code_Release\

[Bug-Fixed]
  + Compile cap touch function but report error in ASM project
  + Modify and cancel the limit that the read/write protection page command can only be called in Bank0 in PS/ASM project
  + UIO HWPWM pin psf instruction（LD output, [array]/ output = [array]）error
  + FWLib: Keypad library to prevent unpredictable error

-------------
N589 SDS V1.08.000 SP7
-------------
[Features]

[Bug-Fixed]
+ Fix issue to build project through command line NuCmd.exe
+ FW Lib: Fix to avoid stack leaks that could be intercepted during execution.
+ FW LIb: Fix PS library debounce time is 0 issue

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
