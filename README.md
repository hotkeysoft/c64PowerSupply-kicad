# C64 Power Supply
Rev B September 2022

### Work in progress, untested

Will update when build & tested

### Simple Switching Power Supply
- 120/240VAC Input (toggle with jumpers)
- Beefier transformer (56VA)
- TVS diodes on both transformer output lines (optional)
- MOV and filtering cap on input side (optional)
- 9VAC Output 1.5A Max w/Fuse
- 5VDC Output 3A Max w/Fuse, more than enough for C128
- +5V Adjustable with trimmer
- BD9E303EFJ Buck switching regulator for +5V output
  - In theory more efficient than old LM2596T, tests will tell 
- Two terminal blocks to use the power supply with either a C64 or a C128
  - *NOT* at the same time...
    - 9VAC line should be fine in theory (transformer can provide 3A). Altough noise/crosstalk could be an issue.
    - 5V line could overload. The max capacity of this switching regulator is 3A. C128 uses around 2A by itself, with nothing connected. C64 is rated to use 1.5A. Not responsible if someone powers both at the same time.

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
