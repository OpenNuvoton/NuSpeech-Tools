
-------------
NuIDE_V4.00.000 SP4
-------------
Based on V4.00.000 SP3 and add the following issue.

[Features]
 + Support enhanced Memory Layout Window for clear visualization of RAM and ROM usage.
 + Display predefined handlers, allow to select a handler to navigate to its code position or create it if it does not already exist.
 
[Bug-Fixed]
 + Fixed: editor’s reload mechanism which could be failed under some circumstances.
 + Fixed: After uninstalling an SDS, clicking the "Refresh List" button in the SDS List dialog does not display all existing SDS entries that come after the deleted one
 + Fixed: an issue where editing and saving UTF8-encoded files would not trigger the save button in the GUI, due to inconsistent SavePoint status between Scintilla and NuIDE.

-------------
NuIDE_V4.00.000 SP3
-------------
Based on V4.00.000 SP2 and add the following issue.

[Features]
+ Support IDT UI mode.
+ Support project type “Powerscript with C”.
+ Support getting tab control icons from SDS and displaying them on the tab control of the Library Settings Window.
+ Added duplicate ICON in toolbar.

[Bug-Fixed]
+ Fixed: The invoked installer cannot complete the flow when updating NuIDE.(# 0004319)
+ Fixed: When load and reload among SDS, the use of chipinfo.dll should be loaded from each SDS instead of using firstly loaded one.
+ Fixed: When loading the N588LP, an error message saying “Failed to load chip information” appears, even though the information has actually loaded correctly.
+ Fixed: The external tools' ICON cannot show in Docking Toolbar.
+ Fixed an issue where the theme style of the Library Setting window was lost after opening the Option window or applying settings.

-------------
NuIDE_V4.00.000 SP2
-------------
Based on V4.00.000 SP1 and add the following issue.

[Features]
+ Support viewing PDF format document.
+ Update Icons for docking window and file types
+ Enlarge the width of bottom-right RAM/ROM information box for new information containing percentage of program/resource used ROM.
+ Added menu to show external tools of opened SDS.

-------------
NuIDE_V4.00.000 SP1
-------------
Based on V4.00.000 and add the following issue.

[Features]
+ Add search function to instruction help window
+ Enhanced version updater
   - Only show version check result at NuIDE open
   - Provide release note information
   - Can skip this new version and prompt at newer version detected
   - Do not show this updater within today

-------------
NuIDE_V4.00.000
-------------
Based on V3.08.000 SP9 and add the following issue.

[Features]
 + Change NuIDE icon
 + Support dark mode.
 + Save the settings of the Find & Replace dialog and restore them when reopening the dialog.
 + Support the cloning of service packs as standalone versions.
 + Modify the method to open projects with a different SDS version than the default SDS version
   If the project's SDS version doesn't match the default SDS version, prompt to decide how to open project.
	- If choose "Yes", the NuIDE will open the project with the default SDS.
	- If choose "No" , the NuIDE will open the project with the SDS version specified in the project. If the specified version isn't found in the system, NuIDE will ask to install it.
 
 [Bug-Fixed]
 + When opening a new file and using the 'Save As' function to save it as a new file, it does not save it as a new file.(#3898)


-------------
 NuIDE_V3.08.000 SP9
-------------
Based on V3.08.000 SP8 and add the following issue.

[Bug-Fixed]
+ Resolve the problem causing the failure to create a new N589E project

-------------
 NuIDE_V3.08.000 SP8
-------------
Based on V3.08.000 SP7 and add the following issue.

[Feature]
+ Support N589L340 and N36D65 chip.


-------------
 NuIDE_V3.08.000 SP7
-------------
Based on V3.08.000 SP6 and add the following issue.

[Features]
+ New formula for chip duration calculation with UltraIO(#0003773)
+ Show filter note on chip selector dialog(#0003803)

[Bug-Fixes]
+ Fix: allow user to directly press F5/F9/F10 etc.. hot key to continue after entering debugger without the need to press the main frame again.
+ Caret of GotoLine dialog will be set at input box right after dialog was opened.
+ For some string token which start with number but mixed with other characters cannot be highlighted as number color.


-------------
NuIDE_V3.08.000 SP6
-------------
Based on V3.08.000 SP5 and add the following issue.

[Features]
+ Show N589 flash size of program, resource and not limit code bank only 4.

[Bug-Fixed]
+ Wrong encode name shown on duration field of N589 SDS.
+ Range of Min/Max values of Duration not work well.
+ N589E duration info of chip selector.

-------------
NuIDE_V3.08.000 SP5
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
