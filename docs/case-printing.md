# Case Printing Guide

## Top Case

### First Layer & LED Bezel

A good first layer is crucial since it is the exposed top surface of the board. At 0.08-0.12mm thickness, it enables the dead-front effect of the LEDs.

#### Build Plate

Finish will largely depend on the type of build plate. I've tested a few with varying results:

| Type | Finish | Notes |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------- | --------------- |
| YOOPAI Doubled Sided Epoxy | Finely textured finish. Adhesion is not the best; corners might curl up slightly. | -0.04 Z offset |
| BIQU CryoGrip Glacier | Slightly shinier and coarser texture than YOOPAI. Very sticky; **best choice overall**. | -0.025 Z offset |
| Bambu Lab Smooth PEI | Very smooth and matte finish when it works. Some filaments show stress marks after removal. | -0.03 Z offset |
| Bambu Lab Cold Plate Supertack | Haven't been able to get a consistent finish with this. |  |
| Bambu Lab Textured PEI | Very pronounced texture; might have pinholes at 0.08mm layer height. Not recommended. | -0.04 Z offset (default)|

Z offset is increased from default values; the extra squish makes infill lines virtually invisible. Speed doesn't matter much, so feel free to crank it up if you're using CryoGrip.

#### Filament Choice

Only neutral shades (black and grey) will display LED colors cleanly without tinting. Lighter colors may show light bleed around case edges. Even among black and grey filaments, light transmission varies significantly and will require some experimentation. Here are a few I've tested:

| Filament | Notes | On Smooth PEI |
| ------------------------------ | -------------------------------------------------------------------------------------------------------------------- | ------------------------------------------ |
| Protopasta cMatte PLA Black | About the right amount of translucency at 0.08mm. Extremely matte side wall finish. | Works really well. See photos in the main README. |
| Overture Matte PLA Black | Very opaque; still quite dim at 0.06mm. |  |
| Sunlu PLA Matte Black | Almost 100% opaque, doesn’t work at all. |  |
| Elegoo/Deeplee Matte PLA Black | Lets through quite a bit of light; I use 0.12mm. | Shows stress marks. |
| Bambu Lab PLA Matte Nardo Grey | Works well at 0.1mm. |  |
| Elegoo/Deeplee Matte PLA Grey | Too translucent even at 0.12mm; might work at 0.2mm. The translucency gives it a nice soft-edged look though. |  |

A variant with separate LED bezels is available if you want a colored case body and have a multi-color printer.

> [!NOTE]
> You can tweak the brightness of LEDs by using different valued current limiting resistors. See the [TI LP5012 datasheet](https://www.ti.com/lit/ds/symlink/lp5012.pdf) on how to calculate values. Default is 15kΩ for 4.9mA per channel; higher values result in lower current/dimmer LEDs, and vice versa.

### Print Settings

| Setting | Value | Notes |
| ------- | ----- | ----- |
| Layer Height | 0.15mm |  |
| Walls printing order | Inner/Outer/Inner | Helps with outer wall quality. |
| Wall loops | 3 | Required for Inner/Outer/Inner order. |
| Enable support | Y | For USB cutout overhang. |
| Support: Type | tree |  |
| Support: Top Z distance | 0.2mm |  |
| Support: Interface pattern | Concentric |  |
| Support: Top interface spacing | 0mm |  |
|  |  |  |
|  |  |  |

## Switch Plate and Bottom Cover

These parts are less critical in appearance as they are mostly hidden. Standard print settings should work fine.