
------------
UltraIO V6.11.000
------------
Based on UltraIO_V6.10.000 SP10

[Features]
1. Change spline curve, triangle, envelope curve editing window layout
2. Support motor mode on curve pin
3. Support frequency transition function for flashing, sine, and triangle curve
4. Change the ruler unit to a more appropriate measurement.
5. Upgrade the building tool from visual studio 2010 to visual studio 2022

------------
UltraIO V6.10.000 SP10
------------
Based on UltraIO_V6.10.000 SP9

[Features]
1. scale bitmap width and height to fit the row and column number on SLED "import Bitmap file" function
2. advance simulation redo and undo function
3. rename the UI word from "morphing/fading" to "transition" and update help document

[Bug Fixed]
1. fixed press mouse wheel then scroll up/down but scroll waveform to right/left. Should scroll waveform to left/right
2. fixed press mouse wheel then move mouse to left/right but scroll waveform to left/right. Should scroll waveform to right/left
3. fixed advance simulation play can't display curve color
4. fixed some window mouse scroll feature not working
5. fixed can't import problem that the first item interval is 0 and the format is BMP on SLED "import Bitmap file" function
6. fixed Waveform view window display error at select region in waveform editor [Mantis:4195]

------------
UltraIO V6.10.000 SP9
------------
Based on UltraIO_V6.10.000 SP8

[Features]
1. support to press and drag the middle mouse button will move waveform left or right
2. support to scroll middle mouse button up or down will move waveform left or right
3. support to hold on "Ctrl" key and scroll middle mouse button up or down will zoom in or zoom out waveform.
4. support to import UltraIO setting file (xxx.reg) from help menu
5. add "UltraIO Tool User Guide.pdf" into Document folder on application folder 

[Bug Fixed]
1. Resolve the issue where modifying the starting position of the energy curves causes an unintended change in the overall shape of the curves, which should remain consistent regardless of the starting position adjustment.

------------
UltraIO V6.10.000 SP8
------------
Based on UltraIO_V6.10.000 SP7

[Features]
1. Enhance LED flash frequency checking with customized sampling rate not according to waveform sample rate
2. Can see flash detect error reason and its position
3. Can adjust ALED output by gamma correction setting

[Bug Fixed]
1. simple simulation result is incorrect at zoom in waveform then choose new playback position

------------
UltraIO V6.10.000 SP7
------------
Based on UltraIO_V6.10.000 SP6

[Feature]
1. implement to soften transition at color flyer control pointer on color flyer setting window or event view
2. implement to export current UltraIO registry setting for debug customer window environment on menu [Help | Export UltraIO setting]
3. ensure the simulation view is visible and start play when click menu [Run | Simulation | Simple Simulation]
4. check and modify the serial LED color pixel information must be smaller than max sample position when load WIO file
5. check and modify the serial LED color pixel information must be smaller than max sample position when generate the play ALED data

[Bug Fixed]
1. import SLED data from WIO file without checking scale option does not cut those ALED data after last PCM sample.
2. waveform, curve edit, curve view panel height is incorrect when setting different screen font size.

------------
UltraIO V6.10.000 SP6
------------
Based on UltraIO_V6.10.000 SP5

[Feature]
1. speed up to parse Vixen CSV data to SLED data
2. modify curve list view layout
  (a) change the active low icon picture
  (b) add blank between tree node text and icon

------------
UltraIO V6.10.000 SP5
------------
Based on UltraIO_V6.10.000 SP4

[Feature]
1. modify the new layout to import SLED data from Vixen data window
  (a) add [Replace serial LED data] or [Append serial LED data] selection on serial LED mode
  (b) add [Scale data to fit waveform] selection on serial LED mode
  (c) remove color mode selection
  (d) remove sample selection on timing group
  (e) show wire scan order setting if selected serial LED group is matrix mode
2. add advance simulation to support SLED edit and play
3. modify UIO batch merge convert window
  (a) add grid line to control lists
  (b) add auto LED flash frequency restriction to [WAV->WIO] and [WIO->WAV]
  (c) fix the problem that the triangle curve disappear after importing with option SCALE
4. update reset layout registry file to clear more layout data

------------
UltraIO V6.10.000 SP4
------------
Based on UltraIO_V6.10.000 SP3

[Bug Fixed]
1. fix the wrong action that import Vixen format data to serial LED group with array type’s matrix mode

