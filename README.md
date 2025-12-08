
-------------
N588H - V3.15.000 SP12
-------------
Based on N588H_V3.15.000 SP11 and provide the following new issue.
[Feature] 
 + Support resource window on dark mode
 + Warning about the current system clock may not be sufficient if the speech synthesis process demands excessive computing power. 
   All analysis data kept in "Code_Release\AudioPlaybackProfile\PlaybackProfile.csv".
 + Added the display of internal ROM usage statistics (programs and resources) on the bottom-right graph in NuIDE
 
[Bug-Fixed]
 * N588H crash during project builds with NuIDE V4.00.000
 * Resource size information area does not resize to fit font size.
 
-------------
N588H - V3.15.000 SP11
-------------
Based on N588H_V3.15.000 SP10 and provide the following new issue.
[Feature] 
+ Support RAM version of play MIDI external note for ASM and PS project.
+ Remove mask option suggest message about LVR.
 
[Bug-Fixed]
+ Play midi+stop all+play midi，midi is not be played.(#0003860) 
+ Play speech+stop all+ext note on，ext note is not be played.(#0003861)

-------------
N588H - V3.15.000 SP10
-------------
Based on N588H_V3.15.000 SP9 and provide the following new issue.
[Feature]
+ For N588[H|J]Pxx2, always generate \Code_Release\ICProgrammingService\*.zip which contains *.bin and *.p



-------------
N588H - V3.15.000 SP9
-------------
Based on N588H_V3.15.000 SP8 and provide the following new issue.
[Bug-Fixed]
+ Comment lines are removed after pressing Apply button

-------------
N588H - V3.15.000 SP8
-------------
Based on N588H_V3.15.000 SP7
[Feature]
+ Extend keypad, trigger key, mode key de-bounce time to 400ms

[Modification]
+ Adjust multi-NRES mechanism
+ PS compiler automatically detect section and replace JP/CALLL as LJP/LCALL if need
+ TABLE_LOOKUP macro changed to instructions to detect cross-bank access by PS compiler

[Bug-Fixed]
+ PSF code-gen – Auto-Remarking issue
+ Parsing .map file incorrectly and caused IDE shows wrong information
+ FW – Failed to execute ASM macro – SET_PORT_OUTPUT_0 PORT_INDEX, PIN_MASK under the following circumstances
  - Apply to BP2
  - Disable UIO

-------------
N588H - V3.15.000 SP7
-------------
Based on N588H_V3.15.000 SP6 and provide the following new issues.
[Bug-Fixed]
+ If pattern event is applied, auto enable converted pins.
+ User event should be kept if the event index in patten event table is reserved type.
	
-------------
N588H SDS V3.15.000 SP6
-------------
Based on N588H_V3.15.000 SP5 and provide the following new issues.

[Feature]
+ Handle CFG7.5 LVD function for new version of N588H000 ICE chip.

[Bug-Fixed]
+ Handle comment code incorrectly to cause crash.

-------------
N588H SDS V3.15.000 SP5
-------------
Based on N588H_V3.15.000 SP4 and provide the following new issues.

[Bug-Fixed]
+ Key matrix has chance to be unable to wakeup if debounce time is small.
+ Generate wrong code for BP2 mode pin.
+ Key scan bug when using "if(inputkey=[0])" chip would cause reset.

-------------
N588H SDS V3.15.000 SP4
-------------
Based on N588H_V3.15.000 SP3 and provide the following new issues.

[Bug-Fixed]
+ If no any TG/mode pin/key matrix was enabled, the value of IEF0 would be wrong when entering POI.
+ PS Initial RAM Clear bug.
+ Add UltraIO HW PWM shared pin information to provide output init module more info and avoid output incorrect behavior.
+ Linker report incorrect size.
+ Allow to type '-' (hyphen) in project name(#0003184)

-------------
N588H SDS V3.15.000 SP3
-------------
Based on N588H_V3.15.000 SP2 and provide the following new issues.

[Bug-Fixed]
+ Volume Meter and LED VC error of SOP8. 
+ Output=x error of SOP8
    
-------------
N588H SDS V3.15.000 SP2
-------------
Based on N588H_V3.15.000 SP1 and provide the following new issues.

[Feature]
+ Allow to type '-' (hyphen) in project name on Project Duplicator Window(#3184)

[Bug-Fixed]
+ Hide the Global EQ UI
+ Duplicated project has an empty "Include" folder(#3161)

-------------
N588H SDS V3.15.000 SP1
-------------
Based on N588H_V3.15.000 and provide the following new issues.

[Bug-Fixed]
+ The N588H chip will enter STOP mode while executing WDT or SET_LVD_xxV if ‘ENTER_SLEEP’ was once executed before
+ Lower down the execution time of CHECKSUM macro.
+ Change macro name ENTER_SLEEP to ENTER_STOP. Help & keyword color shows the new macro name but keep the old one in code for backward compatibility.


-------------
N588H SDS V3.15.000
-------------
Based on N588H_V3.14.000 SP5 and provide the following new issues.

[Feature]
+ Handle LVD SFR issue.
    
[Bug-Fixed]
+ Crash when preprocessor handle Japanese code.(#3069)
+ Update code for shift sample position parameter on UltraIO file and fix some build fail problem
+ Modify the code that play by index waiting channel for EVO file
