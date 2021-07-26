+++
title = "TAS"
description = "Tool Assisted Speedrun"
+++
This tool allows you to enter precise controller inputs to the game that is near impossible at a human level without missing a beat. 
You can set the different analog sticks and lock them to certain positions as well as check certain buttons to be pressed and released.

# How to use

To play back TAS scripts on Yuzu, select the folder with scripts in the configuration menu below
Tools -> Configure TAS. The file itself has normal text format and has to be called `script0-1.txt`
for controller 1, `script0-2.txt` for controller 2 and so forth (with max. 8 players).

After placing the file at the correct location, it can be read into Yuzu with the (default) hotkey
`CTRL+F6` (refresh). In the bottom left corner, it will display the amount of frames the script file
has. Playback can be started or stopped using `CTRL+F5`.

However, for playback to actually work, the correct input device has to be selected: In the Controls
menu, select TAS from the device list for the controller that the script should be played on.

Recording a new script file is really simple: Just make sure that the proper device (not TAS) is
connected on P1, and press `CTRL+F7` to start recording. When done, just press the same keystroke
again (`CTRL+F7`). The new script will be saved at the location previously selected, as the filename
record.txt.

{{< imgs
    "./control_debugger.png|For debugging purposes, the controller debugger can be used"
    "./control_debugger_pressed.png|View -> Debugging -> Controller P1"
>}}

## Example script

A script file has the same format as [TAS-nx](https://github.com/hamhub7/tas-script) uses.
<article class="message"><div class="message-header">Example</div><div class="message-body">
1 KEY_B 0;0 0;0<br>
6 KEY_ZL 0;0 0;0<br>
41 KEY_ZL;KEY_Y 0;0 0;0<br>
43 KEY_X;KEY_A 32767;0 0;0<br>
44 KEY_A 32767;0 0;0<br>
45 KEY_A 32767;0 0;0<br>
46 KEY_A 32767;0 0;0<br>
47 KEY_A 32767;0 0;0<br>
</div></article>

For more advanced scrips you can take a look at this Super Mario Odyssey [TAS script](./script0-1.txt) made by matthewpugs24.
{{< youtube Gh2aCXdnZRk >}}