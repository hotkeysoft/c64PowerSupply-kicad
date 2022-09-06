# C64 Power Supply
Rev A June 2021

### Update September 2022

The power supply works okay, but needs improvement. I havent't tested it long term but enough to see the downsides of this version:

- The heat sink is a bit flimsy for long term use;
- It needs inrush current protection. I had to beef up the 5V side fuse to 2A and I'm probably just lucky it doesn't blow;
- The transformer is marginally OK for a C64, but underpowered for a C128 that uses ~2A on the 5V side;
- I kinda trust the LM2596 regulator (it's used everywhere), but for people a bit more paranoid, the circuit could use overvoltage protection on the 5V side;
- Not much protection on the mains side, could use a MOV or three. A fuse on the input side is probably a good idea too (but a fused power connector or in-line fuse can easily be added)

So I'll start working on Rev B, especially since I need a C128 power supply.

### Simple Switching Power Supply
- 120AC Input
- 9VAC Output 1.5A Max w/Fuse
- 5VDC Output 1.5A Max w/Fuse
- LM2596T-ADJ for +5V output
- +5V Adjustable with trimmer

Images
============
|Front                                                 | Back                                              |
|------------------------------------------------------|---------------------------------------------------|
|![Render Front](./img/render-front.jpg "Render Front")|![Render Back](./img/render-back.jpg "Render Back")|


![Render](./img/C64PowerSupply.jpg "Render")

### Schematics (pdf)
- [Complete schematics](./img/schema.pdf)

### PCB Images (svg)
- [Top](./img/pcb-front.svg)
- [Bottom](./img/pcb-back.svg)
