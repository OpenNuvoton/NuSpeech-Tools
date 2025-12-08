-------------
Speech ICP Writer V2.06.000
-------------
Based on V2.05.000.

[Features]
+ Support for chips N589D086, N589D126, and N589D176 package SOP8, SOP14, TSSOP20
+ Add checksum-based verification to confirm whether the .obj file matches the content previously written to flash
  Should update FW to write checksum infomration into flash for off-line.
  - Updated mass storage firmware file to [59.0B.0E.12] for Normal-Version Dongle
  - Updated mass storage firmware file to [59.0B.15.10] for Auto-Version Dongle
  - Updated mass storage firmware file to [59.0B.15.11] for Factory-Version Dongle
+ Improve the UI and refined the selection method for the upload function area

-------------
Speech ICP Writer V2.05.000
-------------
[Feature]
+ Fix unstable at detecting N589 EVB board.

-------------
Speech ICP Writer V2.04.000
-------------
[Feature]
+ For the N589LS00 chip, according to the SPI flash VSS pin setting, run SPI flash VSS control before writing the SPI Flash.

-------------
Speech ICP Writer V2.03.000
-------------
[Feature]
+ support for programming SPIFlash with the N589LS00 TSSOP28 package

-------------
Speech ICP Writer V2.02.000
-------------
[Feature]
+ support chip N589L080
+ fixed the issue of getting the incorrect protection page address on device flash content
+ extract header from the SPI Flash object file to determine whether the content should be divided and written into different SPI Flash devices

-------------
Speech ICP Writer V2.01.000
-------------
[Feature]
+ support these N589LS series chip: N589LS[00|08|16|32|64]

-------------
Speech ICP Writer V2.00.000
-------------
[Feature]
+ upgrade the build platform from Visual Studio 2010 to Visual Studio 2022
+ cancel the packet check and warning message display after loading the object file
+ support these N589B/D chip TSSOP28 package
  - N589B[480|650|960|1K5|2K0], N589D[650|960|1K5|2K0]
  - N589B[485|655|965], N589D[655|965]
+ update mass storage firmware file [58.0C.05.12] for normal version

-------------
Speech ICP Writer V1.23.000
-------------
[Feature]
+ update mass storage firmware file [58.08.16.13] for factory version
+ update mass storage firmware file [58.08.16.10] for normal version
+ support chip N589S080


-------------
Speech ICP Writer V1.22.000
-------------
[Feature]
+ support switching ICP firmware version to factory or normal version from menu [Help|ICP firmware Check]
+ support programming and verifying SPIFlash content for these chips
  - N589B340,N589B250,N589B200,N589B170,N589B120,N589B080(TSSOP28)
  - N589B345,N589B255,N589B205,N589B175,N589B125,N589B085(TSSOP28)
  - N589B650 (DIE)
+ update mass storage firmware file [56.08.08.0B] for factory version 
+ update mass storage firmware file [56.08.08.0A] for normal version 

-------------
Speech ICP Writer V1.21.000
-------------
[Feature]
+ support chip N589D655/N589D965

-------------
Speech ICP Writer V1.20.000
-------------
[Feature]
+ support chip N36D65
+ support to record programming result to excel log file and can click menu [Help | Program Log Folder] to open folder using file browser

-------------
Speech ICP Writer V1.19.000
-------------
[Feature]
+ support chip N589L120/N589L170/N589L200/N589L250/N589L340
+ add N589L chip mask option configuration
+ update F/W file [57.09.16.10]

-------------
Speech ICP Writer V1.18.000
-------------
[Feature]
+ support chip N589B965/N589B655/N589B485
+ support chip N589D485/N589D345/N589D255/N589D205


-------------
Speech ICP Writer V1.17.000
-------------
[Feature]
+ support chip N589D175/N589D125/N589D085
+ support chip N589E081/N589E061/N589E041

-------------
Speech ICP Writer V1.16.000
-------------
[Feature]
+ support chip N589B345/B255/B205/B175/B125/B085
+ update user guide document
+ update F/W file [56.05.1B.12] to support new data structure on offline mode to update N589A2K0 series chip
+ only allow to program N589 series object file to N589 series chip

[Bug Fix]
+ Load the ini file of N589E obj, an error message will appear 
+ Load ini file recent does not appear, it will appear after restart
+ The upload protection page function for N589E080 chip that upload flash start address is wrong

-------------
Speech ICP Writer V1.15.000
-------------
[Feature]
+ update F/W file(55.07.08.0C) to support new data structure on offline mode to update N589A2K0 series chip
+ support chip N589A1K4/A1K9/B1K5/B2K0/C1K5/C2K0/D1K5/D2K0 and related package N589BK5B/BK5F/BK5L/B2KB/B2KF/B2KL/CK5B/CK5F/CK5L/C2KB/C2KF/C2KL/DK5B/DK5F/DK5L/D2KB/D2KF/D2KL
+ support upload the content of protection page at security bit in unlock

