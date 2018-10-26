<!--lint disable list-item-indent-->
<!--lint disable list-item-bullet-indent-->
# Sensors

info's for the different Sensor Ideas that can be useful for interacting with the amulet

## Distance

use [VL53L1X](https://www.st.com/en/imaging-and-photonics-solutions/vl53l1x.html)  
4-400cm ToF 940nm Laser sensor

#### cover glass
![acryl glass - visible light](pictures/acrylglas_IR_visibillity__only_VISIBLE.png)
![acryl glass - IR light](pictures/acrylglas_IR_visibillity__only_IR.png)

use the blue one in combination with real black.
or transparent with black.  

create cover glass window in 'sandwich' variant -  
like explained in this [video](https://www.youtube.com/watch?v=BHM2CZVXZGc&feature=youtu.be&t=166)

#### TODO
- write CircuitPython driver
    - [check this topic for some starting points](https://forum.micropython.org/viewtopic.php?t=4827)

## Ambient-Light Level

use [TSL2591](https://ams.com/tsl25911#tab/documents)  
already has
[arduino](https://learn.adafruit.com/adafruit-tsl2591/wiring-and-test#raw-data-access-api-4-25) and
[CircuitPython](https://learn.adafruit.com/adafruit-tsl2591/python-circuitpython#full-example-code-6-15) libraries

## Touch

use [FDC1004](http://www.ti.com/product/FDC1004)?  
it has a shield so eventually it could work while hanging at the body?  

#### TODO
- test if this works
- write CircuitPython driver