------------
UltraIO V6.10.000 SP3
------------
Based on UltraIO_V6.10.000 SP2

[Bug Fixed]
1. fix to display the wrong waveform view data if all wave data is silence

------------
UltraIO V6.10.000 SP2
------------
Based on UltraIO_V6.10.000 SP1

[Feature]
1. Support automatically detect sample per group for mono and color envelop to pass LED flash detection.


------------
UltraIO V6.10.000 SP1
------------
Based on UltraIO_V6.10.000

[Feature]
1. support to move splitter to change the waveform view, curve edit, and curve view
2. show full path tool tip text when mouse move enter combobox control on batch mode window
3. check and show error message if the wave file is not 16-bit PCM format
4. Add sample per group option in the color envelope curve.
5. Relayout color envelope dialog to have more margin between controls. 
6. "Apply to All" button move to the place closed to Morphing which is the checkbox "Apply to All" apply to.
7. Add "Shift Curve Start Index" menu item function on menu Options

[Bug Fixed]
1. Apply the morphing option to the control points of color envelope curve.
2. fix to add multiple files but add files count is not match with selected files on batch mode window
3. fix to open unsupported PCM format file but add file path to the file list

------------
UltraIO V6.10.000
------------
Based on UltraIO_V6.09.000 SP4

[Feature]
1. new serial LED functions
   a. copy serial LED time points and paste to another UltraIO file then scale time points position to fit target file
   b. copy serial LED group and paste to another UltraIO file then scale time points position to fit target file
   c. support to add multiple time points on serial LED group by right-mouse clicking on Serial LED event view
   d. support to pick color by right-mouse clicking on color pixel panel
   e. limit Serial LED max LED count to 256
2. import serial LED data in batch mode
3. import Vixen format CSV file using menu [File | Import Vixen format data from CSV file]
4. support LED flash check function using menu [Run | Run LED Flash Check] with set frequency range and set ignore to change message color
5. insert silence function that select a region on waveform view and using menu [File | Insert Silence]
6. delete selected waveform function that select a region on waveform view  and using menu [File | Delete Selected Waveform]
7. add de-bounce time between left-mouse down and mouse move to avoid moving time point easily
8. set default silence sample rate is 8000 after open new silence window
9. update UltraIO user guide document

[Bug Fixed]
1. fix crash problem that generate the RGB group action
2. fix crash problem that generate color flyer curve but doesn't select all curve pins on color group
3. fix select multiple files then add into file list but some files will be lost

------------
UltraIO V6.09.000 SP4
------------
Based on UltraIO_V6.09.000 SP3

[Feature]
1. record the last enable option for "Enable color Range By Wave Length"
2. enable serial LED fading setting
3. modify the time and sample rate limitation for creating silence wave file
  a. time length must be bigger than 1 (ms)
  b. sample rate must be bigger than 30 (sample/second)
4 check total used memory size to show waveform and curve information for creating silence wave file

------------
UltraIO V6.09.000 SP3
------------
Based on UltraIO_V6.09.000 SP2

[Feature]
1. implement the global shift sample function of all UltraIO curves at [WAVE->WIO] mode on UltraIO batch merge generator
2. implement "Move All Curves..." function to move all curves on selected curve pins ([Menu]->[Curve]->[Move All Curves...])

------------
UltraIO V6.09.000 SP2
------------
Based on UltraIO_V6.09.000 SP1

[Feature]
1. There is only one serial LED group will be enable
2. On curve list view if the user enable/disable curve and this curve is not selected, the other selected curves will not be enable/disable
3. If exist the checked group item on serial LED, the serial LED group will be set checked

------------
UltraIO V6.09.000 SP1
------------
Based on UltraIO_V6.09.000

[Bug Fixed]
1. Show "End Position must be larger than Start Position" error message at pressing energy curve apply button twice when display unit is time.

------------
UltraIO_V6.09.000
------------
Based on UltraIO_V6.08.000

[Feature]
1. Support address LED setting

