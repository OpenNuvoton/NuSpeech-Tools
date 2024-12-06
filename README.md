All installers are zipped with password: 123456

---------------------------------------------------
NSP PlayList Editor V3.00.000
---------------------------------------------------
Based on V2.00.000 SP9
[Features]
(1) support multi-language GUI (current support English and Simple Chinese GUI)
(2) support multi-language resoure files in resource editor
(3) support multi-language search folder name in reosurce editor
(4) support multiple play lists on sound editing mode
(5) speed ​​up project building time
(6) support NSR chip series: NSR2230Z/NSR2530Z/NSR2830Z
(7) unsupport EOL chips: NSP080A/NSP081A/NSP170A/NSP171A/NSP340A
(8) support new sound recording command [RECORD_INDEX_START/RECORD STOP] on CPU mode for NSR chip project
(9) support new play mode (Record Index/Level Hold Record/Stop) on Demo mode for NSR chip project
(10) support LED configuration on Demo mode for NSR chip project
(11) support auto detect new version then upgrade
(12) switch chips will not close tool then reopen tool

[Bug-Fixed]
(1) Fix P16 silence compression setting error then lead to P16 playback noise

---------------------------------------------------
NSP PlayList Editor V2.00.000 SP9
---------------------------------------------------
[Features]
(1) support ISP FW update via USB to UART dongle
(2) support chip NSP2080A03G/NSP2170A03G/NSP2340A03G
(3) support NSP command "MULTI_PLAY_SILENCE" and "MULTI_PLAY_2B_SILENCE"
(4) fix to always enable silence compression condition on NSP2 chip project
(5) pop the floating prompt window to show different remain time of different sample rate(8K,12K,16K) or rate(8K,10K,12K) setting when mouse move on the remain block of status bar

---------------------------------------------------
NSP PlayList Editor V2.00.000 SP8
---------------------------------------------------
[Features]
(1) Based on SP7, disable ISP FW update via USB to UART dongle.
(2) Add "Low Active" text on busy pin label control of project setting
(3) Pop ISP function tips message after user clicked "Enable ISP Function" check box

[Bug-Fixed]
(1) NSP040 resource window hide unsupported menu items [Volume Boost(db)] and [Change Bit Rate]
(2) fix to drag and drop resource item on play list will fail if wave file name with "." word
(3) fix to export excel file and some information become garbled if information with non-English word

---------------------------------------------------
NSP PlayList Editor V2.00.000 SP7
---------------------------------------------------
[Features]
(1) Support P16 resource format on NSP1(exclude NSP040, NSP OTP) and NSP2 project
(2) Always pop update firmware message if the firmware version is different between chip board and tool firmware file
(3) Add NSP2 sleep mode and wake up via trigger key on Demo mode excluding NSP2 touch series
(4) Add UART/2-wire/1-wire Linux host sample codes in installer folder "NSP_HOST/NSP_HOST_Linux"

[Bug-Fixed]
(1) I2C data pin pull up resistance is 1M not 150K ohm
(2) Should disable GPIO interrupt to avoid abnormal GPIO interrupt happen before enter power down for NSP2
(3) Build project failed when resource resample value is changed on NSP OTP chip project

---------------------------------------------------
NSP PlayList Editor V2.00.000 SP6
---------------------------------------------------
[Features]
(1) Support “PLAY_REPEAT” NSP command for NSP1 chip project
(2) Support NM4/NSP with 16k sample rate for NSP1 and NSP2 project
(3) Support NM4 only with 24K sample rate for NSP1 and NSP2 project
(4) Switch UI language to "English" or "Simplified Chinese" from menu [View][Switch Language]
(5) Support to set the external PA Enable Pin, Pin Active level, and Delay Time on NSP650B/960B/2K0B chip project setting
(6) Support to add MP3 file into resource window
(7) Support [Sound & I/O preview], [resource update], [Touch Configuration Access] function on NSP1 and NSP2 UART mode project with USB 2 UART dongle
(8) Support to load user data binary file as default user data on NSP1 and NSP2 chip project setting
(9) Change the index column header text from "Index" to "Res Index" on resource window and shown index to resource files used for Playlist on resource window
(10) Change the index column header text from "Index" to "Play Index" on Sound Editing mode
(11) Extend user space max size from 99999 to 999999 bytes on NSP2340 chip project
(12) New NSPUpdate.exe tool supports updating single resource, whole resource and cap touch sensitive data
(13) Update document to describe command “TOUCH_READ_STATUS”
(14) update NSP ICP Writer tool
    (a) update mass storage firmware file [57.09.16.10]
    (b) support set I/O mode function to swith NSP dongle to "Input mode" and "SPI mode" for UART mode setting

