# Tagger

Tagger 0.6.1.2

Tagger is alpha release software. Your performance may vary.

System requirements:

Hardware

1] A fast Apple Mac Computer: recommended Mac Pro with 6GB+ VRAM.
2] A large screen capable of displaying 1920x1200px or more

Software

1] MacOS 10.7 to 10.11.6. Currently untested on MacOS 10.12

2] Quart Composer 4.6.2 or greater (available here (requires devloper account): https://developer.apple.com/download/more/ - look for Additional_Tools_for_Xcode_8.dmg

3] Quartz Composer plugins/patches:

ChartTools.plugin http://kineme.net/product/ChartTools

GLTools.plugin https://github.com/kineme/GLTools

Climb CSV Importer.plugin http://www.climbapp.com/plugin/csvimporter/index.html

FileTools.plugin https://github.com/kineme/FileTools

FXFactory Patches.plugin https://fxfactory.com/download/ (installed as part of FxFactory)

Origami.plugin http://facebook.github.io/origami/

1024_StructureTools.plugin https://1024d.wordpress.com/qc-plugins/

DataTools.plugin https://github.com/kineme/DataTools

FreeboardPatch.plugin http://kineme.net/release/FreeboardPatch/01

Note - to work on versions of MacOS later than 10.8 some of these plugins/patches may require compiling from source using Xcode 7 or later.

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

