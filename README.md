All installers are zipped with password: 123456

-------------
N566H - V1.06.000 SP10
-------------
[Bug-Fixed]
 * Inconsistence between Binary Code Checksum show on FRM file and checksum calculated by writer tool.


-------------
N566H - V1.06.000 SP9
-------------
[Feature]
 + Allow BTV 3.3V when 2 batteries for N566LPxx0(#0004045)
 
-------------
N566H - V1.06.000 SP8
-------------
[Bug-Fixed]
 * Remove the limitation of Precode that it can only run in certain network domain.
 
-------------
N566H - V1.06.000 SP7
-------------
[Feature]
 * Add setting of “hardware protection mode” in mask option for N566LP chip series.

-------------
N566H - V1.06.000 SP6
-------------
[Feature]
 + Adjust binary file format of N566LP chip series to be used as input file for EVB programming.

-------------
N566H - V1.06.000 SP5
-------------
[Bug-Fixed]
+ Pull High/Low 1M ohm will get back to 150K ohm after close mask option dialog

-------------
N566H - V1.06.000 SP4
-------------
[Feature]
 + Remove 330K ohm from MaskOption UI for N566LP
 + Remove 330K ohm from frm file for N566LP

[Bug-Fixed]
 + Mask option booster voltage is empty after open N566LP project
 
-------------
N566H - V1.06.000 SP3
-------------
[Feature]
 + Add support of play-by-index.

-------------
N566H - V1.06.000 SP2
-------------
[Bug-Fixed]
 + Update assembler to fix if statements bug
 + Avoid leaving too many files in temporary folder which cause NuIDE slow down.

-------------
N566H - V1.06.000
-------------
[Feature]
 + Add N566LP chip series supported
   1. N566LP120
   2. N566LP160
   3. N566LP200
   4. N566LP240
   5. N566LP280
   1. N566LP320
 + Add two more OTP chip bodies supported
   1. N566HP081 for N566H080
   2. N566KP081 for N566K080

[Modification]
 + Add HW PWM options

[Bug-Fixed]
 + Play [0ms] is illegal and SDS have to locate where is the problem
 