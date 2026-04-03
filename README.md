# Bee Write Back

![Bee Write Back WriterDeck](images/writerdeck_1.jpeg)

## Table of Contents

- [Introduction](#introduction)
- [Build Guide](#build-guide)
- [Hardware](#hardware)
- [Software](#software)
- [Cost](#cost)

## Introduction

I struggled to fall alseep easily for a while, and after being recommended journaling I found that it helped me immensely. The one catch was that I didn't like writing in a physical journal, since I would be greeted by all of my previous entries and all the emotions would come flooding back.

To solve this problem, I created a simple Raspberry Pi based journal, which I could use each night, entering in the chaos of the day, locking it away once I was done. After creating this, I found that the form factor of the writerdeck was really fun to use, and began developing more apps and functions, including a Claude chat client.

After creating the first one, I wanted to make it as cheap and available as possible, so I took the CAD model and adapted it for an old Android phone.

[![Bee Write Back Demo Video](https://img.youtube.com/vi/mUFC60MM2Fw/0.jpg)](https://youtu.be/mUFC60MM2Fw)

^ Click me to watch a quick demo ^

## Build Guide

Since this is still a WIP, and I am ironing out some small changes, I have not created a formal build guide yet. However, I have put together a [BOM](Hardware/BOM.md) and a [block diagram](images/block.png) for now. Expect a build guide soon!  

## Hardware

You can find STEP and STL files available in the [CAD](Hardware/CAD) directory, or if you want to go spin the model around, you can check it out in Onshape [here](https://cad.onshape.com/documents/e6482d1ab00cb5a2719e37b7/w/38d6de8130338c05d74e4ecf/e/8865c15cb975933cc3691846?renderMode=0&uiState=69bdc61baa0cf63feb704019). Onshape is free to use (but all designs are public), so I encourage you to create an account and start learning about CAD.


If you want to 3D print this, you can find the STLs and 3MF files in the [Print](Hardware/CAD/Print) directory.

Since the faceplate utilizes multicolor printing, I have included a 3MF file. If you don't have access to multicolor printing or just want a blank faceplate, the regular STL will work. I printed my deck out of PLA, but PETG would also work.

## Software

I have included the two scripts that I vibe coded (I know it's lazy, but I have a background as a mechanical engineer, so programming is not my strong suit).

My current setup revolves around using 3 virtual terminals:
1. Standard terminal
2. Claude chat
3. Journal

In the Software folder, you will also find my .bashrc and .bashprofile file, which contain small tweaks to make switching virtual terminals as easy as possible.

## Cost

For more a more detailed breakdown of the cost for each variant, please reference the individual BOMs in their respective directory. Below are the rough totals for each variant. Screws and filament are not included in the total cost.

**TOTAL COST: $270**

(This number does NOT include shipping, taxes and/or tariffs)