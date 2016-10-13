# Tagger

# Tagger 0.6.1.3

Tagger is an interactive software tool and workflow to visualise, characterise, sample and tag 1d time-variant geoscientific datasets from both local and cloud-based repositories. It uses an animated interface and human-computer interaction to utilise the capacity of human expert observers to identify features via enhanced visual analytics. 

Tagger is alpha release research software. Your performance may vary.

System requirements:

# Hardware

1] A fast Apple Mac Computer: recommended Mac Pro with 6GB+ VRAM.

2] A large screen capable of displaying 1920x1200px or more

# Software

1] MacOS 10.7 to 10.11.6. Currently untested on MacOS 10.12

2] Quartz Composer 4.6.2 or greater (available here (requires developer account): https://developer.apple.com/download/more/ - look for Additional_Tools_for_Xcode_8.dmg

3] Quartz Composer plugins/patches:

  ChartTools.plugin http://kineme.net/product/ChartTools

  GLTools.plugin https://github.com/kineme/GLTools

  Climb CSV Importer.plugin http://www.climbapp.com/plugin/csvimporter/index.html

  FileTools.plugin https://github.com/kineme/FileTools

  FXFactory Patches.plugin https://fxfactory.com/download/ (installed as part of FxFactory)

  Origami.plugin http://facebook.github.io/origami/

  1024_StructureTools.plugin https://1024d.wordpress.com/qc-plugins/ __seems to be unavailable online__

  DataTools.plugin https://github.com/kineme/DataTools

  FreeboardPatch.plugin http://kineme.net/release/FreeboardPatch/01

  QCGUI.plugin https://github.com/nenghuo/QCGUI

  jQC 1.0 http://qcdesigners.com/index.php/forums/topic/100/it-s-finally-here-j-qc-1-0-a-u/


Note - to work on versions of MacOS later than 10.8 some of the plugins/patches hosted on github may require compiling from source using Xcode 7 or later. Alternatively versions are supplied with this repository that ~may~ work on your MacOS version (tested up to MacOS 10.11.6)

Some plugins ~may~ have become unavailable online (eg. _1024_StructureTools.plugin)_. 

If so, please use the supplied versions from the attached zip file in this repository. This bundles all the necessary plugins that may not be currently available (precompiled) online. Kineme ChartTools, Data Tools, GLTools, FileTools may be 30 day demo versions that will require an end-user license to be purchased after the end of the trial period. Licenses may be purchased from Kineme (http://kineme.net/downloads) or the plugins can be compiled from souce if available on github (see above URLs).

Quartz Composer can install plugins/patches in two key locations:

##1.

"/Users/****/Library/Graphics/Quartz Composer Patches" (if you don’t have this folder,create one)

"/Users/****/Library/Graphics/Quartz Composer Plugins" (if you don’t have this folder,create one)

##2.

"Macintosh HD/Library/Graphics/Quartz Composer Patches" (if you don’t have this folder,create one)

"Macintosh HD/Library/Graphics/Quartz Composer Plugins" (if you don’t have this folder,create one)

Confusingly, some '.plugin' files need to be placed in the 'patches' directory, NOT the plugins directory.

See here for more information: http://kineme.net/HowtoInstallCustomPatches

The EASIEST way to correctly install all patches and plugins is to use the QC Plugin Manager: http://imimot.com/qc-plugin-manager/

_________________________________

# Instructions:

Once Quartz Composer has been installed, as well as all custom patches/plugins, please run the file QCGUI_test.qtz to confirm that Tagger interface buttons are performing correctly and not causing non-specific OpenGL crashes. From testing, running this small program will overcome a temporary OpenGL problem that may cause Tagger to crash under MacOS 10.11/10.12, earlier versions (10.7-10.10) are not affected. This program may be left open in the background whilst Tagger is running.

Open Tagger_v0.6.1.3.qtz in Quartz Composer and follow this video for user instructions and demonstration:

https://vimeo.com/113643647

This repository includes an example WaveRider buoy data file: cpso2001_h1.csv 

For demonstration purposes, this is a non-THREDDS-capable version of Tagger that works with local .csv/.txt data files.

_________________________________

# Data

Tagger can be used with any .csv file that meets the following criteria:

1] The first 6 fields (0-5) contain timestamp data in the format:

DD, MM, YYYY, HH, MN, SS, (Day, Month, Year, Hour, Minute, Second). 

2] It is currently hard-coded for the WaveRider Buoy data - meaning that its GUI nomenclature for other variables after the timestamp will not change, i.e. it is hard-coded to

DD, MM, YYYY, HH, MN, SS, Hs, Hrms, Hmax, Tz, Ts, Tc, THMax, EPS, T02, Tp, Hrms.1, EPS.1 - e.g.

7,1,1998,14,20,8,2.1,1.45,3.87,7.26,9.8,4.05,9.84,0.83,7.33,11.31,1.55,0.87

Other field values after the 6 timestamp fields (up to 12) can be read and graphed,but will not be assigned field names other than pre-existing ones.

Field-name Header interpretation may be implemented in a later version of the software.


