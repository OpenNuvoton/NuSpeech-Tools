-------------
Gang Writer Release Note
-------------
Speech Gang Writer V2.03.000
-------------
[Features]
+ Support for chips N589D086, N589D126, and N589D176 package SOP8, SOP14, TSSOP20
+ Add checksum-based verification to confirm whether the .obj file matches the content previously written to flash.
  - Should update FW [00.00.02.00] to write checksum information into flash

-------------
Speech Gang Writer V2.02.000
-------------
(1) Support chip N589D176(TSSOP20)

=================================================
============Speech Gang Writer_V2.01.000=========
============Date: 2025/06/17=====================
=================================================
(1) support for programming SPIFlash with the N589LS00 TSSOP28 package
(2) update help document
(3) update firmware file(00.00.01.09)

=================================================
============Speech Gang Writer_V2.00.000=========
============Date: 2025/03/07=====================
=================================================
(1) upgrade the build platform from Visual Studio 2010 to Visual Studio 2022
(2) support chip N589L080
(3) support chip N589S080
(4) support these N589LS series chip: N589LS[00|08|16|32|64]
(5) support programming and verifying SPIFlash content for these chips
  (a) N589B340,N589B250,N589B200,N589B170,N589B120,N589B080(TSSOP28)
  (b) N589B345,N589B255,N589B205,N589B175,N589B125,N589B085(TSSOP28)
  (c) N589B650 (DIE)

=================================================
=           Speech Gang Writer_V1.09.000        =
=           Date: 2024/02/29                    =
=================================================
(1) support chip N589D655/N589D965

=================================================
=           Speech Gang Writer_V1.08.000      	=
=           Date: 2023/11/22                    =
=================================================
(1) support chip N36D65

=================================================
=           Speech Gang Writer_V1.07.000      	=
=           Date: 2023/09/28                    =
=================================================
(1) support chip N589L120/N589L170/N589L200/N589L250/N589L340
(2) add N589L chip mask option configuration
(3) update firmware file(00.00.01.04)

=================================================
=           Speech Gang Writer_V1.06.000      	=
=           Date: 2023/03/21                    =
=================================================
(1) support chip N589B965/N589B655/N589B485
(2) support chip N589D485/N589D345/N589D255/N589D205

=================================================
=           Speech Gang Writer_V1.05.000      	=
=           Date: 2022/09/30                    =
=================================================
(1) support chip N589D175/N589D125/N589D085
(2) support chip N589E081/N589E061/N589E041

=================================================
=           Speech Gang Writer_V1.04.000      	=
=           Date: 2022/06/21                    =
=================================================
(1) update firmware file(00.00.01.00)
(2) support chip N589B345/N589B255/N589B205/N589B175/N589B125/N589B085

=================================================
=           Speech Gang Writer_V1.03.000      	=
=           Date: 2021/09/30                    =
=================================================
[Note]
(1) support these new chip
	(a)N589A1K4/A1K9
	(b)N589B1K5/B2K0/BK5B/BK5F/BK5L/B2KB/B2KF/B2KL
	(c)N589C1K5/C2K0/CK5B/CK5F/CK5L/C2KB/C2KF/C2KL
	(d)N589D1K5/D2K0/DK5B/DK5F/DK5L/D2KB/D2KF/D2KL
	(e)N589E040/N589E060/N589E080
	(f)NSC128DF/192DF/384DF/512DF/768DF/1K0DF
	(g)NC9008/9017/9034/9048/9065/9096
(2) update firmware file(00.00.00.0C)

=================================================
=           Speech GangWriter_V1.02.000      	=
=           Date: 2020/06/09                    =
=================================================
[Note]
1. support these new chip
(a) N589A400/600/900
(b) N589B480/650/960
(c) N589C480/650/960
(d) N589D650/960
(e) N589D201/251/341/481
2. update firmware file(00.00.00.08)
3. modify the code to check connection PID and VID is match or not

=================================================
=           Speech GangWriter_V1.01.000      	=
=           Date: 2019/03/27                    =
=================================================
[Note]
1. Support NSP Chip
2. Update F/W file
3. UI Adjustment(Menu Icon、Tab Icon)
4. Support NSP081、NSP171

=================================================
=           N589 GangWriter_V1.00.000      	=
=           Date: 2018/09/19                    =
=================================================
[Note]
1. Support to download and verify the APROM data and SPI-Flash data.
2. Supported Chips: N589A、N589B、N589C、N589D Series Chips.
