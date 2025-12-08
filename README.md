
-------------
N588L_V1.07.000 SP5 
-------------
[Features]
* Documents revised and upgraded to PDF format. (Require at least NuIDE V4.00.000 SP2)
* Added the display of internal ROM usage statistics (programs and resources) on the bottom-right graph in NuIDE
* For N588LP, added commands to adjust the brightness of the UIO curves according to the proportion through SET_EVOn_PWM_LEVEL and SET_EVOn_PWM_LEVEL_RAM commands.

[Bug-Fixed]
* Fixed bug that the UlraIO event could be missed under certain circumstances.
* Fixed an issue where text in the memory information section of the resource window was cut off when Windows display scaling was applied
* For N588L, Fixed the bug that the saved path will become longer and longer by constructing path by the ".\" string every time when the project was opened. Although the path is still correct, the building process will crash eventually if the path was too long.

-------------
N588L SDS V1.07.000 SP4
-------------
[Features]
* Added support for dark mode when used with NuIDE version 4.00.000 or later
* Updated documentation.
[Bug-Fixed]
* Fixed various GUI issues.
* Adjusted the order of the request form to match the layout of the mask option GUI.

-------------
N588L SDS V1.07.000 SP3
-------------
[Bug-Fixed]
* Inconsistence between Binary Code Checksum show on FRM file and checksum calculated by writer tool.

-------------
N588L SDS V1.07.000 SP2
-------------
Based on N588L V1.07.000 SP1 and add the following issues.
[Feature]
* Allow BTV 3.3V when 2 batteries for N588LP(#04045)
[Bug-Fixed]
* Remove the limitation of Precode that it can only run in certain network domain.

-------------
N588L SDS V1.07.000 SP1
-------------
Based on N588L V1.07.000 and add the following issues.
[Feature]
+ Rename N588LP332 to N588LP322.
+ Support generating binary file for EVB programming. (N588LP)
+ Add option "Hardware Protection Mode" in mask options. (N588LP)


-------------
N588L_V1.07.000
-------------
Based on N588L V1.06.000 SP3 and add the following issues.
[Feature]
+ Add chip items: N588LP122/N588LP162/N588LP202/N588LP242/N588LP282/N588LP332.


-------------
N588L SDS V1.06.000 SP3
-------------
Based on N588L V1.06.000 SP2 and add the following issues.

[Features]
+ Add N588Lxx1 chip series
 
[Bug-Fixed]
+ Incorrect code-generation of key-matrix table

-------------
N588L SDS V1.06.000 SP2
-------------
Based on N588L V1.06.000 SP1 and add the following issues.

[Features]
+ Improvement on UIO code-generation
 
[Bug-Fixed]
+ For these equations with silence inside, if we do not use these equations in user program, it will lead to linking error.

-------------
N588L SDS V1.06.000 SP1
-------------
Based on N588L V1.06.000 and add the following issues.

[Features]
 + HW PWM Frequency show real frequency instead of clock source.
 
[Bug-Fixed]
 + FW PWM Frequency option didn't contain in modification list so it do not update if it was changed individually
 + Apply HW PWM Frequency option to codgen.
 + Allow to type '-' (hyphen) in project name(#0003184)

-------------
N588L SDS V1.06.000
-------------
Based on SDS V1.05.000 and add the following issues.

[Features]
+ Support play by index function.
+ Support to apply the property about shift sample position on UltraIO file.
