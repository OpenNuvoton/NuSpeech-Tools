-------------
N567H - V3.04.000 SP6
-------------
Based On N567H_V3.04.000 SP5 and add the following issues.

[Features]
+ Add procedure of checking stack overflow.

-------------
N567H - V3.04.000 SP5
-------------
Based On N567H_V3.04.000 SP4 and add the following issues
[Modification]
+ SDS always output build target to Project_Folder\Code_Release\ then copy *.rbf and *.obj to sub-folder if NRES file name is different with project name.
+ Show "UNDEF" in resource window when meet undefined location of audio resource. Check defined audio resources at the beginning of building process.

-------------
N567H - V3.04.000 SP4
-------------
Based On N567H_V3.04.000 SP3 and add the following issues.

[Modification]
 + Adjust handling of added-by-code audio resource information, and fine-tune procedure of on-line encoded size estimation.
 
-------------
N567H - V3.04.000 SP3
-------------
Based On N567H_V3.04.000 SP2 and add the following issues.

[Feature]
 + Add LED flash frequency check function.
 
[Bug-Fixed]
 + It has change to crash after converting MIDI file.
 + Value of Call Layer is changed to 0 after opening Pin Mappings dialog.
 + Allow to type '-' (hyphen) in project name.
    
-------------
N567H - V3.04.000 SP2
-------------
Based On N567H_V3.04.000 SP1 and add the following issues.

[Fixes]
 + Different debounce in FXF15 TG will have chance to cause all keys become unable to response.
 
-------------
N567H - V3.04.000 SP1
-------------
Based On N567H_V3.04.000 and add the following issues

[Features] 
 + UltraIO keep value function changed to keep level.
 + Add EN_INT, EN_INT_QUIT commands to control interrupt.

[Fixes]
 + Modify sound library for user one key one note function.
 + Fix delay compiler error bug. When enable IO expander and cap sensor, calling delay macro may cause compiling error(related jump too long).
 + Fix Functionality of ultraio pin configured as FW PWM would be invalid after waking up from sleep.

-------------
N567H - V3.04.000
-------------
Based On N567H_V3.03.000 SP1 and add the following issues.

[Features] 
+ Convert UltraIO output with reference the LED active low or high flag in WIO file.
+ Support normal user to install program in user folder instead of C:\ root drive.
+ Correct problem about different rbf size after each audio resource converting.
    
[Fix]
+ Prevent user from changing chip to N567H/K/G 120,160,200.
