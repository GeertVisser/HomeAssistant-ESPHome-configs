# HomeAssistant-ESPHome-configs
Collection of my ESPHome configurations that I use in HomeAssistant


for all: 
- Latest Home Assistant / ESPHome
- esp-idf framework
- Stock hardware
- Soldered headers on esp-32 devices
- Grove 4 pin Female Jumper to Grove 4 pin Conversion Cable: https://www.seeedstudio.com/Grove-4-pin-Female-Jumper-to-Grove-4-pin-Conversion-Cable-5-PCs-per-PAck.html
- optional Grove Green/Yellow/x Wrapper: https://wiki.seeedstudio.com/Grove-Wrapper/
- optional battery power (requires soldering & battery & resistors) / deep-sleep for battery powered applications
  
air-quality-sensor.yaml
- seeed_xiao_esp32s3: https://wiki.seeedstudio.com/xiao_esp32s3_getting_started/
- seeed SGP41: https://wiki.seeedstudio.com/grove-smart-air-quality-sensor-sgp41/
- 3v3, gnd, D4, D5

gas-sensor.yaml
- seeed_xiao_esp32c6: https://wiki.seeedstudio.com/xiao_esp32c6_getting_started/
- seeed BME680: [https://wiki.seeedstudio.com/grove-smart-air-quality-sensor-sgp41/](https://wiki.seeedstudio.com/Grove-Temperature_Humidity_Pressure_Gas_Sensor_BME680/)
- 3v3, gnd, D4, D5
- bme68x_bsec2_i2c setup (bme680 setup is also an option)

grove-segment-lcd.yaml
- seeed_xiao_esp32c6: https://wiki.seeedstudio.com/xiao_esp32c6_getting_started/
- Grove-16x2 LCD: [https://wiki.seeedstudio.com/grove-smart-air-quality-sensor-sgp41/](https://wiki.seeedstudio.com/Grove-16x2_LCD_Series/)
- 3v3, gnd, D4, D5
- Uses this library: https://github.com/AlekEagle/esphome-lcd_grove_rgb

temp-sensor.yaml
- seeed_xiao_esp32s3: https://wiki.seeedstudio.com/xiao_esp32s3_getting_started/
- AHT20 Temp sensor: [[https://wiki.seeedstudio.com/grove-smart-air-quality-sensor-sgp41/](https://wiki.seeedstudio.com/Grove-16x2_LCD_Series/)](https://wiki.seeedstudio.com/Grove-AHT20-I2C-Industrial-Grade-Temperature&Humidity-Sensor/)
- 3v3, gnd, D4, D5
