-------------
N589 SDS V2.00.000 SP2
-------------
Based On N589_V2.00.000 SP1 and add the following issue.

[Features]
+ Added chip items: N589D [086/126/176] [SOP8/SOP14/TSSOP20]
+ For N589E, display timers used by what kinds of PS/ASM functions
+ Added Amplitude Modulation feature to UltraIO.
+ Update NSS, NSP, NSPO codec.
+ Volume transition according to the time set by command
+ For N589L, added options of “HW Protection Mode”.
+ Write checksum to USRCFG2 for verification. The checksum written is the same as the last two bytes of .obj file as well as the checksum in "S/W" item's value in form file, which is the number after version and customer id.

[Fixed Bugs]
+ Prevent key-scan from missing valid key presses due to glitches.  Key polling will also be performed when a port interrupt occurs.
+ Fixed RGB LED white flash during HW PWM transition before entering sleep
+ Fixed an issue in which the PowerScript LRC wake-up function might cause a compiler error on certain chip bodies.
+ Fixed multi-byte character handling in line continuation detection
+ Fixed: Selecting "Disable" option in "Initial RAM Clear" would mistakenly clear the lib RAM.
+ Fixed some compiling error for common files of C language.


-------------
N589 SDS V2.00.000 SP1 2025/10/15
-------------
Based On N589_V2.00.000 and add the following issue.

[Features]
 + N589L support two-channel playback.
 + For PowerScript table lookup function, allow one new scenario: if table is in Program section, looup table command can be in any section.
 + Added two more options of Debounce Time for Direct Trigger: [24|30] ms.

[Bug-Fixed]
 + Adjust HW engine wakeup flow for runtime color fly to ensure correct color index update and LED transition.
 + IR Tx pin just has BP24 excluding BP14 for N589D125 TSSOP20.


-------------
N589 SDS V2.00.000
-------------
Based On N589_V1.09.000 SP16 and add the following issue.

[Features]
+ Enhanced UI with new style and layout
 - Redesign the library setting UI to offer a more intuitive and user-friendly experience
 - Support for editing IDT file with UI mode(required at least NuIDE V4.00.000 SP4)
 - Enhance Memory Layout Window to clearly RAM and ROM usage (Required at least NuIDE V4.00.000 SP4)
 - Display predefined handlers, allow to select a handler to navigate to its code position or create it if it does not already exist. (Required at least NuIDE V4.00.000 SP4)
 - Illustrate the usage of relevant parameters in the IR Setting window.
 - Support the new layout for the ALED settings.
+ Add support of two-wire ALED for N589L chip series.
+ Add a "Use boost voltage periodically during sleep" option for playing external flash on the N588L chip series.
+ Add documents with PDF format for N589ABCDSL

[Bug-Fixed]
+ Fixed timer TMG0 calculation bug
+ Keep library setting dialog in the selected theme mode after changing chip
+ Fixed compiler parsing issue with single-line conditional blocks for Play instruction of C language

-------------
N589 SDS V1.09.000 SP16
-------------
Based On N589_V1.09.000 SP15 and add the following issue.

[Features]
+ Added options of “Using BP1.3 to control SPI Flash VSS” for N589LS00
+ Exposed ALED data for customized usage.

[Bug-Fixed]
+ Fixed: Do not auto fill options of IR type because the IR commands are commonly used across all types.
+ Fixed: The way to describe ALED capability has been changed, but the option for setting Vixen timing didn't modify correspondingly.
+ Update FWLib : Modify the way MCU sends Deep Power-Down command to SPI flash.
+ For N589LS00[TSSOP20|TSSOP28], fixed maskoption value which caused the failure of setting booster voltage at run-time.

-------------
N589 SDS V1.09.000 SP15
-------------
Based On N589_V1.09.000 SP14 and add the following issue.

[Features]
+ Support N589LS00 TSSOP28
+ Support N589L080/120/170/200/250/300 TSSOP20 and TSSOP28
+ Support new PS instructions to control input/output mode directly
	- SET_PORT_FLOATING, SERT_PORT_PUL_HIGH
	- SET_PORT_OUTPUT_0, SET_PORT_OUTPUT_1
