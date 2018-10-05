<!--lint disable list-item-indent-->
<!--lint disable list-item-bullet-indent-->
# Magic Amulet

a amulet with an power / guarding animal / creature

- it can magical glow
- useful as prop
- motive can be easily changed

![overview amulet](amulet.png)
![finished - detailed](./pictures/P1680869_small.jpg)
![finished - with controller](./pictures/P1680868_small.jpg)


## features
- material
    - wood
    - acrylic
- glowing / lighting effects
- creature / animal / symbol ideas
    - see [inspiration.md](inspiration.md)
    - saurian
    - lizard
    - owl
    - phoenix
    - dragon
    - moon
    - star
    - flower of life
    - tree of life

TODO: add art on front wood
![some idea sketches](ideas.svg)

## housing
the housing is build from 4 Layers of 4mm pine plywood parts.  
the Acrylic inlay consists of 4 2mm parts.  
the Backside is hold by 3 M3-Screws.  
for this the nuts are inserted before the first three plywood parts
(front, in_front, in_back) are glued together.

## rope
- [Hanfseil HEMPBRAID von Kanirope ø5mm Meterware (lfm) 16-fach geflochten](https://www.kanirope.de/hanfseil-hempbraid-kanirope-5mm-meterware-lfm-16-fach-geflochten)

this rope has a core that can be exchanged with cables.
![rope - core visible](./pictures/P1680854_small.jpg)
![rope with cable](./pictures/P1680851_small.jpg)
![fitting the rope](./pictures/P1680857_small.jpg)


## electronic

→ currently there is a APA102 60LEDs/m pixel-strip (3 segments with each 4LEDs)
fitted. (this was to get done in time :smile:)
![soldering APA102 strip in place](./pictures/P1680803_small.jpg)


the electronic parts are hand-soldered / assembled.
for this there is a helper that can be manufactured out of >= 1mm cardboard
![soldering helper](led_soldering_helper.svg)
→ first iteration of this did not work. holes are to big.
but i managed to create a working test:
![hand-solder prototype](./pictures/P1680990_small.jpg)
![hand-solder prototype](./pictures/P1680991_crop.jpg)
![hand-solder prototype](./pictures/P1680995_crop.jpg)

TODO: design pcb  
see [LEDBoard_1x4_16bit_highdensity](https://github.com/s-light/LEDBoard_1x4_16bit_highdensity/)

### planed parts
- LEDs: Nichia 124
- driver: TLC5971
