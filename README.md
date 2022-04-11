# ELPixel

This project tries to make it easy to control EL wire as if it were a ws2811 LED. Why? I wanted to make dance costumes that had both LEDs and EL wire, and I wanted to do it with xLights and ESPixel. Therefore, the easiest way seemed to be to make the EL wire work like an LED!

## How it works

The board contains two simple circuits, the WS2811 IC circuit and the HV850 IC circuit. The WS2811 reads the signals and converts to 0-5v outputs on the R, G, and B outputs. The R output is then fed as input to the HV850 circuit. 0v will mean off, 5v will mean on, and a voltage in the middle will dim the EL wire (maybe?). In xLights, you can set it up so the visualization reflects the color of the EL wire instead of being "red". The choice o the R channel was arbitrary.