+ Support SPI instructions for N589LS chip series

[Modification]
* Remove N589LS MCP from chip supporting list
* Adjust SPIM pin mapping of N589LS00
* Resize resource size window according to scale % setting
* Show program size and resource size in internal ROM usage

[Bug-Fixed]
* Fixed an issue where text in the memory information section of the resource window was cut off when Windows display scaling was applied


-------------
N589 SDS V1.09.000 SP14
-------------
Based On N589_V1.09.000 SP13 and add the following issue

[Feature]
+ Introduced automated options selection for multiple functions (PS optional functions, peripheral and background number) if related PS function call is found.

-------------
N589 SDS V1.09.000 SP13
-------------
Based On N589_V1.09.000 SP12 and add the following issues

[Features]
+ Extended PS instructions for
    - New arithmetic operations – Multiplication, Division and Remainder.
    - New port and pin assignment operations.
    - New port and pin IF conditional statements.
+ Added 2-wired ALED for N589D[201|251|341|481|205|255|345|485].
+ Supported N589L080

[Bug-fixed]
+ Bit setting of protection area for N589S080 is incorrect.
+ N589B[085|125|175|205|255|345]_[TSSOP28|LQFP48] didn’t support one-wire ALED.

-------------
N589 SDS V1.09.000 SP12
-------------
Based On N589_V1.09.000 SP11 and add the following issue

[Features]
 + Add N589LS[00|08|16|32|64]
 + N589S080 series chip support HW I2C with commands I2C_WRITE_MULTI_BYTES and I2C_READ_MULTI_BYTES.
 + Added support of one-wire ALED by HW Engine via SPIM For N589B[085|125|175|205|255|345]_[TSSOP28|LQFP48].
 + Added support of generating .obj file which can be calibrated by Cap Touch Tool for N589L/N589LS series chips.

[Bug-Fixed]
 + LVD will be disabled before entering IDLE mode to avoid currency leakage.
 + Remove special handling to deal with the following circumstance: duration of note is shorter than one FXF interval.

-------------
N589 SDS V1.09.000 SP11
-------------
Based On N589_V1.09.000 SP10 and add the following issue

[Features]
 + N589S support ALED function
 + Add new macro - SET_SLD_GROUP_OUTPUT to do one-wire ALED output switch
 + Add TSSOP28 package support of the following chip bodies
	- N589B[480|650|960]_TSSOP28
	- N589D[650|960]_TSSOP28
	- N589B[1K5|2K0]_TSSOP28
	- N589D[1K5|2K0]_TSSOP28
	- N589B[485|655|965]_TSSOP28
	- N589D[655|965]_TSSOP28

[Modification]
 * [N589E FW] Upon power-up and wake-up, set the EXT LVD pin as a floating input. 
              The enable/disable LVD statements no longer handle the state of the EXT LVD pin.
 * For [TSSOP20|TSSOP28] of N589Bxx5 and N589Dxx5, two pins are being used as ICE pins (ICEDATA, ICECLK).
   PS. Capability of available functions are slightly different from previous definition.
  
-------------
N589 SDS V1.09.000 SP10
-------------
Based On N589_V1.09.000 SP9 and add the following issue

[Features]
 + Add chip item support for N589S080[DIE|TSSOP20|TSSOP28|LQFP48]
 + Add the PS commands: PROTECTION_PAGE_ERASE_ALL, IDLE
 + Support for converting servo motor and frequency transition curves in UIO files.

[Bug-Fixed]
 + Fix bug in wave table file conversion process which has chance to convert fail under new multiple process resource conversion mechanism.
 + Fix cap key index mapping for some package form chips.

-------------
N589 SDS V1.09.000 SP9
-------------
Based On N589_V1.09.000 SP8 and add the following issue

[Features]  
  + Support these TSSOP28 chips
	- Add N589B085|125|175|205|255|345
	- Add N589D081|121|171|201|251|341|481
	- Add N589D085|125|175|205|255|345|485