[Fix bugs]
(1) fix playing long duration sound will become silence
(2) fix del all obj files at build/rebuild project
(3) remove unnecessary folder "NuVoiceFlashProgrammer"
(4) generate the directory name "BurningFactory" if generate directory "烧录厂" fail on none-Simplified Chinese windows environment
(5) update NSP2 FW 
    (a) fix playback un-stop in touch "LEVELHOLD mode" on "Demo Mode"
    (b) enable WDT function on "Demo Mode"
    (c) fix HCLK=HIRC/5 no sound playing problem
(6) update touch calibration tool [NuTouchConf.exe]
    (a) fix re-insert dongle that pad icon display wrong
    (b) fix insert dongle not pop up update firmware version message
    (c) fix calibration when user no touch in last step that no show "Too few effective taps detected" message
(7) update NSP ICP Writer
    (a) fix ISP updating fail (single resource, all resource, user data, touch configuration) if enable auto sleep on project setting

---------------------------------------------------
NSP PlayList Editor V2.00.000 SP5
---------------------------------------------------
[Features]
(1) Support chips with 16 touch keys- NSP2340T16L/NSP2170T16L/NSP2080T16L
(2) Support chips with 6 touch keys - NSP2340T06E/NSP2170T06E/NSP2080T06E
(3) Support chips with embedded PA - NSP2340A01G/NSP2170A01G/NSP2080A01G
(4) Support touch calibration tool to tune and create touch key settings for NSP2xxxT chip 
(5) Support touch configuration update/upload tool to update/upload touch key settings for NSP2xxxT chip
(6) Update host driver header file to have API comments
(7) Remove the user configuration and checksum information from *.rtf file
(8) Support new I2C host command – GET_SLAVE_ADDRESS
(9) Support power amplifier option for NSP2340 project to avoid pop up noise at using external power amplifier
(10) Support user data size over 999 bytes (max: 99999 bytes)
(11) Show message to explain 0 means play loop infinitely at modify play repeat count in demo mode
[Fix bugs]
(1) FW bugs
  (a) NSP2340 power on and wakeup time too long then make first command fail
  (b) Host MCU can’t communicate with other I2C device at NSP2340 enters sleep mode
  (c) Speech channel 2 can’t play silence even have silence duration set but channel 1 can
  (d) For NSP2 executing DO_CHECKSUM, ISP commands, should let execute new command as invalid command like NSP1
  (e) For NSP2 executing DO_CHECKSUM then enter sleep, the checksum value will be wrong after wakeup then issue READ_CHECKSUM
(2) Tool Bugs
  (a) At open NSPxx2 project created by version 1.xx.xxx, the auto sleep option will be set enable.
  (b) At change chip from NSP1 to NSP2 or NSP2 to NSP1, the settings about "auto sleep", "reset status", "UART enable", "UART baud rate" are incorrect
  (c) The rest of sound length is incorrect for project using large flash size chip.
	
---------------------------------------------------
NSP PlayList Editor V2.00.000 SP4
---------------------------------------------------
[Features]
(1) update NSP ICP Writer V1.13.110 to support HID connection protocol on NSP2340 chip project
(2) modify configuration setting to make the sound quality is better on NSP2340 project
(3) update NSP2340 firmware file
    (a) Add - Support new chip: NSP2xxxA01 series.
    (b) Modify - Wake-up function: Only BP0 can wake up the chip.
    (c) Modify - I2C communication process: Prevent CHIP from no-responding when EFT is tested.
    (d) Fixed - Noise problem: When playing commands sequentially (Stop->Delay->Play), a noise will be produced.
    (e) Fixed - Volume setting problem: After completing the ISP, changing the volume has no effect.
