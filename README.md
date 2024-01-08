# TomeNET-Tileset

This is a graphical tileset for the TomeNET game (https://tomenet.eu/)

## How to setup

### Linux 

1) put `16x22sv.bmp` in your `tomenet/lib/xtra/graphics` folder
2) put `graphics-16x22sv.prf` in your `tomenet/lib/user` folder
3) configure `~/.tomenetrc`: add graphics setup lines
```
graphics		1
graphic_tiles		16x22sv
```

### Windows


## Problems

There are two known problems with using graphics right now:

- [monster list shows wrong tiles](https://github.com/TomenetGame/tomenet/issues/50)  
- [interface crash and packet errors if there is no graphic tiles for "Floor" features](https://github.com/TomenetGame/tomenet/issues/51)
- Windows: in character overview window items that have tiles are not displayed correctly
- Windows: game launch take much more time (few minutes)
