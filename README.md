# Tagger

# Tagger 0.6.1.3

Tagger is alpha release software. Your performance may vary.

System requirements:

# Hardware

1] A fast Apple Mac Computer: recommended Mac Pro with 6GB+ VRAM.
2] A large screen capable of displaying 1920x1200px or more

# Software

1] MacOS 10.7 to 10.11.6. Currently untested on MacOS 10.12

2] Quartz Composer 4.6.2 or greater (available here (requires devloper account): https://developer.apple.com/download/more/ - look for Additional_Tools_for_Xcode_8.dmg

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


Note - to work on versions of MacOS later than 10.8 some of the plugins/patches hosted on github may require compiling from source using Xcode 7 or later. Alternatively versions are supplied with this repository that ~may~ work on your MacOS version (tested up to MacOS 10.12)

Some plugins ~may~ have become unavailable online (eg. _1024_StructureTools.plugin)_. 

If so, please use the supplied versions from the attached zip file in this repository. This bundles all the necessary plugins that are not currently available online. Kineme ChartTools, Data Tools, GLTools, FileTools may be 30 day demo versions that will require a end-user license to be purchased after the end of the trial period. Licenses may be purchased from Kineme (http://kineme.net/downloads) or the plugins can be compiled from souce if available on github (see above URLs).

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

Once Quartz Composer has been installed, as well as all custom patches/plugins, please run the file QCGUI_test.qtz to confirm that Tagger interface buttons are performing correctly and not causing non-specific OpenGL crashes. From testing, running this small program will overcome a temporary OpenGL problem that may cause Tagger to crash. This program may be left open in the background whilst Tagger is running.

Open Tagger_v0.6.1.3.qtz in Quartz Composer and follow this video for user instructions and demonstration:

https://vimeo.com/113643647