Note:
The HID connection protocol only support to send NSP command on two-wire mode sound & I/O preview

---------------------------------------------------
NSP PlayList Editor V2.00.000 SP3
---------------------------------------------------
[Features]
(1) support I2C protocol related function on NSP2340 project
    (a) support all resource update function
    (b) support single resource update function
    (c) support to access user space function
	(d) update NSP dongle firmware [56.09.1D.0A] to support sound & I/O preview function
(2) support new NSP command if continue playback is disable on NSP2340 project setting
    (a) PLAY_CHANNEL(0xA0)
    (b) STOP_CHANNEL(0xA1)
    (c) PAUSE_CHANNEL(0xA2)
    (d) RESUME_CHANNEL(0xA3)
(3) support one wire mode on NSP2340 project
(4) add UART supported baud rate 7200 and 128000 option on NSP2340 project setting
(5) limit the I2C device address maximum text length is 2 (1 byte) on NSP2340 project setting
Note: If the NSP2340 project support all resource update function on SP2, need to rebuild project and write project on chip after updating to SP3

---------------------------------------------------
NSP PlayList Editor V2.00.000 SP2
---------------------------------------------------
[Features]
(1) update these features of NSP2 chip project
	(a) change the UART support baud rate (9600, 19200, 38400, 57600, 115200, 153600)
	(b) support to set reserved resource time function on resource window
(2) support [GET_MAX_INDEX] NSP command
(3) fixed to run "NSP Partial Update Tool" application and pop warning message
(4) NSP2080/2170/2340, NSP082/172/342 and NSP171A53/341A53 chip project do not support one-wire protocol
(5) update document
    (a) NSP PlayList Editor Tool User Guilde CHS.pdf
    (b) NSP PlayList Editor Tool User Guilde EN.pdf
    (c) NSP Update Function Application Note EN.pdf
    (d) NSP Update Function Application Note SC.pdf
    (e) NSP_TwoWire MCU Interface_CHS.pdf
    (f) NSP_TwoWire MCU Interface_EN.pdf
    (g) NSP_UART MCU Interface_CHS.pdf
    (h) NSP_UART MCU Interface_EN.pdf
    (i) NSPOTP_TwoWire MCU Interface_CHS.pdf
    (j) NSPOTP_TwoWire MCU Interface_EN.pdf
    (k) NSP_TwoWire MCU Interface Timing.pdf
    (l) NSP_I2C MCU Interface_CHS.pdf
    (m) NSP_I2C MCU Interface_EN.pdf
[Note]
If the project chip item is NSP2080, NSP2170, and NSP2340, please rebuild project to generate all resource update binary file after updating to SP2

---------------------------------------------------
NSP PlayList Editor V2.00.000 SP1
---------------------------------------------------
[Features]
(1) update the SDS chip list on new project and can switch chip between NSP and NSP2
    NSP group:
	NSP040A,NSP080A,NSP080B,NSP081A,NSP082A,
	NSP170A,NSP170B,NSP171A,NSP172A,NSP340A,
	NSP340B,NSP341A,NSP342A,NSP480B,NSP481A,
	NSP650B,NSP960B,NSP2K0B,NSP171A53A,NSP341A53A
    NSP 2 group:
	NSP2080A,NSP2170A,NSP2340A
    NSP OTP group:
	NSP075A,NSP075B,NSP165A,NSP165B,NSP335A,NSP335B
(2) support NSP082A/172A/342A
(3) support NSP2 ISP functions (All resource update, single resource update, update user space)
(4) support to generate precode zip file on NSP2 group project
(5) update NSP PlayList Editor Tool User Guide document with new features added.
(6) update NSP Update Function Application Note with new features added.

