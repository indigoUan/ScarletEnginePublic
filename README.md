# Scarlet Engine (public repo)

The public repository of Scarlet Engine.
###### If you're looking for DLC files, go to [this page](https://google.com)

# Compilation - Required libraries

## [plainenglish](https://github.com/indigouan/plainenglish) (all targets)
This library is for the Plainenglish script implementation of the engine.  
You can install plainenglish by running
```bash
haxelib git plainenglish https://github.com/indigouan/plainenglish.git
```
in your cmd.  

## [linc_discord_rpc](https://github.com/Aidan63/linc_discord-rpc) (C++ targets only)
This library adds the Discord Rich Presence API to the engine.  
You can install linc_discord_rpc by running
```bash
haxelib git linc_discord_rpc https://github.com/Aidan63/linc_discord-rpc.git
```
in your cmd.  

## [hxCodec 2.6.1](https://github.com/polybiusproxy/hxCodec) (C++ targets only)
This library is for rendering videos.  
As of Scarlet Engine version 0.0.0.1, the version of hxCodec MUST be 2.6.1. Check the [log](https://github.com/indigoUan/ScarletEngineData/blob/main/compilation-requirements-log.md) for past versions.
You can install hxCodec by running
```bash
haxelib install hxCodec 2.6.1
```
in your cmd.  
On Linux targets you need to install some other libraries **as well**:  
```bash
sudo apt-get install libvlc-dev
sudo apt-get install libvlccore-dev
sudo apt-get install vlc-bin
```

# Compilation - Compiling the source code

After downloading as .zip or cloning this repository, you might want to compile the project.  
As of version 0.0.0.1 of the engine, only Windows and Linux are compatible. Check the [log](https://github.com/indigoUan/ScarletEngineData/blob/main/compilation-requirements-log.md) for past versions.  

## Step one - installing Haxe, HaxeFlixel, and OpenFl:
### Haxe:  
Head to [Haxe's official downlod website](https://haxe.org/download) and select the installer version compatible with your computer. If you're unsure if you're using 32 bit or 64 bit, look it up.  
After downloading the installer, launch it and follow the instructions.  
To check if you succeeded, launch your CMD and try the command `haxe`.  
### HaxeFlixel and OpenFl:
Please follow [the official HaxeFlixel guide to installation](https://haxeflixel.com/documentation/install-haxeflixel/).

## Step two - Libraries:
Make sure that all the [libraries](https://github.com/indigoUan/ScarletEnginePublic/blob/main/README.md#compilation---required-libraries) are installed.

## Step three - Compiling:
Once you have a clone or copy of the source code, make sure that the file `project.xml` is in the root of the project.  
Open your CMD to the directory where the `project.xml` file is stored and run the command `lime test windows` if you're on Windows, or `lime test linux` if you're on any Linux sytem.  

## Step four - Compilation errors:
Ahah good luck.
