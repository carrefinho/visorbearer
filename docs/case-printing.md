# Case Printing Guide

## First Layer & LED Bezel

A good first layer is crucial since it is the exposed top surface of the board and at 0.08-0.12mm thin it enables the dead front effect of the LEDs.

### Build Plate

Finish will largely depend on the type of build plate which I’ve tested a few with varying results:

| Type | Finish | Notes |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------- | --------------- |
| YOOPAI Doubled Sided Epoxy | Nice and finely textured. Adhesion is not the best so corners might curl up a bit. | -0.04 Z offset |
| BIQU CryoGrip Glacier | A bit shinier and coarser texture than above but not bad. Very sticky; overall this is the most solid choice. | -0.025 Z offset |
| Bambu Lab Smooth PEI | Very smooth and matte finish when it works. some filaments show stress marks from removal. | -0.03 Z offset |
| Bambu Lab Cold Plate Supertack | Haven't been able to get a consistent finish with this. |  |
| Bambu Lab Textured PEI | Very pronounced texture; might have pinholes at 0.08mm layer height. Not recommended. | -0.04 Z offset |

Generally speaking, Z offset is increased from default values so the extra squish turns infill lines virtually invisible. Speed doesn't seem to matter much; feel free to crank it up if you're using CryoGrip.

### Filament Choice

Filament color wise, only neutral shades will show LED colors cleanly without tinting them. Lighter colors might show some light bleed around the case edges; so in practice that limits color choices to black and grey. Even among black and grey filaments there is quite a bit of variance in light transmission so it will take some trial and error. Here’s a couple I’ve tried:

| Filament | Notes | On Smooth PEI |
| ------------------------------ | -------------------------------------------------------------------------------------------------------------------- | ------------------------------------------ |
| Protopasta cMatte PLA Black | Just about the right amount of translucency at 0.08mm. Extremely matte side wall finish. | Works well. See photos in the main README. |
| Overture Matte PLA Black | Quite opaque, still quite dim at 0.06mm.  |  |
| Sunlu PLA Matte Black | Almost 100% opaque, doesn’t work at all. |  |
| Elegoo/Deeplee Matte PLA Black | Lets through quite a bit of light so I tend to use 0.12mm. | Shows stress marks. |
| Bambu Lab PLA Matte Nardo Grey | Works well at 0.1mm. |  |
| Elegoo/Deeplee Matte PLA Grey | Too translucent even at 0.12mm; might be okay at 0.2mm. The translucency does give it a nice soft edged look though. |  |

A variant with separate LED bezels is available if you want the case body in color and have a multi-color capable printer.

> [!NOTE]
> You can tweak the brightness of LEDs by using different valued current limiting resistors. See the [TI LP5012 datasheet](https://www.ti.com/lit/ds/symlink/lp5012.pdf) on how to calculate values. Default is 15kΩ for 4.9mA per channel; higher values result in lower current/dimmer LEDs, and vice versa.