[Bug Fix]
(1) fix noise at the end of sound if enable silence compression with larger threshold value
(2) fix the silence compression not work on NSP2 group project

---------------------------------------------------
NSP PlayList Editor V2.00.000
---------------------------------------------------
[Features]
(1) support NSP2 series chip: NSP2340A/NSP2170A/NSP2080A
(2) support NSP1_SP series chip: NSP171A53A/NSP341A53A
(3) support to change output file name on NSP chip project(*.obj and *.rtf)
(4) support to switch chip between NSP040 chip and other NSP chip(NSP080, NSP340, etc...) on project setting page
(5) generate the precode zip file on NSP project "烧录厂" folder

[Bug Fix]
(1) update HW file to modify decode function for noise issue

---------------------------------------------------
NSP PlayList Editor V1.20.000
---------------------------------------------------
[Features]
(1) support chip: NSP2K0
(2) demo mode support mixed pins(BP00+BP01) on SOP8 packet

[Bug Fix]
(1) After access user data space, running any command will cause command invalid on sound & I/O preview window.
(2) On project setting, sets the busy pin of one wire mode then change to UART mode. This will cause the BP01 option is missing in “Busy Pin” selection window.
(3) Move resources from source index to target index then build project but these moved resource will be shown up in source index.
(4) The wrong selectable busy pin for some package then generate wrong busy pin definition for FW

---------------------------------------------------
NSP PlayList Editor Tool V1.13.000 SP1
---------------------------------------------------
[Features]
(1) set the default play index is 1 for PLAY command in sound and IO preview window
(2) check and update dongle firmware before download object file or send sound and IO preview commands
(3) support IO pull mode of keypads for demo mode
(4) support level hold play mode with IO pull mode for demo mode
(5) support import/export resource and playlist information from/to excel file
(6) support "auto save resource" function to copy resource files into "Resources" folder in project folder.

---------------------------------------------------
NSP PlayList Editor Tool V1.13.000
---------------------------------------------------
[Features]
1. Support chip: NSP040A(does not support resource update)
2. Remove chip: NSP650A, NSP960A.
3. Change OTP two wire wakeup pin form SDA to SCL pin
   (Need upgrade Host Driver Code)
4. Move host files to NSP_HOST folder
5. Change default value of “time to sleep” to 10 seconds.
6. New function is “Save Project(Include Resource Files)” to copy resource files to local project folder.
7. Change selecting chip name and package to be selecting chip name only on project setting.
8. Remove message to notify user to update host files.

---------------------------------------------------
NSP PlayList Editor Tool V1.12.000
---------------------------------------------------
[Features]
1. add continue play function (only for NSP 480/650/960)
2. add single resource update enable setting function
3. add busy pin selection GUI
4. add can drag&drop, copy, cut index item into audio resource
5. add sound resource list can according name sort
6. add enable silence compression
7. can stop resource update after start resource update and take too long time in sound and IO preview mode
8. add auto sleep function and support command on sound & I/O preview
9. add command timeout function 
10. support option to disable resource update function

