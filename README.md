
-------------
N584H SDS V1.03.000 SP4
-------------
Based on SDS V1.03.000 SP3 and add following issue.

[Features]
+ Supported resource window dark mode
+ Added the display of internal ROM usage statistics (programs and resources) on the bottom-right graph in NuIDE
+ Added support for viewing documents in PDF format. (Requires NuIDE version V4.00.000 SP2 or later.)
+ Revised documents.

[Bug-Fixed] 
+ Fixed an issue where text in the memory information section of the resource window was cut off when Windows display scaling was applied.
 
-------------
N584H SDS V1.03.000 SP3
-------------
Based on SDS V1.03.000 SP2 and add following issue.

[Feature]
 + Add new option - 0 ms debounce setting for direct trigger.
 
-------------
N584H SDS V1.03.000 SP2
-------------
Based on SDS V1.03.000 SP1 and add following issue.

[Bug-Fixed]
+ Update FW and codegen to fix UltraIO FW PWM level Resolution < 14, the LED flashing is wrong
	
-------------
N584H SDS V1.03.000 SP1
-------------
Based on SDS V1.03.000 and add following issue.

[Bug-Fixed]
+ Converting some kinds of MIDI file would cause crash. 

-------------
N584H SDS V1.03.000
-------------
Based on SDS V1.02.000 SP2 and add following issue.

[Features]
+ Add chip items:
  1. N584P300,N584P300_SOP8,N584P300_TSSOP20,N584P300_LQFP48
  2. N584P260,N584P260_SOP8,N584P260_TSSOP20,N584P260_LQFP48
  3. N584P210,N584P210_SOP8,N584P210_TSSOP20,N584P210_LQFP48
  4. N584P170,N584P170_SOP8,N584P170_TSSOP20,N584P170_LQFP48
  5. N584P120,N584P120_SOP8,N584P120_TSSOP20,N584P120_LQFP48
  6. N584P070,N584P070_SOP8,N584P070_TSSOP20
  7. N584P040,N584P040_SOP8,N584P040_TSSOP20
+ Can install SDS without administrator right

[Bug-Fixed]
+ Fix the issue that PLAYW EVO will not wait for the end of the playback to continue running.
+ Fix: Format menu didn't show correctly in resource window. Volume Boost menu didn't show selected item in resource window.
+ Hide FW PWM Frequency option in UltraIO Property Dialog.
+ Use lower case letter in equation name would cause play by index mechanism linking error. 
+ If resource is edited, building project would cause linking error that cannot find resource section.
+ After switching chip the SDS didn't force rebuild project so it link the wrong .lic and cause linking error.
+ Some optional Functions are not saved after close then open project.
+ Make unused pins to be output low to avoid currency leakage.