-------------
Speech ICP Writer V1.14.000
-------------
[Feature]
+ update F/W file(55.04.08.0A) to check the protected bit of SPI Flash

-------------
Speech ICP Writer V1.13.000
-------------
[Feature]
+ support the chip N589E040/N589E060/N589E080
+ revise the UI position to fit the notebook size (1366x768)

-------------
Speech ICP Writer V1.12.000 
-------------
[Feature]
+ Chip NC9048/NC9065/NC9096 support to write SPI flash

-------------
Speech ICP Writer V1.11.000 
-------------
[Feature]
+ update F/W file(54.09.11.15)
+ update ICEDriver.dll to call get SPI-Flash ID function to wake up SPI-Flash download and upload function if SPI-Flash is power-off
+ add [AppPublisher] and [AppPublisherURL] on application to show information on Windows Programs and Features page
+ change the application file description and product name

-------------
Speech ICP Writer V1.10.000
-------------
[Feature]
+ The chip connection mode and related UI not switch correctly between ICE mode and ICP mode when the chip board is changed
+ Update help document for packet information
+ Support NSC series chips (NSC128DF/192DF/384DF/512DF/768DF/1K0DF)
+ Support NC90 series chips (NC9008/9017/9034/9048/9065/9096)
+ Support set limit count property at offline mode using command mode
  - "Speech ICP Writer.exe" /Console /Operation:pv /OfflineInternalFlash:"C:\Flash.obj" /SetLimitCount:1
+ Support to detect HID protocol USB connection and related operation(erase、program、verify etc...)
+ Update mass storage and hid protocol firmware file [54.07.19.0B]

-------------
Speech ICP Writer V1.09.000
-------------
[Feature]
+ Update F/W file(54.02.18.12)
+ Support to recognize TSSOP20 package type
+ Support N589D201/251/341/481
+ After connect D171 chip and burn into NSP171 obj, USB dongle / chip Board shows disconnect 
+ File combobox will record recently used files

-------------
Speech ICP Writer V1.08.000
-------------
[Feature]
+ Support N589A400/600/900,N589B480/650/960,N589C480/650/960,N589D650/960
+ The GUI will not always show upgrade firmware message continuously when choose to cancel update firmware until the application re-open
+ Chip size checking error at download object file to ICE in ICE driver.
+ Update firmware file(53.0C.0C.17)

-------------
Speech ICP Writer V1.07.000 
-------------
[Feature]
+ Encrypt UI setting file to avoid wrong modification by user
+ Show security lock bit status duration chip connection
+ To block the object type Normal N589 object file to program on N589 171 series chip board
+ Fix the problem to cause whole chip erase fail and program fail
+ Modify code about get PID and VID from device for some computer can't detect connection
+ Update last F/W file
+ Support new features on console mode
  - detect dongle connection and chip board connection
  - program flash object file 
  - program spiflash object file
  - check firmware version 
  - ISP command for NSP
+ Show prompt to close previous instance application if application already opened
+ Fix the check firmware function not work problem


-------------
Speech ICP Writer V1.06.000 
-------------
[Feature]
+ Distinguish USB dongle connection and chip connection message
+ Show shorter path name and complete filename on file browser.
+ Support NSP081 and NSP171 chip

-------------
Speech ICP Writer V1.05.000 
-------------
[Feature]
+ Update F/W file
+ Support N589D171 Seriese and NSP Series 
+ Update F/W will freeze problem
+ Support Console Mode
+ Fix the crash problem if the chip item is not support
+ Check target device size and lock option duration upload method

-------------
Speech ICP Writer V1.04.000
-------------
[Feature]
+ Detect the connection is (BP00,BP01) or (ICECLK,ICEDATA) and switch related online mode
+ When the object is SOP on online mode, show the warning message "When package type is SOP, please reserve BP00/BP01 for production programming."
+ Fix the crash problem for loading data or ICE connect on online mode

-------------
Speech ICP Writer V1.03.000 
-------------
[Feature]
+ Online Mode Show F/W Version Text
+ F/W Update
+ Support 4K Screen Resolution
+ N589 Confuguration Page Modify
+ Support N589D series chip

-------------
ICPWriter V1.02.000 
-------------
[Feature]
+ Program APROM and SPIFlash Data using 3 mode
  - Online ICE Mode
  - Online ICP Mode
  - Offline ICP Mode
+ Update F/W to NHS-ICE Device when detect Newer version
