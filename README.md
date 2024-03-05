# TomeNET-Tileset

This is a graphical tileset for the TomeNET game (https://tomenet.eu/)

Its still in development.  

**Roadmap:**
- [x] objects
- [ ] terrain
- [ ] monsters

Right now there are tiles only for objects(_stuff that you can put in you inventory_), like:
- **all character equipment**
- Mushrooms
- Scrolls 
- Tomes
- Wands
- Rods
- Staves
- Potions
- Runes
- etc.

## Example game view (with TG font)

![image](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/faf02db6-b696-45da-9ac8-9a275c831904)
![image14](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/4f590da0-66fa-4479-bf87-06d1a693b42e)

![image4](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/784f6ff1-e453-4c96-bcdc-2962fd2f3af3)
![image6](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/68555195-cdaa-4e93-a4ec-7e0578bed106)

![image](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/627d8aee-6d76-44a3-bc91-a039005cd1a5)
![image](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/12a6f97a-3d10-455d-96cb-71b609ffdf78)
![image](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/85b4b989-818b-4223-a7c4-64137b0e30a0)
![image3](https://github.com/EvgenijK/TomeNET-Tileset/assets/8179946/50b84d68-398a-4b58-96cc-297b10003bd9)

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

- monster list shows wrong tiles https://github.com/TomenetGame/tomenet/issues/50
- interface crash and packet errors if there is no graphic tiles for "Floor" features https://github.com/TomenetGame/tomenet/issues/51
- in character overview window items that have tiles are not displayed correctly
- Windows: game launch take much more time (few minutes)
- [SOLVED] fps slowndown if there are many graphic tiles on screen https://github.com/TomenetGame/tomenet/issues/59
