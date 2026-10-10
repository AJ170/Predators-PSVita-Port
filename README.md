# Predators-PSVita-Port
Credit to Mobstudios for making the game.
Credit to ShadowOsmium for decompiling the game.

<img width="2404" height="1434" alt="predscreen" src="https://github.com/user-attachments/assets/7ba434b3-5974-4ab4-b9ee-728a1d3d8d30" />

## Controls
```
cross - Attack/Select for mouse
square - Grab
circle - I forgot
triangle - I forgot
start - Pause
Left Stick - Move Character
Right Stick - Move Mouse
L - Change Melee
R - Change Ranged
```

## Installation

No VPK is provided directly. Release contains an xdelta patch that must be
applied to your own copy of the original games .obb file.
You need version 1.5.1 of Predators .obb file for android (MUST BE ORIGINAL GAME FILES)

1. Install `PREDATORS-FinalBuild_v1.0-stub.vpk` on your Vita with VitaShell or VitaDB
2. Download [xdelta3](https://github.com/jmacd/xdelta) ([Windows builds here](https://github.com/jmacd/xdelta-gpl/releases)) and put `xdelta3.exe`, the .obb file and `PredatorsData.xdelta` in the same folder
```
Newly Created Folder
└── /main.21.com.fde.predators.obb
└── /PredatorsData.xdelta
└── /xdelta3.exe
```
3. Open a command prompt in that folder and run:     

`./xdelta3 -d -B 536870912 -s main.21.com.fde.predators.obb PredatorsData.xdelta PredatorsData.zip`

4. Extract `PredatorsData.zip` and copy the "Media" folder into `ux0:app/PRED42069/`
and merge with the existing files
5. Launch PREDATORS
