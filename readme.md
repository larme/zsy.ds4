# [zsy.ds4]

`[zsy.ds4]` is is a simple max patch to handle Dualshock 4 inputs (over bluetooth). It works with the major analog and digital inputs come from DS4 but without some advance features (trackpad and Sixaxis).

## Installation and Usage

Pair your DS4 with computer using bluetooth.

Copy this folder to your Max's `packages` folder. Then you can just right click on your patch windows (in editing status) and select "Paste From" -> "zsy.ds4.clip" to paste a bpatcher to your patch.

The bpatcher will have three outlets. The first outlet outputs following analog data from your DS4:

- Lx/Ly: Left analog stick's x/y position
- Rx/Ry: Right analog stick's x/y position
- L2p: Left analog trigger's pressure
- R2p: Right analog trigger's pressure


All analog data's range is 0-255.

The second outlet of `[zsy.ds4]` outputs digital data from DS4:

- L1/R1/L2/R2/L3/R3: triggers
- square/cross/circle/tirange: face buttons
- share/options: share and options button
- ps: the playstation button
- trackpad: trackpad click


The third outlet of `[zsy.ds4]` outputs DS4's dpad status:

- north: up is pressed
- northeast: up and right is pressed
- east: right is pressed
- southeast: down and right is pressed
- south: down is pressed
- southwest: down and left is pressed
- west: left is pressed
- northwest: up and left is pressed
- release: the dpad is released