[Fix]
1. incorrect sort after inserting multiple Audios right on Index (#3120)
2. delete the resource in sound editing used by the demo mode switching demo mode will cause crash (#3055)
3. setting operation, press Enter on the keyboard, some icons will disappear (#2936)
4. demo Mode adds resource in the blank space, additional branches will appear (#3041)
5. The sampling rate of the Chinese wav file exceeds 16000, the post-build message is not Chinese (#3060)
6. One Wire does not support User Data Size suggestion field is grayed out (#3119)

---------------------------------------------------
NSP PlayList Editor Tool V1.11.000
---------------------------------------------------
[Features]
1. support UART communication (only for NSP 480/650/960 SOP14 chip)
2. provide reserved user space function on build setting
   user can get the user space information(ISP address, user space size) and access using ISP read and write partial command
3. support multiple play 2 bytes command on two wire mode
4. support to set equalizer parameter value and the resource can apply equalizer effect on resource window
5. speed up the build time
6. support the USB HID protocol connection (one-wire command not implement completely) 
7. Enlarge play list index from 1024 to 65536.
8. Support multiple NSP chips coworking with one MCU.
9. NSP OTP chip series support MDM playback format

[Fix]
1. NSP OTP chip series with LVR should be set to 2.0V
2. Programming OTP chip will be failed sometimes.
3. Fail to rebuild NSP OTP project
4. Clear the content of a folder at new project to a existed folder, to prevent old encoded resource data are used at build project.

---------------------------------------------------
NSP PlayList Editor Tool V1.10.000
---------------------------------------------------
[Features]
1. add support NSP341/481
2. add support NSP OTP chip include NSP075/165/335 (#2754)
3. add drag and drop function on “Sound Editing” and “CPU Mode”
4. add support multiple select resource on “Sound Editing” and “CPU Mode”
5. add sound resource list use shift hot key to add separate index on “Sound Editing”
6. add when resample out of range need to popup warning message (#2336)
7. add export full error log file to verify problem (#2745)

[Fix bugs]
1. fixed device not found, but when build and write finish, the message is write ok(#2919)
2. fixed parameter error and crash while type volume boost (#2340)
3. fixed when demo mode index have resource but repeat is 0 when open befoere V1.09.000 version (#2738)
4. fixed can not set 0 to disable reSample (#2701)
5. fixed default should focus on "OK" while New Project Settings Window (#2726)
6. fixed always highlight after cancel drag resource to add audio (#2731)
7. fixed whole index should not be selected after delete the final audio (#2728)
8. fixed wrong dispaly if close tool at max size then open again (#2348)
9. fixed select resouce that reaction to slow (#2212)
10. fixed some wave file play with "Bo" noise sound


---------------------------------------------------
NSP PlayList Editor Tool V1.09.000
---------------------------------------------------
[Features]
 1. support NSP 480/650/960 chip
 2. Add repeat command & stop repeat function (#2735)
 3. Remove unnecessary information and file of playlist tool (#2544)
 4. support setting sound quality level in resource window (#2545)
 5. Move "PLAY" command to be the first command in Sound & IO Preview window (#2598)
 6. Support POR to play sound in demo mode (#2605)
 7. Add BP06 and BP13 normal pin at SOP14 when at demo mode(#2644)
 8. Support new HOST ISP command with checksum verification

[Fix bugs]
 1. execute two Playlist Editor Tool at the same time lead to write function fail(#2262)	
 2. execute Playlist Editor Tool and ICP Writer at the same time lead to write function fail(#2114)
 3. popup update F/W when execute Sound & IO Preview function sometimes (#2260)
 4. the resource path is not found, build+write will still succeed (#2242)
 5. Sound & IO Preview function should not be executed when in demo mode (#2542)
 6. Add resource that estimate percentage inaccuracy (#2543)

---------------------------------------------------
NSP PlayList Editor Tool V1.08.000
---------------------------------------------------
[Features]
 1. NSP PlayListEditor Tool uninstall can not clear all file	(#2349)
 2. Use ISP online update audio resource 			(#2215)
 3. Build will no action after open project			(#2213)
 4. GUI no action at loading a large of resource 		(#2210)	
    files into resource window		
 5. When create new project can immediately to set option	(#2256)	
 6. Support chinese folder name					(#2259)	
 7. Select/Delete: take too much time at add or del 		(#2261)
    resource file in resource window
 8. Resource Editor added wave file can not be save		(#2238)
 9. Using the hotkey Delete to delete more than 5 		(#2245)
    consecutive times will cause the NSP PlayList Editor to stop
 10.Sound and IO Preview Index over 50 PLAY will be Invalid	(#2246)
 11.Build project demo or cpu mode be copy object file from 	(#2374)
    Code_Release to project folder, and only one mode 
    object file exist.
 12.Change sample rate but this project will not build 		(#2375)
    if this project was built before.	
 13.Click Next time not notify update NSP_HOST message, 	(#2429)
    and re-build+write message will pop up this message.
 14.Add one wire and two function
 15.Add Rebuild function 
