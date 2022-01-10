All installers are zipped with password: 123456

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