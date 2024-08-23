---
layout: page
title: Semi-automatic watering system
description: A esp32 powered remote moisture level sensing and watering system
img: /assets/img/hobby/esp32_watering/pw9.jpg
importance: 1
category: fun
---

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/hobby/esp32_watering/section_view.png" title="CAD model of design" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     CAD model section view of controller design
</div>


section_view.png

The plants watering setup uses an esp32 microcontroller board which is connected to a 8 channel relay board. The relays switch on 5V water pumps via buttons on a smartphone app.  Soil moisture sensors are also connected to the plants that measure the soil moisture at regular intervals and show it as a percentage on the app. A temperature and humidity sensor namely he DHT11 is also installed to collect weather data. The ESP32 is connected to the home wifi and also added to the software **Home Asisstant** which is installed on a raspberry pi central hub. The raspberry pi acts like a central hub and the esp32 as a node.

The reason I built this was becaue I found it really cumbersome begging my neighbour to water my plants, every time I was away from home for over a month. So i decided to build one with really cheap with off the shelf components. I didn't want a system that would water my plants completely automatically, I actually wanted to water them myself depending on which plant actually needed it. Depending on the soil moisture readings, I pressed a button on the app and this switched on the pumps for a set duration of time and so I had full control and also enjoyed watering my plants, as I was in another country.

I designed the enclosure and electronics mounts in Onshape. The esp32 casing was designed to be 3d printed, since it had to be a little complex. The rest of the enclosure was designed to be laser cut. I cut out the casing out of balsa wood and then spray painted it so it had some form of water resistance. Connectors were attached on one side to attach the 3 wire capacitive soil moisture sensors and the other side had the female connectors for the 5V pumps.

TailVPN was used to connect to my home internet when I was outside my home WiFi. This allowed med to water my plants when I was on vacation for 2 months.

The esphome code for the project is below. I have covered some keys and passwords.

{% raw %}
```C++
ESP32 Home code

esphome:
  name: esphome-web-######
  friendly_name: MyPlants
  on_boot:
  - switch.turn_off: relay_1
  - switch.turn_off: relay_2
  - switch.turn_off: relay_3
  - switch.turn_off: relay_4

esp32:
  board: esp32dev
  framework:
    type: arduino

# Enable logging
logger:

# Enable Home Assistant API
api:
  encryption:
    key: "#####" //covered

ota:


wifi:
  ssid: !secret wifi_ssid
  password: !secret wifi_password

  # Enable fallback hotspot (captive portal) in case wifi connection fails
  ap:
    ssid: "Esphome-Web-#####" //covered
    password: "#####" //covered

captive_portal:

output:
  - platform: gpio
    pin: GPIO2
    id: builtin_led
    inverted: False

interval:
  - interval: 1s
    then:
      if:
        condition:
          wifi.connected:
        then:
          - output.turn_on: builtin_led
        else:
          - output.turn_off: builtin_led

  - interval: 15s
    then:
    - if:
        condition:
          wifi.connected:
        then:
        else:
          - switch.turn_off: relay_1
          - switch.turn_off: relay_2
          - switch.turn_off: relay_3
          - switch.turn_off: relay_4
  

sensor:
  - platform: adc
    pin: A0
    attenuation: auto
    id: "adcRaw_Sensor_Data_BOT"
    accuracy_decimals: 2
    name: "Sensor_Voltage_BOT"
    update_interval: 3600s
  - platform: adc
    pin: A0
    attenuation: auto
    id: "adcMoisture_BOT"
    accuracy_decimals: 1
    unit_of_measurement: '%'
    filters:
      - calibrate_linear:
        - 2.456 -> 0
        - 0.970  -> 100.0  
    name: "Moisture_Big_Olive_Tree"
    icon: mdi:water-percent
    update_interval: 3600s
  - platform: wifi_signal
    name: "Plant_WiFi_Signal_Sensor"
    update_interval: 60s

  - platform: adc
    pin: A3
    attenuation: auto
    id: "adcRaw_Sensor_Data_SOT"
    accuracy_decimals: 2
    name: "Sensor_Voltage_SOT"
    update_interval: 3600s
  - platform: adc
    pin: A3
    attenuation: auto
    id: "adcMoisture_SOT"
    accuracy_decimals: 1
    unit_of_measurement: '%'
    filters:
      - calibrate_linear:
        - 2.456 -> 0
        - 0.970  -> 100.0  
    name: "Moisture_Small_Olive_Tree"
    icon: mdi:water-percent
    update_interval: 3600s

  - platform: adc
    pin: A6
    attenuation: auto
    id: "adcRaw_Sensor_Data_FB1"
    accuracy_decimals: 2
    name: "Sensor_Voltage_FB1"
    update_interval: 3600s
  - platform: adc
    pin: A6
    attenuation: auto
    id: "adcMoisture_FB1"
    accuracy_decimals: 1
    unit_of_measurement: '%'
    filters:
      - calibrate_linear:
        - 2.456 -> 0
        - 0.970  -> 100.0  
    name: "Moisture_Flowerbed_1"
    icon: mdi:water-percent
    update_interval: 3600s

  - platform: adc
    pin: A7
    attenuation: auto
    id: "adcRaw_Sensor_Data_FB2"
    accuracy_decimals: 2
    name: "Sensor_Voltage_FB2"
    update_interval: 3600s
  - platform: adc
    pin: A7
    attenuation: auto
    id: "adcMoisture_FB2"
    accuracy_decimals: 1
    unit_of_measurement: '%'
    filters:
      - calibrate_linear:
        - 2.456 -> 0
        - 0.970  -> 100.0  
    name: "Moisture_Flowerbed_2"
    icon: mdi:water-percent
    update_interval: 3600s
	
	- platform: dht
		pin: D2
		temperature:
			name: "Living Room Temperature"
		humidity:
			name: "Living Room Humidity"
		update_interval: 60s

switch:
  - platform: gpio
    name: "Water_BOT"
    id: relay_1
    pin: 19
    icon: mdi:watering-can
    inverted: true

  - platform: gpio
    name: "Water_SOT"
    id: relay_2
    pin: 18
    icon: mdi:watering-can
    inverted: true

  - platform: gpio
    name: "Water_FB1"
    id: relay_3
    pin: 5
    icon: mdi:watering-can
    inverted: true

  - platform: gpio
    name: "Water_FB2"
    id: relay_4
    pin: 17
    icon: mdi:watering-can
    inverted: true
```
{% endraw %}
