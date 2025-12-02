------------
UltraIO V6.11.000 SP3
------------
Based on UltraIO V6.11.000 SP2

[Features]
+ Enhance addressable LED (addr.LED) with these new features for matrix mode
  - Extended the maximum supported addr.LED count from 255 to 65,025
  - Enabled zoom in/out operations on the addr.LED setting and editing page
  - Supported importing addr.LED image files and splitting them into multiple time points when either the row or column is 1
+ Limit advanced simulation to simulate addressable LED matrix with size not over 256.
+ Enhance flash, sine, and triangle curve frequency precision from two to four decimal places.

------------
UltraIO V6.11.000 SP2
------------
Based on UltraIO V6.11.000 SP1

[Features]
+ Support the function to increase or decrease playback speed

------------
UltraIO V6.11.000 SP1
------------
Based on UltraIO V6.11.000

[Features]
+ Support editing the position, transition, and color of multiple control points on color flyer and color envelope, except for the positions of the first and last control points


------------
UltraIO V6.11.000
------------
Based on UltraIO V6.10.000 SP10

[Features]
+ Change spline curve, triangle, envelope curve editing window layout
+ Support motor mode on curve pin
+ Support frequency transition function for flashing, sine, and triangle curve
+ Change the ruler unit to a more appropriate measurement.
+ Upgrade the building tool from visual studio 2010 to visual studio 2022

------------
UltraIO V6.10.000 SP10
------------
Based on UltraIO V6.10.000 SP9

[Features]
+ scale bitmap width and height to fit the row and column number on SLED "import Bitmap file" function
+ advance simulation redo and undo function
+ rename the UI word from "morphing/fading" to "transition" and update help document

[Bug Fixed]
+ fixed press mouse wheel then scroll up/down but scroll waveform to right/left. Should scroll waveform to left/right
+ fixed press mouse wheel then move mouse to left/right but scroll waveform to left/right. Should scroll waveform to right/left
+ fixed advance simulation play can't display curve color
+ fixed some window mouse scroll feature not working
+ fixed can't import problem that the first item interval is 0 and the format is BMP on SLED "import Bitmap file" function
+ fixed Waveform view window display error at select region in waveform editor [Mantis:4195]

------------
UltraIO V6.10.000 SP9
------------
Based on UltraIO V6.10.000 SP8

[Features]
+ support to press and drag the middle mouse button will move waveform left or right
+ support to scroll middle mouse button up or down will move waveform left or right
+ support to hold on "Ctrl" key and scroll middle mouse button up or down will zoom in or zoom out waveform.
+ support to import UltraIO setting file (xxx.reg) from help menu
+ add "UltraIO Tool User Guide.pdf" into Document folder on application folder 

[Bug Fixed]
+ Resolve the issue where modifying the starting position of the energy curves causes an unintended change in the overall shape of the curves, which should remain consistent regardless of the starting position adjustment.

------------
UltraIO V6.10.000 SP8
------------
Based on UltraIO V6.10.000 SP7

[Features]
+ Enhance LED flash frequency checking with customized sampling rate not according to waveform sample rate
+ Can see flash detect error reason and its position
+ Can adjust ALED output by gamma correction setting

[Bug Fixed]
+ simple simulation result is incorrect at zoom in waveform then choose new playback position

------------
UltraIO V6.10.000 SP7
------------
Based on UltraIO V6.10.000 SP6

[Feature]
+ implement to soften transition at color flyer control pointer on color flyer setting window or event view
+ implement to export current UltraIO registry setting for debug customer window environment on menu [Help | Export UltraIO setting]
+ ensure the simulation view is visible and start play when click menu [Run | Simulation | Simple Simulation]
+ check and modify the serial LED color pixel information must be smaller than max sample position when load WIO file
+ check and modify the serial LED color pixel information must be smaller than max sample position when generate the play ALED data

[Bug Fixed]
+ import SLED data from WIO file without checking scale option does not cut those ALED data after last PCM sample.
+ waveform, curve edit, curve view panel height is incorrect when setting different screen font size.

------------
UltraIO V6.10.000 SP6
------------
Based on UltraIO V6.10.000 SP5

[Feature]
+ speed up to parse Vixen CSV data to SLED data
+ modify curve list view layout
  - change the active low icon picture
  - add blank between tree node text and icon

------------
UltraIO V6.10.000 SP5
------------
Based on UltraIO V6.10.000 SP4

[Feature]
+ modify the new layout to import SLED data from Vixen data window
  - add [Replace serial LED data] or [Append serial LED data] selection on serial LED mode
  - add [Scale data to fit waveform] selection on serial LED mode
  - remove color mode selection
  - remove sample selection on timing group
  - show wire scan order setting if selected serial LED group is matrix mode
