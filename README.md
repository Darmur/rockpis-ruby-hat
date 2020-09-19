# RockPi-S Ruby-HAT

### HAT for RockPi-S with 0.96" OLED display, joystick, push-buttons, lineout jack and headphone jack (with dedicated amplifier)

#### Project description

![Ruby-HAT](https://github.com/Darmur/rockpis-ruby-hat/blob/master/RockPi-S_Ruby-HAT.Rev1.0.3D-01.png)

Ruby-HAT is an expansion board for [Radxa RockPi-S](https://wiki.radxa.com/RockpiS). It's been designed to fit in a compact volume together with the RockPi-S.


#### Specs

Ruby-HAT is powered by the following peripherals:

* 1x [0.96" I2C OLED Display Module](https://github.com/Darmur/rockpis-ruby-hat/blob/master/pictures/OLED_module.jpg), with 128x64 resolution, display controller [SSD1306](https://cdn-shop.adafruit.com/datasheets/SSD1306.pdf)
* 2x Tactile push-button
* 1x 5-way Tactile joystick [SKRHABE010](https://tech.alpsalpine.com/prod/e/html/multicontrol/switch/skrh/skrhabe010.html)
* 1x Lineout 3.5mm jack, connected to Lineout pins through DC-blocking capacitors
* 1x Headphone jack, connected to the dedicated headphone amplifier
* 1x Class AB headphone amplifier [PAM8908](https://www.diodes.com/assets/Datasheets/PAM8908.pdf), it can deliver up to 25mW per channel with very low distortion


#### What's available

* Schematic
* Layout
* Gerber
* Bill-of-Materials
* Pick&Place Centroid file

Nothing is missing for ordering bare or assembled PCBs from PCB manufacturers. The design has been made for keeping cost as low as possible, people with good soldering skills can try to solder all the components by hand, it's tricky but still doable.


#### How to use

For audio playback, any image with integrated DAC enabled will work out-of-the-box. It will be required to configure ALSA with software volume control, for increasing or lowering the volume of both lineout and headphone. 

For joystick and push-buttons connected to GPIOs, plenty of [libraries and examples](https://wiki.radxa.com/RockpiS/dev/libmraa) are available for implementing and using them in your own application. Please refer th the schematic for the mapping between buttons and GPIO number.

For controlling the OLED display, several [libraries and examples](https://luma-oled.readthedocs.io/en/latest/intro.html) are available as well, SSD1306 is a pretty common device. The display has been connected to the I2C bus #1.

#### Support

An official thread has been open on [Radxa forum](https://forum.radxa.com/t/rockpi-s-ruby-hat-opensource-hat-for-rockpi-s-with-lineout-headphone-oled-display-joystick-and-buttons/4476). Please feel free to report your experience and ask for support, if required.
