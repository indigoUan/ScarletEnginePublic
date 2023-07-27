# Scarlet Engine (public repo)

The public repository of Scarlet Engine.
###### If you're looking for DLC files, go to [this page](https://google.com)

# Compilation - Required libraries

## [hxvm-lua](https://github.com/kevinresol/hxvm-lua) (C++ and JavaScript targets)
This library is for the Lua implementation of the engine.  
You can install hxvm-lua by running `haxelib git hxvm-lua https://github.com/kevinresol/hxvm-lua.git` in your cmd.  

## [linc_discord_rpc](https://github.com/Aidan63/linc_discord-rpc) (C++ targets only)
This library adds the Discord Rich Presence API to the engine.  
You can install linc_discord_rpc by running `haxelib git linc_discord_rpc https://github.com/Aidan63/linc_discord-rpc.git` in your cmd.  

## [hxCodec](https://github.com/polybiusproxy/hxCodec) (C++ targets only)
This library is for rendering videos.  
You can install hxCodec by running `haxelib install hxCodec` in your cmd.  
On Linux targets you need to install some other libraries **as well**:  
`sudo apt-get install libvlc-dev`  
`sudo apt-get install libvlccore-dev`  
`sudo apt-get install vlc-bin`  
