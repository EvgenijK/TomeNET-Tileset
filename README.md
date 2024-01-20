# TomeNET-Tileset

This is a graphical tileset for the TomeNET game (https://tomenet.eu/)

Its still in development.  
Right now there are tiles only for:
- **all character equipment**
- Mushrooms
- Scrolls 
- Tomes
- Wands
- Rods
- Staves
- Potions
- Runes

But will be more!)

## Example game view

![image](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/faf02db6-b696-45da-9ac8-9a275c831904)

![image](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/85b4b989-818b-4223-a7c4-64137b0e30a0)
![image](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/0e9b8170-d9d9-44f1-bb44-a60d39145272)
![image](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/12a6f97a-3d10-455d-96cb-71b609ffdf78)


## How to setup

### Linux 

1) copy `lib` folder into your `tomenet` folder
2) configure `~/.tomenetrc`: add graphics setup lines
```
graphics		1
graphic_tiles		16x22sv
```

### Windows
1) put `16x22sv.bmp`(from `lib/xtra/graphics`) in your `TomeNET/lib/xtra/graphics` folder (Create if doesn't exist) 
2) put `graphics-16x22sv.prf`(from `lib/user`) in your `C:/Users/%USERNAME%/TomeNET-user` folder
3) configure `TomeNET.ini`: find and update graphics setup lines
```
Graphics=1
GraphicTiles=16x22sv
```

## Problems

There are some known problems with using graphics right now:

- [monster list shows wrong tiles](https://github.com/TomenetGame/tomenet/issues/50)  
- [interface crash and packet errors if there is no graphic tiles for "Floor" features](https://github.com/TomenetGame/tomenet/issues/51)
- in character overview window items that have tiles are not displayed correctly
- Windows: game launch take much more time (few minutes)
