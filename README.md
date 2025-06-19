# ESP32-SumpPump_Integration-for-HA
Existing Sump Pump and backup Integration

My equipment

Pro-Series https://www.stopflooding.com/
PS-C50 Combination Pump

Goals:

- To not spend $100 on wifi add-on unit
- Monitor:
    - Voltage, Current, Power
    - 12 Marine Battery voltage
    - when main pump starts and stops
    - ALARM Condition
- Poss add a water sensor

- Home Assistant interfacing with ESPHome addon
    - All monitoring above
    - Interesting data (to me)
    - Battery health
    - low voltage
    - Estimated time left on battery
    - HA app, mobile txt, and e-mail notification (Alarms, % battery life, low battery voltage, etc.)
      - gallons of water per hour
      - battery discharge rate


I "think" at this moment I can only connet to the controller and get a signal of an, ANY alarm.

The system is self testing and monitors battery but all the sensors only alert through the manufacture add-on.
So, 
    I must interface the ESP32 with external sensors.


  Possible:

  ACS712 AC/DC Current Sensor or better
  Temp Sensor
  ESP32-C6 (w/wo additional ethernet jack)
  Small Battery backup (not sure if siphoning off the 12V batt stepped down to 5V (ESP32 direct wire) or a very small UPS for the 5V power adapter (USB-C to ESP32) 
