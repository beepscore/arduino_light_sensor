# Purpose
Sense light using Arduino.

# References
Adafruit TSL2561 Luminosity Sensor
http://learn.adafruit.com/tsl2561/overview

# Equipment
## Hardware
Arduino Duemilanove w/ ATmega328 (Duemilanove="2009")

TSL2561 digital luminosity / lux / light sensor
Adafruit ID: 439

## Software libraries
### Adafruit_Sensor
https://github.com/adafruit/Adafruit_Sensor
Put in Arduino/libraries/Adafruit_Sensor

### Adafruit_TSL2561
https://github.com/adafruit/Adafruit_TSL2561
Put in Arduino/libraries/Adafruit_TSL2561  

# Results
Copied file Adafruit_TSL2561/examples/sensorapi.pde  
Opened in Arduino then closed, Arduino changed file extension from .pde to .ino  
Renamed to arduino_light_sensor.ino  

## Hardware Connect
The luminosity sensor TSL2561 runs at 3.3 V.
### CONNECTING A SECOND DEVICE TO THE I2C BUS RUNNING AT 5V COULD DAMAGE THE 3V DEVICE.

"As long as all the sensors/device on the i2c bus are running on 3.3V power, we're fine.
However, don't use a 5.0v powered i2c device (like the DS1307) with pullups at the same time as a 3.3V device like the TSL2561"
http://learn.adafruit.com/tsl2561/wiring

| Sensor | Arduino Duemilanove Pin | Arduino Leonardo Pin | Arduino Due Pin  |
| ------ | ----------------------- | -------------------- | ---------------- |
| VCC    | 3.3V                    | 3.3V                 | 3.3V             |
| GND    | GND                     | GND                  | GND              |
| SDA    | A4                      | D2                   | D20 or SDA1      |
| SCL    | A5                      | D3                   | D21 or SCL1      |

http://arduino.cc/en/Reference/Wire