[Bug Fixed]
1. In the absence of the wave file, setting the Envelope Control Curve Dialog to press ok does not work.		(#2649)
2. Revised Nuvoton link for About UltraIO										(#2651)
3. UI shows only part of whole view after several steps									(#2448)
4. Fix the Polyline and Spline import fail problem using scale function if the first point's sample is 0
5. Fix the repeat segment event insert more than max range problem if select all region and use ms unit interval

------------
UltraIO V6.08.000
------------
Based on UltraIO_V6.07.000

[Feature]
1. Update help document about color picker view

[Bug Fixed]
1. If the UltraIO default not enable any curve pin, it will not enable the first curve pin or group automatically	(#2452)
2. Should active color pickup view "apply" button and customer color view at color curve control point selected		(#2304)
3. Should remove the index in color pickup view										(#2305)
4. Operation causes Color Picker View not to appear completely								(#2621)
5. Change the value of Red/Green/Blue in Color Picker by Apply, there is no actual change.				(#2622)
6. Custom Color View's Setting function appears Enable, click No response 						(#2626)
7. Simple simulation no function											(#2626)
9. Unable to delete the rightmost of silence regions by mouse to select 						(#2630, #2633)
10. Curve pin status(Enable, Edit, View, Invert) not be initialized that open exist UltraIO file and then create new silence file.
11. For [Menu]->[File]->[Export Event and Silence Region], will add sample rate and sample count information to export event and silence region txt file.
12. for [Menu]->[File]->[Import Event and Silence Region], will refer the sample rate and sample count information to scale event and silence region.
13. Fail to import poly-line and spin-line curves with scale from WIO file.

------------
UltraIO V6.07.000
------------
Based on UltraIO_V6.06.001

[Feature]
1. Add navigate waveform view to show current waveform position
2. Add color picker view to select color 					(#0002124)
3. Segment event show index not sample position on event view 			(#0002284)
4. Import marker from one WAV file to another WAV file in batch 		(#0001775)
5. Add a icon to show LED active high or active low 				(#0001806)
5. Can add color curve to multiple color group on single curve editor		(#0002125)
6. Fix - Mark Silence Region no function while zoom out full			(#0000513)
7. Fix - Can't add color curve into 2 color group in multiple editor view	(#0001900)
9. Fix - select all range then apply energy curve but crash in Win7	 	(#0001760)
10. Fix - Can't copy curve from another WIO file to a silence WIO file		(#0002071)
11. Fix - Repeat insert user events but over wave total time			(#0002187)

------------
UltraIO V6.06.001
------------
Based on UltraIO_V6.06.000

[Feature]
1. Fixed UIOEventListEditor time be overflow wave total time 

------------
UltraIO_V6.06.000
------------
Based on UltraIO_V6.05.000

[Feature]
1. Copy all curves / Paste all curves on curve list view
2. Invert All Curves on curve list view
3. Direct copy a region curve that won't generate image curve
4. Direct delete a region curve that won't generate level low curve
5. Can select and switch the past wst file on file list view (Max number is 10)
6. Auto save to current wst file when close the program
7. Can change the simulation color (Menu->Options->Curve Color Setting) for single curve pin(not RGB group curve pin) and show on the color bar on curve edit window and curve view window, and on simulation window
9. Color Event Setting extend to Pattern Event Setting(Menu->Options->Pattern Event Setting)
10. Auto select a region by double click the event view, waveform view, curve edit, curve view(Menu->Edit->Snap by Double Click)
11. Theme style change(Options->Theme style)
12. Multiple Curve View can set every Row Height
13. Update Help Information CHM file

------------
UltraIO V6.05.000
------------
Based on UltraIO_V6.04.000

[Feature]
1. Enable and disable option of RGB Group at the same time 
2. Installer will not administrator permission 
3. Add CueFormatRegex.ini to support SONIX marker
4. Batch Script Add Cue Point(User event、Silence event)
5. Fix the bug for resource run out when the file list changes file many times

------------
UltraIO V6.04.000
------------
Based on UltraIO_V6.03.000

[Feature Add]
1. Modify the item size for 4K screen
2. Add Multiple Curve Editors
3. Lock Min Application Size 640 x 480

------------
UltraIO V6.03.001
------------
Based on UltraIO_V6.03.000

[Feature Add]
1. Batch Merge Support Multiple file selecting

------------
UltraIO V6.03.000
------------
Based on UltraIO_V6.02.000

[Feature Add]
1. Add Property View to edit the control point color and morphing.
2. Add file list to record the used UltraIO file.
3. Add the file list to advance simulation view. 

------------
All installers are zipped with password: nuvoton
