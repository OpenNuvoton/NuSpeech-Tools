All installers are zipped with password: 123456

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
