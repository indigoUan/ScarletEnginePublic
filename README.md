# Scarlet Engine (public repo)

The public repository of Scarlet Engine.
###### If you're looking for DLC files, go to [this page](google.com) (placeholder).

# Compilation
###### A foolproof guide by îndigoUán, AKA the author of the project, AKA the coolest person to set foot on the planet.
Please, use the built-in modding system instead of publishing a new executable every mod.

# Compilation - Required libraries

## [plainenglish](https://github.com/indigouan/plainenglish) (all targets)
This library is for the Plainenglish script implementation of the engine.  
You can install plainenglish by running the following command.
```bash
haxelib git plainenglish https://github.com/indigouan/plainenglish.git
```

## [linc_discord_rpc](https://github.com/Aidan63/linc_discord-rpc) (C++ targets only)
This library adds the Discord Rich Presence API to the engine.  
You can install linc_discord_rpc by running the following command.
```bash
haxelib git linc_discord_rpc https://github.com/Aidan63/linc_discord-rpc.git
```

## [hxCodec 3.0.2](https://github.com/polybiusproxy/hxCodec) (C++ targets only)
This library is for rendering videos.  
As of Scarlet Engine version 0.0.0.1, the version of hxCodec MUST be 3.0.2, as it loves to change radically across versions. Check the [log](https://github.com/indigoUan/ScarletEngineData/blob/main/compilation-requirements-log.md) for past engine versions.  
You can install hxCodec by running the following command.
```bash
haxelib install hxCodec 2.6.1
```

On Linux targets you need to install some other libraries ***as well***:  
```bash
sudo apt-get install libvlc-dev
sudo apt-get install libvlccore-dev
sudo apt-get install vlc-bin
```

# Compilation - Compiling the source code

After downloading as .zip or cloning this repository, you might want to compile the project.  
As of version 0.0.0.1 of the engine, only Windows and Linux are compatible. Check the [log](https://github.com/indigoUan/ScarletEngineData/blob/main/compilation-requirements-log.md) for past engine versions.  

## Step one - installing Haxe, HaxeFlixel, and OpenFl:
### Haxe:  
Head to [Haxe's official download website](https://haxe.org/download) and select the installer version compatible with your computer. If you're unsure if you're using 32 bit or 64 bit, look it up.  
After downloading the installer, launch it and follow the instructions.  
To check if you succeeded, launch your CMD and try the command `haxe`.  
### HaxeFlixel and OpenFl:
Please follow [the official HaxeFlixel guide to installation](https://haxeflixel.com/documentation/install-haxeflixel/).

## Step two - Libraries:
Make sure that all the [libraries](https://github.com/indigoUan/ScarletEnginePublic/blob/main/README.md#compilation---required-libraries) are installed.

## Step three - Compiling:
Once you have a clone or copy of the source code, make sure that the file `project.xml` is in the root of the project.  
Open your CMD to the directory where the `project.xml` file is stored and run the command `lime test windows` if you're on Windows, or `lime test linux` if you're on any Linux system.  

## Step four - Compilation errors:
Time and patience are money and I am broke, you can ask in the (to be) [public Scarlet Engine Discord server](google.com) (placeholder) for help.  

# Compilation - Debugging crashes:
When the engine crashes at runtime (AKA when the game is running) it automatically stores the crashlog (uncaught exception) in the `crashlogs/` directory of the executable file (`export/release/windows|linux/bin/`).  
If you need help with an uncaught exception you can't figure out, I resuggest asking in the (to be) [public Scarlet Engine Discord server](google.com) (placeholder), and NOT asking me.  
