I have modified a Doom version from SDL Doom, optimized for JLiME machines. It works faster than the resource-hungry PrBoom, but still runs in 640 x 240 pixel mode. The game area is 320 x 240 with duplicated x pixels. The game works as it should, but there are some little things to do: the game's title screen and the intermission screens are still 200 pixels in height, so they must be scaled to 240 pixels.

If you want sound (only in Jornada 6xx), you must load the modules snd_sh_dac_audio and snd-pcm-oss with the commands

modprobe snd_sh_dac_audio

modprobe snd-pcm-oss

You should also have libsdl and libsdl-net libraries installed before playing.

Starting the game
- download the binary file and extract it onto the memory card
- go to the folder jlime-doom in Terminal
- write ./doom -file [path to your WAD file]
