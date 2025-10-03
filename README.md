# HomeAssistant-ESPHome-configs
Collection of my ESPHome configurations that I use in HomeAssistant


for all: 
- Making use of Home Assistant / ESPHome
- seeed Grove modules
- esp-idf framework
- Stock hardware
- Soldered headers on esp-32 devices
- Grove 4 pin Female Jumper to Grove 4 pin Conversion Cable: https://www.seeedstudio.com/Grove-4-pin-Female-Jumper-to-Grove-4-pin-Conversion-Cable-5-PCs-per-PAck.html
- optional Grove Green/Yellow/x Wrapper: https://wiki.seeedstudio.com/Grove-Wrapper/
- optional battery power (requires soldering & battery & resistors) / deep-sleep for battery powered applications

air-quality-sensor.yaml
- Air Quality:
  - VOC Index
  - NOx Index
- seeed_xiao_esp32s3: https://wiki.seeedstudio.com/xiao_esp32s3_getting_started/
- seeed SGP41: https://wiki.seeedstudio.com/grove-smart-air-quality-sensor-sgp41/
- 3v3, gnd, D4, D5

gas-sensor.yaml
- Air Quality:
  - Temperature
  - Air Pressure
  - Humidity
  - IAQ (indoor air quality)
  - CO2 Equivalent
  - Breath VOC Equivalent
- seeed_xiao_esp32c6: https://wiki.seeedstudio.com/xiao_esp32c6_getting_started/
- seeed BME680: https://wiki.seeedstudio.com/Grove-Temperature_Humidity_Pressure_Gas_Sensor_BME680/
- 3v3, gnd, D4, D5
- bme68x_bsec2_i2c setup (bme680 setup is also an option)

grove-segment-lcd.yaml
- Display 16x2:
  - lambda it.printf()
- seeed_xiao_esp32c6: https://wiki.seeedstudio.com/xiao_esp32c6_getting_started/
- seeed Grove-16x2 LCD:https://wiki.seeedstudio.com/Grove-16x2_LCD_Series/
- 3v3, gnd, D4, D5
- Uses sensor input from gas-sensor.yaml
- Uses this library: https://github.com/AlekEagle/esphome-lcd_grove_rgb
- todo: map special characters like the degree symbol (°)

temp-sensor.yaml
- Temperature sensor:
  - Temperature
  - Humidity
- seeed_xiao_esp32s3: https://wiki.seeedstudio.com/xiao_esp32s3_getting_started/
- seeed AHT20 Temp sensor: https://wiki.seeedstudio.com/Grove-AHT20-I2C-Industrial-Grade-Temperature&Humidity-Sensor/
- 3v3, gnd, D4, D5

TBD-1:
- Motor control
  - motor 1 speed
  - motor 2 speed
  - status?  
- seeed_xiao_esp32c6: https://wiki.seeedstudio.com/xiao_esp32c6_getting_started/
- seeed Mini I2C Motor Driver: https://wiki.seeedstudio.com/Grove-Mini_I2C_Motor_Driver_v1.0/
- 3v3, gnd, D4, D5
- Uses this library:
  - https://github.com/Seeed-Studio/Drv8830_Motor_Driver
  - alternative lib: https://github.com/adafruit/Adafruit_DRV8830

TBD-2:
- LED strip
  - Color
  - Brightness?  
- seeed_xiao_esp32c6: https://wiki.seeedstudio.com/xiao_esp32c6_getting_started/
- seeed WS2813 RGB LED Strip Waterproof 60 led//meter: https://www.seeedstudio.com/Grove-WS2813-RGB-LED-Strip-Waterproof-60-LED-m-1m.html
- 3v3, gnd, D4, D5 ???
- cabling??
- Uses this component:
  - https://esphome.io/components/light/neopixelbus/
