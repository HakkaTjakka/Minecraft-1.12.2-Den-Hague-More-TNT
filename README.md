*********************************************************** FLOODFILL 1.15.2 ********************************************************************

Floodfill for 1.15.2 fixed. 
See world/datapacks for fill function.
Or place floodfill.zip into world/datapacks dir. (not both).
Use self powered command block (how to details see below) with /function exxabite:fill

fill.mcfunction: saves\More-TNT\datapacks\floodfill\data\exxabite\functions\fill.mcfunction contents:

fill ~ ~-1 ~ ~ ~-1 ~ minecraft:repeating_command_block{Command:"function exxabite:fill",auto:1b} keep

fill ~ ~ ~1 ~ ~ ~1 minecraft:repeating_command_block{Command:"function exxabite:fill",auto:1b} keep

fill ~ ~ ~-1 ~ ~ ~-1 minecraft:repeating_command_block{Command:"function exxabite:fill",auto:1b} keep

fill ~1 ~ ~ ~1 ~ ~ minecraft:repeating_command_block{Command:"function exxabite:fill",auto:1b} keep

fill ~-1 ~ ~ ~-1 ~ ~ minecraft:repeating_command_block{Command:"function exxabite:fill",auto:1b} keep

setblock ~ ~ ~ minecraft:water

file: saves\More-TNT\datapacks\floodfill\pack.mcmeta contents:

{
  "pack": {
    "pack_format": 5,
    "description": "Exxabite's flood fill datapack"
  }
}

*********************************************

Latest news: Directory with region files truncated to 1000 files :( , so download from Google drive. https://drive.google.com/drive/folders/1CpZNVoF67IbI-6axhiI0VhlXajw9B1Pf
(Meanwhile try to rar them into 1 GB files).

# Minecraft-1.12.2-Den-Hague-More-TNT
More TNT

(Short) sample(s):

https://www.facebook.com/gerard.wensink/videos/3408524012543515/

https://www.youtube.com/watch?v=h_L3k7FgbAc

Changed code for more TNT (two east west and two north south tunnels).

Download also from: https://drive.google.com/drive/folders/1CpZNVoF67IbI-6axhiI0VhlXajw9B1Pf

Tell me on: https://www.facebook.com/Minecraft-Worldeditor-110607880303634/ if you like it.

Other worlds: 

Large tunneled boobytraped indoor maze: https://drive.google.com/drive/folders/17jv6QdazFIbb9YjeYdk4_STRRydNjQYt?usp=sharing
Enschede, The Netherlands, BTE (Build The Earth 121 projection): https://drive.google.com/drive/folders/11OMOV-JhyPRYNm3qXhCrOgGFZ0zEeBfk?usp=sharing
Enschede (diff. scale, Amsterdam, Amsterdam small/large, maze): https://drive.google.com/drive/folders/1RuIClj5k9hI7i3NJv5cLOhdohfn4S9tR?usp=sharing

Source code: https://github.com/HakkaTjakka/MinecraftWorldEditor

Do you want to create schematics / region files from 2d / 3d source (voxelizer), i will help you out installing and using, it is a whole process..


*********************************************************** FLOODFILL 1.12.2 ********************************************************************
(Put in saves/world/data) 

Create self powered command_block:

/give @me minecraft:command_block

Command: /function exxabite:fill

(Maybe comment (‘#’) out statements in saves/world/data/exxabite/fill.mcfunction first).
/reload

Put block down, copy to inventory: ctlr + middle mouse button.

(Then uncomment (‘#’) out statements in saves/world/data/exxabite/fill.mcfunction).
/reload

(Block gets active then….) 

Block is inside level.dat.

Runs only on 1.12.2 till now. 
(need info on directory for functions and usage of fill/setblock command.

Place block -> floodfill (left/right, north/south, down). Replacing only air to water.

Command in repeating/self powered command block:

 “/function exxabite:fill” (without the quotes)

File in: saves/world/data/exxabite/fill.mcfunction

fill ~-1 ~ ~ ~-1 ~ ~ repeating_command_block 0 keep {Command:"/function exxabite:fill",auto:1b}

fill ~1 ~ ~ ~1 ~ ~ repeating_command_block 0 keep {Command:"/function exxabite:fill",auto:1b} 

fill ~ ~ ~-1 ~ ~ ~-1 repeating_command_block 0 keep {Command:"/function exxabite:fill",auto:1b} 

fill ~ ~ ~1 ~ ~ ~1 repeating_command_block 0 keep {Command:"/function exxabite:fill",auto:1b}

fill ~ ~-1 ~ ~ ~-1 ~ repeating_command_block 0 keep {Command:"/function exxabite:fill",auto:1b}

setblock ~ ~ ~ water

https://youtu.be/6qW7vLGR_4w