+ add advance simulation to support SLED edit and play
+ modify UIO batch merge convert window
  - add grid line to control lists
  - add auto LED flash frequency restriction to [WAV->WIO] and [WIO->WAV]
  - fix the problem that the triangle curve disappear after importing with option SCALE
+ update reset layout registry file to clear more layout data

------------
UltraIO V6.10.000 SP4
------------
Based on UltraIO V6.10.000 SP3

[Bug Fixed]
+ fix the wrong action that import Vixen format data to serial LED group with array type’s matrix mode

------------
UltraIO V6.10.000 SP3
------------
Based on UltraIO V6.10.000 SP2

[Bug Fixed]
+ fix to display the wrong waveform view data if all wave data is silence

------------
UltraIO V6.10.000 SP2
------------
Based on UltraIO V6.10.000 SP1

[Feature]
+ Support automatically detect sample per group for mono and color envelop to pass LED flash detection.


------------
UltraIO V6.10.000 SP1
------------
Based on UltraIO V6.10.000

[Feature]
+ support to move splitter to change the waveform view, curve edit, and curve view
+ show full path tool tip text when mouse move enter combobox control on batch mode window
+ check and show error message if the wave file is not 16-bit PCM format
+ Add sample per group option in the color envelope curve.
+ Relayout color envelope dialog to have more margin between controls. 
+ "Apply to All" button move to the place closed to Morphing which is the checkbox "Apply to All" apply to.
+ Add "Shift Curve Start Index" menu item function on menu Options

[Bug Fixed]
+ Apply the morphing option to the control points of color envelope curve.
+ fix to add multiple files but add files count is not match with selected files on batch mode window
+ fix to open unsupported PCM format file but add file path to the file list

------------
UltraIO V6.10.000
------------
Based on UltraIO V6.09.000 SP4

[Feature]
+ new serial LED functions
   - copy serial LED time points and paste to another UltraIO file then scale time points position to fit target file
   - copy serial LED group and paste to another UltraIO file then scale time points position to fit target file
   - support to add multiple time points on serial LED group by right-mouse clicking on Serial LED event view
   - support to pick color by right-mouse clicking on color pixel panel
   - limit Serial LED max LED count to 256
+ import serial LED data in batch mode
+ import Vixen format CSV file using menu [File | Import Vixen format data from CSV file]
+ support LED flash check function using menu [Run | Run LED Flash Check] with set frequency range and set ignore to change message color
+ insert silence function that select a region on waveform view and using menu [File | Insert Silence]
+ delete selected waveform function that select a region on waveform view  and using menu [File | Delete Selected Waveform]
+ add de-bounce time between left-mouse down and mouse move to avoid moving time point easily
+ set default silence sample rate is 8000 after open new silence window
+ update UltraIO user guide document

[Bug Fixed]
+ fix crash problem that generate the RGB group action
+ fix crash problem that generate color flyer curve but doesn't select all curve pins on color group
+ fix select multiple files then add into file list but some files will be lost

------------
UltraIO V6.09.000 SP4
------------
Based on UltraIO V6.09.000 SP3

[Feature]
+ record the last enable option for "Enable color Range By Wave Length"
+ enable serial LED fading setting
+ modify the time and sample rate limitation for creating silence wave file
  - time length must be bigger than 1 (ms)
  - sample rate must be bigger than 30 (sample/second)
+ check total used memory size to show waveform and curve information for creating silence wave file

------------
UltraIO V6.09.000 SP3
------------
Based on UltraIO V6.09.000 SP2

[Feature]
+ implement the global shift sample function of all UltraIO curves at [WAVE->WIO] mode on UltraIO batch merge generator
+ implement "Move All Curves..." function to move all curves on selected curve pins ([Menu]->[Curve]->[Move All Curves...])

------------
UltraIO V6.09.000 SP2
------------
Based on UltraIO V6.09.000 SP1

[Feature]
+ There is only one serial LED group will be enable
+ On curve list view if the user enable/disable curve and this curve is not selected, the other selected curves will not be enable/disable
+ If exist the checked group item on serial LED, the serial LED group will be set checked

------------
UltraIO V6.09.000 SP1
------------
Based on UltraIO V6.09.000

[Bug Fixed]
+ Show "End Position must be larger than Start Position" error message at pressing energy curve apply button twice when display unit is time.

------------
UltraIO V6.09.000
------------
Based on UltraIO V6.08.000

[Feature]
+ Support address LED setting

