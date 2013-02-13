
EXIF Metadata Utility for Exotic Lenses
=======================================

Author: Nik Gaffney <nik@fo.am>

Based on the Droplet for "MS Super Triplet Perar 35mm f/3.5" by Dirk Rösler (at http://japanexposures.com )


Requirements
------------

ExifTool by Phil Harvey http://www.sno.phy.queensu.ca/~phil/exiftool/


Install
-------

Download from here

https://github.com/zzkt/Jupiter-8-50mm-f-2-exif-droplet/raw/master/Jupiter-8%2050mm%20f:2.zip

Description
-----------

Stand-alone Automator application that sets the lens name, focal length and maximum aperture of your image to Jupiter-8 50mm f/2 in the file's EXIF data.


How to use 
----------

Drag and drop DNG or other file onto the application. EXIF data will be updated with the new information and the original file overwritten.

You need to to reload the image metadata for your application to recognize or apply this script before importing (e.g. into Lightroom).

Warning: in case you have already performed development e.g. in Lightroom and want to apply the script, be sure that your development data is saved to the file before reloading the metadata from the file. This can be done manually (Cmd-S Save Metadata To File) or set to automatic in preferences. Otherwise this may cause development data to be lost.


Commandline
-----------

    exiftool -P -overwrite_original -FocalLength=50 -MaxApertureValue=2 -Lens="Jupiter-8 50mm f/2"


