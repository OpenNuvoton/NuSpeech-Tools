-------------
N566H - V1.06.000 SP16
-------------
[Features]
+ Added support for SPI flash write protection, enabling users to define the write-protected area in the SDS and apply it to the SPI flash after downloading. Current list of supported chips:
 - 4Mbit (4 chips):Boya BY25Q40AW,Boya BY25D40ES,Zbit ZB25WD40C,Zbit ZB25WQ40A
 - 8Mbit (6 chips):Boya BY25Q80AW,Boya BY25Q80ES,Puya P25Q80SU,XTX XT25F08F,Zbit ZB25WD80C,Zbit ZB25WQ80A
 - 16Mbit (6 chips):Boya BY25Q16AW,Boya BY25Q16BS,Puya P25Q16SU,XTX XT25F16F,Zbit ZB25WQ16A,Zbit ZB25VQ16E
 - 32Mbit (4 chips):Boya BY25Q32ES,Puya P25Q32SL,XTX XT25F32F,Zbit ZB25VQ32
 - 64Mbit (4 chips):Boya BY25Q64ES,Puya P25Q64SH,XTX XT25F64F,Zbit ZB25VQ64C
 - 128Mbit (4 chips):Boya BY25Q128AS,Puya PY25Q128HA,XTX XT25F128F,Zbit ZB25VQ128D
 - 256Mbit (4 chips):Boya BY25FQ256ES,Puya PY25Q256HB, XTX XT25F256B,Zbit ZB25Q256A

-------------
N566H - V1.06.000 SP15
-------------
[Bug-Fixed]
* (FW) SET_VOL2 is ineffective

-------------
N566H - V1.06.000 SP14
-------------
[Features]
+ For the Mask IC of N566H080, check for violations related to executing programs from SPI flash in data-only regions.
  - After build project, an error will be displayed if any programs are located within the SPI flash address ranges xxx00280h–xxx002FFh and xxx3FA80h–xxx7FFFFh.
+ Documents revised and upgraded to PDF format. (Require at least NuIDE V4.00.000 SP2)

-------------
N566H - V1.06.000
-------------
[Features]
 + Added the display of internal ROM usage statistics (programs and resources) on the bottom-right graph in NuIDE

[Bug-Fixed]
 * For those instruments that do not contain real root key definition, instrument definitions of IDT table 
   are missing (this bug comes from SP11).
 * Show up memory information in Resource Editor .
   - Fixed an issue where text in the memory information section of the resource window was cut off when Windows display scaling was applied.
 

-------------
N566H - V1.06.000
-------------
[Bug-Fixed]
 * Failed to mute melody correctly.

-------------
N566H - V1.06.000 SP11
-------------
[Features]
 + Support for Dark Mode: Requires NuIDE version 4.00.000 or later
 + Adjust the brightness of the UIO curves according to the proportion by SET_EVOn_PWM_LEVEL, and SET_EVOn_PWM_LEVEL_RAM commands.
 + Enhance the auto-complete function and differentiate between ASM and PS project's keywords.
 + Check for any unused instruments and drums and display them in the output window.
 
[Bug-Fixed]
 *Fix minor GUI layout bug.
 
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
 
  -----------------------------
 All installers are zipped with password: 123456