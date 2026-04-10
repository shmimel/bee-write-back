# Bee Write Back

![Bee Write Back WriterDeck](images/bee-write-back.jpg)

## Table of Contents

- [Introduction](#introduction)
- [Build Guide](#build-guide)
- [Hardware](#hardware)
- [Software](#software)
- [Cost](#cost)

## Introduction

I struggled to fall alseep easily for a while, and after being recommended journaling I found that it helped me immensely. The one catch was that I didn't like writing in a physical journal, since I would be greeted by all of my previous entries and all the emotions would come flooding back.

To solve this problem, I created a simple Raspberry Pi based journal, which I could use each night, entering in the chaos of the day, locking it away once I was done. After creating this, I found that the form factor of the writerdeck was really fun to use, and began developing more apps and functions, including a Claude chat client.

## Build Guide

![Bee Write Back Components](images/BOM.jpg)
  
You can view the PDF [here](Hardware/Bee%20Write%20Back%20Build%20Guide.pdf)  
Or the assembly video [here](https://youtu.be/JutsTp7yeNU)
And when you're ready to print, check out the print profile [here](https://makerworld.com/en/models/2643352-bee-write-back-diy-writerdeck#profileId-2921008)  
  
P.S. if you're curious, try spinning around the 3D model [here](https://cad.onshape.com/documents/e6482d1ab00cb5a2719e37b7/w/38d6de8130338c05d74e4ecf/e/8865c15cb975933cc3691846?renderMode=0&uiState=69bdc61baa0cf63feb704019). Onshape is free, and I highly encourage taking a look at the model in 3D!

## Hardware

![CAD](images/CAD.png)

You can find STEP and STL files available in the [CAD](Hardware/CAD) directory

If you want to 3D print this, you can find the STLs and 3MF files in the [Print](Hardware/CAD/Print) directory.

Since the faceplate and base utilizes multicolor printing, I have included a 3MF file. If you don't have access to multicolor printing or just want a blank faceplate, the regular STL will work. I printed my deck out of PLA, but PETG would also work.

## Software

I have included the two scripts that I vibe coded (I know it's lazy, but I have a background as a mechanical engineer, so programming is not my strong suit).

My current setup revolves around using 3 virtual terminals:
1. Standard terminal
2. Claude chat
3. Journal

In the Software folder, you will also find my .bashrc and .bashprofile file, which contain small tweaks to make switching virtual terminals as easy as possible.

## Cost

For more a more detailed breakdown of the cost for each variant, please reference the individual BOMs in their respective directory. Below are the rough totals for each variant. Screws and filament are not included in the total cost.

**TOTAL COST: $200**

(This number does not include shipping, taxes and/or tariffs)