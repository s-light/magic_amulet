<!--lint disable list-item-indent-->
<!--lint disable list-item-bullet-indent-->
# Interconnection

this document describes ideas and concepts to interconnect the amulet with the controller / power box.

## data
for Data use LVDS or RS485 / RS422 to get the HighSpeed Signals from the controller to the LEDBoards.

[Recommend LVDS or RS422 / RS485 Driver and Receiver Pair for ~30MHz Signals](https://e2e.ti.com/support/interface/f/138/t/755140)

Hello TI-Community,

i have a 'art project' (costume) where i have some LED-Drivers (TLC5957) about 2meters away from my controller.
The Drivers have multiple Signals (GrayscaleClock, SignalClock, SignalData, Latch) that can go up to 30MHz.
So my Idea was to use RS485 / RS422 or LVDS to transmit this over the 2meter.

My Power Supply and IO Voltage is all 3.3V.
Can you Recommend any Drivers for this type of Application?
do i have advantages choosing one over the other technology?

for RS422 i have found this Pair:
- [AM26LV31E Low-Voltage High-Speed Quadruple Differential Line Driver With +/-15-kV IEC ESD Protection](http://www.ti.com/product/AM26LV31E)
- [AM26LV32E Low-Voltage High-Speed Quadruple Differential Line Receiver With +/-15-kV IEC ESD](http://www.ti.com/product/AM26LV32E)

for LVDS i have found this Pair:
- [SN65LVDS391 Quad LVDS Driver](http://www.ti.com/product/SN65LVDS391)
- [SN65LVDT348 Quad Receiver with -4 to 5V Common-mode Range](http://www.ti.com/product/SN65LVDT348)

is either a good choice?
or are there any other better suited parts?
additionally i have found this Info:
- [TI Designs: TIDA-060017 Transmitting SPI Signals Over LVDS Interface Reference Design](http://www.ti.com/lit/ug/tidued8/tidued8.pdf)
- [Blog - Get Connected: How to extend an SPI bus through a differential interface](https://e2e.ti.com/blogs_/b/analogwire/archive/2015/02/13/extending-spi-with-differential-signaling-technology)

i hope you can give me some tips :-)

sunny greetings
stefan

### cable

[SMARTflex Cat.6A U/UTP AWG32 LSOH Schwarz 5,0m](https://aixontec.com/SMARTflex-Cat6A-U-UTP-AWG32-LSOH-Schwarz-50m) 7.95€ + 5.9€ = 13.85€
super thin cable- with outer diameter of 2.8mm

### connector

[RJ45 connector - Bel SS-6488S-A-NF](https://www.mouser.de/ProductDetail/530-SS-6488S-A-NF) [datasheet](https://belfuse.com/resources/drawings/stewartconnector/dr-stw-ss-6488s-a-nf.pdf)

---

## power

use LiFePo4
```
4S
2.0V \* 4 = 8V
3.2V \* 4 = 12.8V
3.6V \* 4 = 14.4V
```

### cable

- [TKD - 01.05.01 HIGHFLEX LIFY](https://www.tkd-kabel.de/de/loesungen/produktbezogen/node-01.05-41/)
    price requested per mail
- [daims-kabelshop.de - 0,35mm² silicon highly flexible](https://shop.strato.de/epages/63697912.sf/sec9f439b4be0/?ObjectPath=/Shops/63697912/Products/20110/SubProducts/20110) 0.5€/m
- [daims-kabelshop.de - 0,50mm² silicon highly flexible](https://shop.strato.de/epages/63697912.sf/sec9f439b4be0/?ObjectPath=/Shops/63697912/Products/20200/SubProducts/20200) 0.6€/m
- [daims-kabelshop.de - 0,75mm² silicon highly flexible](https://shop.strato.de/epages/63697912.sf/sec9f439b4be0/?ObjectPath=/Shops/63697912/Products/20300/SubProducts/20300) 0.8€/m


### StepDown Converter

[2.95V to 17V, 10A Step-Down Power Module with Current Sharing in 10x10x4.3mm QFN Package](http://www.ti.com/product/lmz31710)
([mouser: 10,09€](https://www.mouser.de/Search/Refine.aspx?Keyword=LMZ31710))
