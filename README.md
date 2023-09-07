# ha-gasmeter
YAML Configuration for ESPHome with ESP8266 to "smartly" detect your gas consumption for usual gas meters

Prerequisites:
In my case I used a "d1_mini" board, available on Amazon: https://a.co/d/j6HqnNJ based on esp8266.
It would also be possible to be done with an ESP32, you would just have to adapt the corresponding section in the .yaml-File

The most important part you need is a pulse counter, which detects magnetic impulses, since most of the standard gas meters generate such impulses once a certain amount of gas has been consumed (in my case 0,01 cubic meters).
Often the manufacturer of your gas meter offers such a pulse counter directly.

In my case I use a Honeywell (Elster) gas meter.