[Bug Fixed]
+ In the absence of the wave file, setting the Envelope Control Curve Dialog to press ok does not work.		(#2649)
+ Revised Nuvoton link for About UltraIO										(#2651)
+ UI shows only part of whole view after several steps									(#2448)
+ Fix the Polyline and Spline import fail problem using scale function if the first point's sample is 0
+ Fix the repeat segment event insert more than max range problem if select all region and use ms unit interval

------------
UltraIO V6.08.000
------------
Based on UltraIO V6.07.000

[Feature]
+ Update help document about color picker view

[Bug Fixed]
+ If the UltraIO default not enable any curve pin, it will not enable the first curve pin or group automatically	(#2452)
+ Should active color pickup view "apply" button and customer color view at color curve control point selected		(#2304)
+ Should remove the index in color pickup view										(#2305)
+ Operation causes Color Picker View not to appear completely								(#2621)
+ Change the value of Red/Green/Blue in Color Picker by Apply, there is no actual change.				(#2622)
+ Custom Color View's Setting function appears Enable, click No response 						(#2626)
+ Simple simulation no function											(#2626)
+ Unable to delete the rightmost of silence regions by mouse to select 						(#2630, #2633)
+ Curve pin status(Enable, Edit, View, Invert) not be initialized that open exist UltraIO file and then create new silence file.
+ For [Menu]->[File]->[Export Event and Silence Region], will add sample rate and sample count information to export event and silence region txt file.
+ for [Menu]->[File]->[Import Event and Silence Region], will refer the sample rate and sample count information to scale event and silence region.
+ Fail to import poly-line and spin-line curves with scale from WIO file.

------------
UltraIO V6.07.000
------------
Based on UltraIO V6.06.001

[Feature]
+ Add navigate waveform view to show current waveform position
+ Add color picker view to select color 					(#0002124)
+ Segment event show index not sample position on event view 			(#0002284)
+ Import marker from one WAV file to another WAV file in batch 		(#0001775)
+ Add a icon to show LED active high or active low 				(#0001806)
+ Can add color curve to multiple color group on single curve editor		(#0002125)
+ Fix - Mark Silence Region no function while zoom out full			(#0000513)
+ Fix - Can't add color curve into 2 color group in multiple editor view	(#0001900)
+ Fix - select all range then apply energy curve but crash in Win7	 	(#0001760)
+ Fix - Can't copy curve from another WIO file to a silence WIO file		(#0002071)
+ Fix - Repeat insert user events but over wave total time			(#0002187)

------------
UltraIO V6.06.001
------------
Based on UltraIO V6.06.000

[Feature]
+ Fixed UIOEventListEditor time be overflow wave total time 

------------
UltraIO V6.06.000
------------
Based on UltraIO V6.05.000

+ ature]
+ Copy all curves / Paste all curves on curve list view
+ Invert All Curves on curve list view
+ Direct copy a region curve that won't generate image curve
+ Direct delete a region curve that won't generate level low curve
+ Can select and switch the past wst file on file list view (Max number is 10)
+ Auto save to current wst file when close the program
+ Can change the simulation color (Menu->Options->Curve Color Setting) for single curve pin(not RGB group curve pin) and show on the color bar on curve edit window and curve view window, and on simulation window
+ Color Event Setting extend to Pattern Event Setting(Menu->Options->Pattern Event Setting)
+ Auto select a region by double click the event view, waveform view, curve edit, curve view(Menu->Edit->Snap by Double Click)
+ Theme style change(Options->Theme style)
+ Multiple Curve View can set every Row Height
+ Update Help Information CHM file

------------
UltraIO V6.05.000
------------
Based on UltraIO V6.04.000

[Feature]
+ Enable and disable option of RGB Group at the same time 
+ Installer will not administrator permission 
+ Add CueFormatRegex.ini to support SONIX marker
+ Batch Script Add Cue Point(User event、Silence event)
+ Fix the bug for resource run out when the file list changes file many times

------------
UltraIO V6.04.000
------------
Based on UltraIO V6.03.000

[Feature Add]
+ Modify the item size for 4K screen
+ Add Multiple Curve Editors
+ Lock Min Application Size 640 x 480

------------
UltraIO V6.03.001
------------
Based on UltraIO V6.03.000

[Feature Add]
+ Batch Merge Support Multiple file selecting

------------
UltraIO V6.03.000
------------
Based on UltraIO V6.02.000

[Feature Add]
+ Add Property View to edit the control point color and morphing.
+ Add file list to record the used UltraIO file.
+ Add the file list to advance simulation view. 

------------
All installers are zipped with password: nuvoton
