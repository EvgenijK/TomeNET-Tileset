# TomeNET-Tileset

This is a graphical tileset for the TomeNET game (https://tomenet.eu/)

## Current state

The tileset still in development.  
Currently there is only 16x22 size.  
All items/objects and terrain completed, more sizes goal is the next.

**Roadmap:**
- [x] objects
- [x] terrain
- [ ] more sizes
- [ ] monsters

## 16x22 ASCII font

Because there is no 16x22 ASCII font in TomNET to use with 16x22 graphics here is 16x22 ASCII font based on 16x24 font from the game.  
Font files(`*.fon`(for Windows) and `*.pcf`(for Linux)) located in `lib/font` folder.  
See [(2.5a) Custom fonts](https://www.tomenet.eu/guide.php?chapter=2.5a) chapter in the Guide for the "how to set up" font.  

## Current game view (with TG font)

**[More screenshots with ASCII font below](#more-screenshots)**

![image](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/faf02db6-b696-45da-9ac8-9a275c831904)
![image14](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/4f590da0-66fa-4479-bf87-06d1a693b42e)

![image4](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/784f6ff1-e453-4c96-bcdc-2962fd2f3af3)
![image6](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/68555195-cdaa-4e93-a4ec-7e0578bed106)

![image](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/627d8aee-6d76-44a3-bc91-a039005cd1a5)
![image](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/12a6f97a-3d10-455d-96cb-71b609ffdf78)
![image](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/85b4b989-818b-4223-a7c4-64137b0e30a0)
![image3](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/50b84d68-398a-4b58-96cc-297b10003bd9)

## How to setup

First you need to use the test client as solution to avoid the several minutes of startup freeze in regular client.
Windows only, link in bottom of the page: https://www.tomenet.eu/downloads.php?  
For Linux you have to compile the client from soutce to get the test version.

It might be needed to turn off "Solid walls" setting in `=1 font_map_solid_walls` to avoid seeing wrong tiles.

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

- Windows: bmp from github seems to be corrupted when using in windows. Re-saving it in graphic editor solved the issue (like in Paint)
- monster list shows wrong tiles https://github.com/TomenetGame/tomenet/issues/50
- interface crash and packet errors if there is no graphic tiles for "Floor" features https://github.com/TomenetGame/tomenet/issues/51
- in character overview window items that have tiles are not displayed correctly
- Windows: game launch take much more time (few minutes)
- [SOLVED] fps slowndown if there are many graphic tiles on screen https://github.com/TomenetGame/tomenet/issues/59

# More screenshots

### Bree
![Снимок экрана_20240609_132159](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/b6bddbfa-f83c-4d2a-a3d6-358ba1216e47)

### Player houses
![Снимок экрана_20240609_132312](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/a22a2740-2df1-4e05-be90-c3f67246f02f)
![Снимок экрана_20240609_132350](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/89b8fa4e-eb55-4e66-9c1d-5391e8a28dd6)
![Снимок экрана_20240609_132539](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/518643b0-3201-4701-be4a-f23e20d6e609)

### Training tower
![Снимок экрана_20240609_132712](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/bba5e165-ce40-4bac-8bc8-9ecb51bff2a9)

### Barrow Downs
![Снимок экрана_20240609_132843](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/cd111840-6f16-4f83-9fa3-06d2ff4aed41)

### Mordor
![Снимок экрана_20240609_134739](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/f6ca0303-4d40-42e4-a5bf-b87b37e2a36a)

### Helcaraxe
![Снимок экрана_20240609_134223](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/48897eee-ae21-4b1e-83fa-6361c7dfe2fd)

### Angband
![Снимок экрана_20240609_133344](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/bda99f50-3da1-4ff1-9dd3-5791e50bf6dc)
![Снимок экрана_20240609_133551](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/5636d81b-36e5-4591-a4ba-f829c957e68a)

### Mount Doom
![Снимок экрана_20240609_133916](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/36005528-504b-4eae-bd8e-9f696ff43f4b)
![Снимок экрана_20240609_133938](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/17572882-4ca4-4b19-b141-c81017f89c81)

### Mirkwood and Old Forest
![Снимок экрана_20240609_134036](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/a36fc831-6b13-408b-8b42-a3df313ecf77)
![Снимок экрана_20240609_134140](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/a175b384-3ba4-47b9-8bf4-34e2beb59099)
