ATTENTION
================
I moved my repositories to gitlab, please do any suggestions there: https://gitlab.com/Hirmer/GCode-Paver

Thank you!


# GCode-Paver
uses the CNC_gcode-to-reprap-converter to generate a Pattern of Signs in a defined Space

What it does?
- generates .gcode files in a defined Folder from the included .svg files
- generates a paved.gcode file with a pattern defined by calling the script
- generates a logfile with the callbacks of pyCam and GNC_gcode-to-reprap-converter

What it needs?
- pyCam to generated G-Code from .svg Files (http://pycam.sourceforge.net/)
- CNC_gcode-to-reprap-converter (https://github.com/HardRainbow/CNC_gcode-to-reprap-converter)

How to use:
- open the ***gcode_paverV01.py*** file and edit the "Line 34". It should direct the location of the CNC_gcode-to-reprap-converter location
- call the script by typing ***python gcode_paverV01.py***

Description:
- ***< amount_horizontal >*** defines the amount of signs in a horizontal Line
- ***< sign_width >*** defines sign width
- ***< sign_height >*** defines sign height
- ***< feedrate_traveling >*** values given to the CNC_gcode-to-reprap-converter for traveling speed
- ***< feedrate_cutting >*** values given to the CNC_gcode-to-reprap-converter for cutting speed
- ***< feedrate_zaxis >*** values given to the CNC_gcode-to-reprap-converter for z-axis traveling speed
- ***< filename1 > [filename2 ... n]*** given .svg files to generate .gcode from, the location to an folder with * may convert all files within it. Example: "/home/user/test/*"

Known Bugs:
- Filename-Path may cause errors if Folder contains spaces (no time to fix this yet)
- no proper error-report

~ Hardy
