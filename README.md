-------------
OTP writer V2.12.000
-------------
[Feature]
+ Support these new parts
  - N566HP161 TSSOP20/TSSOP28
  - N566HP200 TSSOP20/TSSOP28
  - N566HP240 TSSOP20/TSSOP28
  - N566HP280 TSSOP20/TSSOP28
  - N566HP321 TSSOP20/TSSOP28
  - N566KP240 TSSOP20/TSSOP28

-------------
OTP writer V2.11.000
-------------
[Feature]
+ Support these new parts
  - N566LP120 TSSOP20/TSSOP28
  - N566LP160 TSSOP20/TSSOP28
  - N566LP200 TSSOP20/TSSOP28
  - N566LP240 TSSOP20/TSSOP28
  - N566LP280 TSSOP20/TSSOP28
  - N566LP320 TSSOP20/TSSOP28

[Bug-Fixed]
+ Fixed show error message: “PDID showing 0xFFFFFFFF” when loading any object file without dongle plugged in.

-------------
OTP writer V2.10.000
-------------
[Feature]
+ N566KP320 can be programed with N566KP320~240, N566GP320~240 object file
+ N566KP200 can be programed with N566KP200~120, N566GP200~120 object file
+ N566GP320 can be programed with N566GP320~240 object file
+ N566GP200 can be programed with N566GP200~120 object file
+ Support N588LP122~N588LP322
+ Support new “enable hardware protection” mask option of N566LP and N588xx2 chip series

-------------
OTP writer V2.09.000
-------------
[Feature]
+ Add on-line mode can create program status excel log

-------------
OTP writer V2.08.000
-------------
[Feature]
+ Add N566LP120/160/200/240/280/320 chip support

-------------
OTP writer V2.07.000
-------------
[Feature]
+ Add N584P070/040 chip support
+ Add N584P300/260/210 chip support
+ Add N566HP081, N566KP081 chip support

-------------
OTP writer V2.06.000
-------------
[Feature]
+ Add N584P170/120 chip support
+ Add N588H, N584P UCID value check
+ Fixed N584, N566, N588HP series when chip have test code lead to program after play no sound.
+ Support N566HP/GP/KP program small size of OBJ file to larger size of N566 OTP chip

-------------
OTP writer V2.05.000
-------------
[Feature]
+ Add Lapis OTP have normal and factory firmware check
  - Fixed N567/N588LP330 two battery and select 3.3v but set 4.2v on chip
  - Fixed N566HP330(80) chip can’t block N566LP object file to program and verify
  - Fixed N566HP080 on-line mode can’t detect chip after program behavior

-------------
OTP writer V2.04.000
-------------
[Feature]
+ Modify N588xx2HP chip load size rule like as, 
  - N588HP342 chip can load N588H/J342-202 object file, 
  - N588HP172 chip can load N588H/J172-122 object file, 
  - N588HP082 chip can load N588H/J082-062 object file
+ Modify N588xx2H/JP series can load object rule, like as
  - N588xx2HP chip can load N588xx2H/J object file, but 
  - N588Jxx2 chip only can load N588xx2J object file.
+ Modify N566H, N588H when chip have test code didn’t overwrite it.  
+ Change log file directory from root to temporary.

-------------
OTP writer V2.03.000
-------------
[Feature]
+ Support N588H/JP 062,082,202,252,342

-------------
OTP writer V2.02.000
-------------
[Feature]
+ Support N588H/JP 122,172

-------------
OTP writer V2.01.000
-------------
[Feature]
+ Support N566HP/GP/KP080, 120, 160, 200, 240, 280, 
+ Support N566HP321, N566KP320, N566GP320

-------------
OTP writer V2.00.000
-------------
[Feature]
+ Support N566HP321/ N566HP281 / N566HP241
+ Support N566KP321/ N566KP281 / N566KP241
+ Support N566GP321/ N566GP281 / N566GP241
+ Support N588J/H 480 OTP chips
+ Check N588J/H OTP chips

