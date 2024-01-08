All installers are zipped with password: 123456


---------------------------------
NSP_ICP_Writer_V1.17.000 SP1
---------------------------------
1. test check version and update tool function 

---------------------------------
NSP_ICP_Writer_V1.17.000
---------------------------------
1. test check version and update tool function 

---------------------------------
NSP_ICP_Writer_V1.16.105
---------------------------------
1. test check version and update tool function 

---------------------------------
NSP_ICP_Writer_V1.16.103
---------------------------------
1. support to update application from Git URL
2. modify code to parse command string

---------------------------------
NSP_ICP_Writer_V1.16.102
---------------------------------
1. fix to program NSP2 chip fail on off-line mode if program option selection is [Program only boot loader]
2. use extra series enumeration value [NSP2_SERIES = 0x90000E] to differentiate NSP2 and NSP chip [NSP_SERIES = 0x900005]

---------------------------------
NSP_ICP_Writer_V1.16.101
---------------------------------
1. support to set program option (Program all data/Program only boot loader) on NSP2340 chip project object file
2. modify the update resource error message from "ISP update header signature wrong." to "Incorrect ISP update file"
Note: Program only boot loader option is that only program LDROM data for ISP update function via UART

---------------------------------
NSP_ICP_Writer_V1.16.100
---------------------------------
1. fix single resource update and user space update fail if the first update space size is less than or equal to one page (512 bytes)

---------------------------------
NSP_ICP_Writer_V1.15.000
---------------------------------
1. update mass storage firmware file [57.09.16.10] to support set I/O mode function

---------------------------------
NSP_ICP_Writer_V1.14.000
---------------------------------
1. support chip NSP2340T06/NSP2170T06/NSP2080T06
2. update mass storage firmware file [57.07.0D.0C]
3. update help document

---------------------------------
NSP_ICP_Writer_V1.13.000
---------------------------------
1. support chip NSP2340A01/NSP2170A01/NSP2080A01
2. support chip NSP2340T16/NSP2170T16/NSP2080T16
3. update mass storage firmware file [57.03.1C.12]
  (a) support touch related command (calibration command, config upload, config download)
  (b) support new NSP command [PLAY_REPEAT][PLAY_CHANNEL][STOP_CHANNEL][PAUSE_CHANNEL][RESUME_CHANNEL]
4. update HID firmware file [57.01.1E.0E] to support NSP2340 chip series
5. support NSP command on I2C mode

---------------------------------
NSP_ICP_Writer_V1.12.000
---------------------------------
1. update help document
2. update firmware file [56.08.04.0A] to support NSP command [GET_MAX_INDEX]
3. support new object file format on NSP2340 chip project

---------------------------------
NSP_ICP_Writer_V1.11.000
---------------------------------
1. support chip NSP082/NSP172/NSP342

---------------------------------
NSP_ICP_Writer_V1.10.000
---------------------------------
1. support chip NSP2340/NSP2170/NSP2080
2. support chip NSP171A53/NSP341A53/NSP082/NSP172/NSP342
3. update firmware file [56.05.1B.12] to modify the Tail time of NSP One-Wire Command from 500us to 3180uS

---------------------------------
NSP_ICP_Writer_V1.09.000
---------------------------------
1. support chip NSP2K0

---------------------------------
NSP ICP Writer_V1.08.000
---------------------------------
1. support offline mode in USB HID protocol dongle for both normal mode and factory mode

---------------------------------
NSP ICP Writer_V1.07.000
---------------------------------
1. support chip NSP040/NSP082/NSP172
2. support to show CRC32 information when the Flash file is selected
3. update help document for NSP075/165/335 program time on offline mode

---------------------------------
NSP ICP Writer_V1.06.000
---------------------------------
1. update mass storage and hid protocol firmware file [54.07.19.0B]
(1) support pause and resume command
(2) support automatically sleep enable or disable command on one-wire mode or two-wire mode
2. the chip mode UI not switch between ICE mode and ICP mode when the chip board is changed

---------------------------------
NSP ICP Writer_V1.05.000
---------------------------------
1. Support HID protocol on online ICP mode and release HID firmware file[54.06.0C.0C] (ISP one-wire command not implement completely)
2. Update OTP Writer to fix the problem that show work successfully but not do anything actually
3. Update mass storage firmware file [54.05.06.14] for ISP upload SCL from 20us to 40us
4. Implement the function to access user space using ISP command

---------------------------------
NSP ICP Writer_V1.04.000
---------------------------------
1. Support NSP 075/165/335 programming with OTP writer
2. Support NSP 341/481/480/650/960 programming
3. Wake up NSP chip before resource partial update or whole resource update to avoid power down on NSP sleep mode
4. Menu support to switch check ICP firmware using normal version or factory version [Help]->[ICP Firmware Check]
   a. NSPAutoFw.bin - factory firmware file(54.03.03.0C)
   b. NSPIceFw.bin - normal firmware file(54.02.18.12)
5. Update document with console mode information

---------------------------------
NSP ICP Writer_V1.03.000
---------------------------------
1. Fix to program NSP650/960 but showing obj file size is not matched with chip size
(Ex.For NSP960 object file to NSP960 Board will show message "Forbidden: The obj file is too large to download to target chip.(Obj:1048576 Bytes, Chip:524288 Bytes))"
2. The GUI will show upgrade firmware message once until the application is closed
3. Update firmware file to version 53.0C.0C.17

---------------------------------
NSP ICP Writer_V1.02.000
---------------------------------
1. Update F/W file[53 0C 0C 17] to support new NSP ISP Command
2. Support new speech chip(NSP480,NSP650,NSP960)
3. The GUI will not always show upgrade firmware message continuously when choose to cancel update firmware until the application re-open

---------------------------------
NSP ICP Writer_V1.01.000
---------------------------------
1. Update F/W file(53091B0E)
2. ISP update function will check the binary file Product ID and PDID is match or not with chip board on console mode
3. Hide the UI that internal Flash is checked or not (This tool only program data on flash)
4. Configuration setting encrypt
5. Support to show chip board lock status
6. Fix the EVB detection flows to cause whole chip erase fail and verify fail

---------------------------------
NSP ICP Writer_V1.00.000
---------------------------------
1. NSP Style UI and document
2. Fix the detection device fail problem (PID and VID can't get valid string)