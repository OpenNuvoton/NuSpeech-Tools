All installers are zipped with password: 123456

-------------
NuIDE_V3.08.000 (2022/05/12) SP6
-------------
Based on V3.08.000 SP5 and add the following issue.
[Features]
+ Show N589 flash size of program, resource and not limit code bank only 4.

[Bug-Fixed]
+ Wrong encode name shown on duration field of N589 SDS.
+ Range of Min/Max values of Duration not work well.
+ N589E duration info of chip selector.

-------------
NuIDE_V3.08.000 SP5 (2022/01/27)
-------------
Based on V3.08.000 SP4 and add the following issue.

[Features]
+ Online version check and auto-install selected version.

[Bug-Fixed]
+ Install SDS to a path other than the default installer folder, “New” Project will fail.
+ Keep clicking on "Reset Filters" in chip selector window then the chip items will be increased.
+ Breakpoint window shows address instead of file name(dasm.txt) if breakpoint is set in disassembler window.
+ NuBuildProjectTool can't work successfully.

-------------
NuIDE_V3.08.000 SP4
-------------
Based on V3.08.000 SP3 and add the following issue.

[Features]
+ Support N589 SDS V1.08.000 and later version
+ Forbidden standalone N589E SDS. Please install N589 SDS V1.08.000 to develop N589E project.

[Bug-Fixed]
+ Remove NUO duration information for N589E
+ Modify duration calculation for N589E

-------------
NuIDE_V3.08.000 SP3
-------------
Based on V3.08.000 SP2 and add the following issue.

[Bug-Fixed]
+ Stop showing tool tip of variable value for C language.
+ Opening file from Include Window has wrong lexer keyword color.
+ Add .c as known extension which can be compiled, so opening .c file in editor would let “Compile” menu item enabled.

-------------
NuIDE_V3.08.000 SP2
-------------
Based on V3.08.000 SP1 and add the following issue.

[Features]
 + SDS support NSD format
 + SDS support N589E SDS

-------------
NuIDE_V3.08.000 SP1
-------------
Based on V3.08.000 and add the following issue.

[Features]
+ The lexers editor symbol color for C project
+ Memory layout window will show the global symbol start address, end address, and size information
+ Memory layout window will show the module size information
+ The same address and the label name is different with the "_",  with "_" label name position is in front of none "_" label name, and show end address and size information on none "_" label name on memory layout window

[Fix]
+ The new Register Window flashes after being added. (mantis:3152)
 
-------------
NuIDE V3.08.000
-------------
Based on V3.07.000 SP5 and add the following issue.

[Features]
+ Preview the UltraIO file that will refer the shift position value
+ Check the open path is directory or file before open document to avoid program crash
+ Watch window don't show address in value item like (value) yyy:zzz
+ Support JP code-page
+ Save/Open should show correct file extensions in File Dialog depends on current project type
+ Save as file with new extension will change its parser method immediately

[Fix]
+ Avoid showing mask option twice when user change mask option and need wizard reload
+ To expand sub item of Watch window will cause crash (mantis:2986)
+ ASM/PS/C instruction window hang up (mantis:3086)
+ Unable to turn off Check for Updates (mantis:3064)
+ Find & Replace layout. Fix: The editor to enter finding string has string length limit.(#3032)
+ Quick find combobox in toolbar cannot work (#3034)
+ No error message when invalid directory path (mantis:3040)
+ Change display format of array variables in Watch window (mantis:3124)