------------------------
Nintenlord's compressor.
------------------------

Note: Requires .NET framework 2.0 or Mono 2.0 or higher.

________________
Version history:
~~~~~~~~~~~~~~~~

Version 1.0
-Original release.

Version 1.1
-Fixed minor problems with compression and 
decompression methods.
-Added file extension filters for output and input.
-Made it possible to use 0x and $ prefixes without
messing actual value.
-Made input and output browse functions use
previous filepaths as defaults.
-Added titles to file selection windows.
-Added Icon to the windows form when program is 
running.

Version 1.2
-Rewrote compression method, runs faster and
has no bugs.

Version 1.3
-Fixed a bug from previous version.

Version 1.4
-Fixed another bug.
-Added the possibility of dragging a file to
the program. Dragged file will automatically be 
placed to Input.

Version 2.0
-Fixed a minor bug on compressing
-Added Lenght, which finds out the size of the 
compressed data.
-Added Uncompressable, which finds out weather
offset can be compressed.
-Updated scan to check automatically check if
offset is compressable. Slow, but effective.

Version 2.1
-Added the exception handling that was missing
in the previous version. 

Version 2.2
-Made lenght more accurate.

Version 3.0
-Performance improvements. Scanning and compressing 
are now faster than before.

Version 3.1
-Fixed typos.
-Removed the checkbox for directing output to message box.
-Replaced offset text boxes with numeric up/downs.

Version 3.2
-Fixed error with compression.

Version 3.3
-Few bug fixes.

Version 3.4
-Made compression to compress to sligthly smaller size.

Version 4.0
-Added extentable compression support.

___________
How to use:
~~~~~~~~~~~

First, you need to select a compression.
If you don't, you can't do anything with
the compressor. Choose one of the dll files
thaat come with the program.

Controls, UI, etc:
Just read what it says in the UI.

Default values:
If no offset or size is specified, the values are
offset = 0 and size = the whole file.

Actions:
-Scan: 
Scans the input file for potential compressed 
data. Will find every instance in 
the file. Offsets are outputted in text to the 
specified outputfile. You can also specifie the
area where to search with input info with input
offset and size.

-Decompress:
Decompresses the data from specified offset for
specified size and writes it to outputfile. If 
outputfile doesn't exist, it will be created. 
Output offset can also be specified.

-Compress:
Compresses data from specified area of input file.
Writes it to specified output file offset. Doesn't
use size for anything.

-Lenght:
Counts the lenght of the compressed data. Input
offset is the location of the compressed data.

-Decompressable:
Checks if data can be decompressed. Input
offset is the position of the data.

________________________________
How to use compression template:
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Copy the file MyCompressionTemplate.zip to
folder ...\Visual Studio 2008\Templates\ProjectTemplates\Visual C#\
and use the template when creating a new project. 
Fix the referance to Nintenlord's compression
and you are ready. NOTE: Do not unzip the template.

Template created with Visual Studio 2008 Professional.
______
Legal:
~~~~~~

Use it and modify it as you wish, I'm not 
responsible for consequenses. All money made with
this program belongs to Nintenlord, though.

________
Credits:
~~~~~~~~

-Nintenlord, making the utility.
-Parasyte, for making GBADecomp which inspired me
to do this program.
-Fellow hackers of Fire Emblem Universe/Tactics Universe,
from being awesome.
-Everyone who uses this, for using it.
