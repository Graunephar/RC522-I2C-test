PlatformIO example project showing how to use RC522 Mini in i2c mode. 

To set the breakout board in i2c mode you need to cut the connection grounding pin 1 as discussed in [this thread](https://forum.arduino.cc/index.php?topic=442750.0) on the arduino forum.

I used the drill method suggested by Renate-USB in above post. 

[This Library](https://github.com/arozcan/MFRC522-I2C-Library) is used to control the module.

Sketch modified from example found [here](https://www.teachmemicro.com/arduino-rfid-rc522-tutorial/)


**Connections**
(When in i2c mode the labels does not make sense anymore. Otherwise it would not make sense to connect MISO to SDA).

Arduino     RC522
SCL         SDA
SDA         MISO
3.3V        3.3V
GND         GND


| Arduino       | RC522         | 
| :-----------  | :----------:  | 
| SCL           | SDA           | 
| SDA           | MISO          |
| 3.3V          | 3.3V          |
| GND           | GND           | 

