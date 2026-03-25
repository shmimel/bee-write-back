# Bee Write Back

![Bee Write Back WriterDeck](images/deck.jpeg)

## Introduction

I struggled to fall alseep easily for a while, and after being recommended journaling I found that it helped me immensely. The one catch was that I didn't like writing in a physical journal, since I would be greeted by all of my previous entries and all the emotions would come flooding back.

To solve this problem, I created a simple Raspberry Pi based journal, which I could use each night, entering in the chaos of the day, locking it away once I was done

After creating this, I found that the form factor of the writerdeck was really fun to use, and began developing more apps and functions, including a Claude chat client.

#### Future plans include:
- Live coding music workspace
- Simple synthesizer
- Mixxx ASCII GUI
- Better battery management

## Sounds cool, I want to make one!

Since this is still a WIP, I don't have a full build guide just yet, but feel free to modify and use the materials that I used as a starting point.

I recently ordered a PiJuice Zero, and will update if this ends up being the best solution for battery management.

You can find STEP and STL files available in the [CAD](CAD) directory, or if you want to go spin the model around, you can check it out in Onshape [here](https://cad.onshape.com/documents/e6482d1ab00cb5a2719e37b7/w/38d6de8130338c05d74e4ecf/e/8865c15cb975933cc3691846?renderMode=0&uiState=69bdc61baa0cf63feb704019). Onshape is free to use (but all designs are public), so I encourage you to create an account and start learning about CAD!


[![Bee Write Back Demo Video](https://img.youtube.com/vi/mUFC60MM2Fw/0.jpg)](https://youtu.be/mUFC60MM2Fw)

^ Click me to watch a quick demo ^

## 3D Printing

If you want to 3D print this, you can find the STL's and 3MF files in the [CAD](CAD) directory.

Since the faceplate utilizes multicolor printing, I have included a 3MF file. If you don't have access to multicolor printing or just want a blank faceplate, the regular STL will work.

I printed everything out of PLA, with no supports, but I would assume that any material (minus TPU) would work well.

I plan to make a two part version that can fit on the bed of the Bambu Lab A1 Mini.

## Software

I have included the two scripts that I vibe coded (I know it's lazy, but I have a background as a mechanical engineer, so programming is not my strong suit).

My current setup revolves around using 3 virtual terminals:
1. Standard terminal
2. Claude chat
3. Journal

I will soon add on a little tutorial file on how to enable 3 different terminals. There are also a few other tweaks I made, such as disabling login text for a cleaner UI experience.

I have tried to keep everything as minimal and light as possible, so the scripts require Python and the Anthropic API packages to run.

## Parts List

| Part | Qty | Cost | Link | Notes |
|-----|-----|-------|-------|-------|
| Raspberry Pi Zero W | 1 | $15 | [raspberrypi](https://www.raspberrypi.com/products/raspberry-pi-zero-2-w/) | Any Pi Zero variant works |
| 5.5" AMOLED Screen | 1 | $45 | [aliexpress](https://www.aliexpress.us/item/3256805978359959.html?channel=twinner) | Any HDMI screen will work, but enclosure will need redesign|
| Air40 Keyboard PCB | 1 | $35-$45 | [aliexpress](https://www.aliexpress.us/item/3256805656168067.html?channel=twinner) | Non-Hot Swap variant works as well | 
| UPS Hat | 1 | $25 | [waveshare](https://www.waveshare.com/ups-hat-c.htm) | Any 3.7V Lipo battery w/ JST connector works|
| Keyboard Switches | 47 | ~$20 | [hippokeys](https://hippokeys.com/) | Any MX style switch works |
| Keycaps | 47 | $14 | [chosfox](https://chosfox.com/products/chosfox-geonix-rev-2-original-keycap-set) | Any MX keycap set will work |
| Right angle USB C Adapter | 1 | $9 | [amazon](https://a.co/d/0iD8tdOh) | Make sure to get the **right** variant |
| USB C to Micro B Cable | 1 | $8 | [amazon](https://a.co/d/02apOZqa) | I used the 1 foot variant, any brand will do |
| FPC Mini HDMI to HDMI Cable | 1 | $9 | [amazon](https://a.co/d/05EBCFm5) | Make sure to get 0.2M variant |
| FPC Mini HDMI connector | 1 | $7 | [amazon](https://a.co/d/0dyc08eN) | Unfortunately there are no mini-to-mini FPC cables, this replaces the standard HDMI connector |
| USB C Cable | 1 | $2 | [amazon](https://a.co/d/090tin6A) | Any USB C to 5V and GND bare wire will do |
| Machine Screws| 6 | ~$1 | [amazon](https://a.co/d/0e3UtxS2) | Any M3 x 25mm screw will do |
| Self Tapping Screws | 12 | ~$1 | [amazon](https://a.co/d/05gDwUqy) | 8x M2.6 x 8mm, 4x M2.3 x 5mm |
| Wires | ~ | ~ | ~ | Need to figure out better wiring solution |
| PLA Filament | ~ | ~ | ~ | Will update with exact filament usage |

**Total: ~$200**

## Issues

The OLED screen that I sourced arrived crooked, meaning that I had to adjust the mounting holes on the screen holder. I plan to make the holes larger and incorporate washers to accomodate for this discrepancy.

The battery life sucks right now, and the power switch does a full power cycle when flipped. Hopefully with the PiJuice Zero I can integrate a sleep mode.

## TODO

- [x] Create Github repo
- [x] Record demo for Youtube
- [ ] Integrate PiJuice power hat
- [ ] Integrate I2S audio hat
- [ ] Clean up wiring (custom PCB?)