###### FMC 2 ZMOD adapter
## What? 
This Mezzanine Card allows you to connect 2 ZMOD adapters. For example for connecting the Zmod ADC 1410 and Zmod DAC 1411 SYZYGY modules on the Digilent Genesys ZU.

## Why? 
Many FPGA boards have a FMC port. The Genesys ZU board has only one SYZYGY ZMOD connector, but also has a FMC port. Many applications, such as software defined radio (SDR), profit from both a high speed ADC and DAC. This FMC adapter allows you to connect 2 ZMOD modules. 

## Are you sure this works? 
I'am not an electrical engineer - and as such cannot guarantee that you won't fry your board(s). It was tested to work with the Genesys ZU and the code in the [marcvhoof/genesys-zu-notes repository](https://github.com/marcvhoof/genesys-zu-notes). Some parts of the SYZYGY specification are not implemented (yet). Such as the I2C functionality, module detection and power configuration. Feel free to modify and improve. 

## How do I get one? 
For testing purposes more were assembled and as such, I have a few left. So if you want an assembled board, without the connectors, feel free to reach out to me. I'd be happy to send you a board for shipping costs. If you want to assemble a board yourself, follow the guide. 

## Prerequisites
- a board with a FMC port
- a software implementation (see [marcvhoof/genesys-zu-notes repository](https://github.com/marcvhoof/genesys-zu-notes) )

# 1. Upload the board files to a PCB(A) service
I used [JLPCB]{jlpcb.com). Take JLC7628 for impedance control. I paid 44$ including shipping and assembly for 5 boards. You need to order a stencil if you don't want to create this yourself. 

# 2. Order the connectors
The connectors are not in the standard inventory. You can find them in different places. 
FMC Samtec - [ASP-134604-01](https://mouser.com/ProductDetail/200-ASP-134604-01) - 1 per board
ZMOD Samtec - [QSE-020-01-L-D-A](https://mouser.com/ProductDetail/200-QSE02001LDA) - 2 per board

# 3. Assemble the connectors
# 4. Build the software part of your project
# 5. Test
# 6. Let me know if you have succesfully used it for other applications

## Credits
Footprints - [dirtypcbs.com](dirtypcbs.com)
PCB layout - Ádám Cseke

