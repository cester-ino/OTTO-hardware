## OTTO-project
Hardware prototype for the [OTTO Synthesizer by Topisani](https://github.com/topisani/OTTO "OTTO Synthesizer by Topisani")

![prototype rendering](https://raw.githubusercontent.com/cester-ino/OTTO-hardware/dev/img/alu.png)
*10x10 silicone buttons with led backlight*

Main features
####Mainboard
- ILI9341 based TFT 2.8" TFT screen.
- 4 low profile clickable encoders
- 40 function keys
- STM32F103VET6 mcu
- Raspberry GPIO connector
- connects to all the various boards
- expansion headers

####Power board
- 2A 5-16V DC input & 500mah micro usb input
- [MAX8903A](https://datasheets.maximintegrated.com/en/ds/MAX8903-MAX8903Y.pdf "MAX8903A") 1s Lipo charger IC with path management
- 5V 2A DC-DC boost converter ([TPS61090](http://www.ti.com/lit/ds/symlink/tps61090.pdf "TPS61090")) & 3V3 700mah LDO ([XC6210](https://www.torexsemi.com/file/xc6210/XC6210.pdf "XC6210"))
- [MAX17048](https://datasheets.maximintegrated.com/en/ds/MAX17048-MAX17049.pdf "MAX17048") 1s lipo fuel gauge, connected via i2c to the raspberry
- [pi_power](https://github.com/craic/pi_power "pi_power") circuit for monitoring and control boot and shutdown routine

####Audio Board
- SGTL5000 Audio Codec
- Electret microphone amp circuit
- LM4860 speaker amplifier
- 1 TRS jack line IN
- 1 TRS jack line OUT
- 1 Headphone IN

####Keyboard
- 2 octaves keyboard with 16 keys bottom row
- expansion headers
- 16 addressable rgb leds

those specs refer to the tactile buttons version, but a led backlight button version is in the works too.

![prototype rendering](https://raw.githubusercontent.com/cester-ino/OTTO-hardware/dev/img/OTTOtac.png)
*one of the first design iteration*