-------------
N589 SDS V1.09.000 SP8
-------------
Based On N589_V1.09.000 SP7 and add the following issue

[Features]
  + N589L support CapTouch
  + Add N589B[080|120|170|200|250|340]_TSSOP28

[Modification]
  * Enhance [Import UID]
	- New DEFAUD attribute - FileExt. Can exprot "fileExt" definition or not in export dialog.
	- Output .LOG file located in project folder which describe each decision step for certain circumstances 
        (e.g. not found audio resource, encoded format is not defined, etc.).
	- Refine searching strategy of audio resources.
	- Refine exporting of UID file.
  * Fine-tune [Duplicate Project]
	- Always disable duplicating system include files.
  * Fine-tune play-by-index code-generation that affected intelligent build.

[Bug-Fixed]
  * Fix bug that after changing search path, the builder will fail to link resource file.
  * Behavior of search path changed.
	- Allow to add non-exist folder when editing the search path.
	- Do not remove the search path even if the path does not exist upon opening the project.
  * Help description about “Play Segment” is missing.

-------------
N589 SDS V1.09.000 SP7
-------------
Based On N589_V1.09.000 SP6 and add the following issue
[Features]
+ Support N55P243 IO expander.
+ Support at most 5 IO expander devices.
+ Support at most 120 UltraIO outputs.
+ Support gamma curve for ALED output signal.

-------------
N589 SDS V1.09.000 SP6
-------------
Based On N589_V1.09.000 SP5 and add the following issue.

[Features]
  + Support N589B650 to access SPI flash by GPIO.
  
-------------
N589 SDS V1.09.000 SP5
-------------
Based On N589_V1.09.000 SP4 and add the following issue

[Features]
  + Enhance IR library to reduce probability of false trigger of N589 IR
  + Support IR 16bits data
  + New GUI to display and list checking result about IR protocol setting
  + Speed up building resource files by multi-processors
  + Check and fix serial LED color pixel information must be smaller than max sample position when generate the play ALED data.
  + Check new generated ALED data position is too close the final ALED data position then skip generate data at converting ALED data

[Bug-Fixed]
  * For N589L chip series, protection page doesn't work.

-------------
N589 SDS V1.09.000 SP4
-------------
Based On N589_V1.09.000 SP3 and add the following issue

[Features]
  + Software ALED with configurable ALED output pins.
  + Add support of N589D [655|965] and related packages
  + Add new defaud parameter - BitRate that is available during UID import/export.

[Modification]
  + Pack checking sample rate messages into SpeechCheck.txt file.

[Bug-Fixed]
  + Smaller silence wio encoded as NSP with noise

-------------
N589 SDS V1.09.000 SP3
-------------
Based On N589_V1.09.000 SP2 and add the following issue

[Features]
  + Support Addressable LED for N589E chip series.
  + Can add Vixen format(.CSV) into resource window as EVO for playback ALED directly for N589E chip series.

[Bug-Fixed]
  + "Reference External Voltage" setting does not be saved
  + Request Form file shows wrong information about UltraIO enabled port name for asm project.
  + Key stop responding when use sleep timer in conjunction with certain stack operations for PS project.(N589ABCDL)
  + For PowerScript project, fixed an issue that the Error Code returned by the “Read/Upadte protection page” instruction was incorrect. (N589ABCDL)

-------------
N589 SDS V1.09.000 SP2
-------------
[Features]
  + Can add Vixen format(.CSV) into resource window as EVO for playback ALED directly with adjustable Vixen data time interval
  + Add a note message to info user to enable LVD in LVD setting GUI

[Bug-Fixed]
  + Fix calculation of address of SLD data chunk bug for N589A1K4|N589A1K9|N589B1K5|N589B2K0|N589C1K5|N589C2K0|N589D1K5|N589D2K0
  + Fix to report error when the IF, SWITCH,WHILE expression do not match with END syntax.

-------------
N589 SDS V1.09.000 SP1
-------------
[Bug-Fixed]
  + Correct MIDI delta time calculation for long duration pairing of note-on and note-off.

-------------
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

