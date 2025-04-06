# Heating Control for BT Thermostats

## How it works

Heating blueprint for BT Thermostats with Schedule or Timer Event. Scheduler/Timer can be added in the helpers section in your home assistant settings.

## Basic function

* current date must be in between *month from* and *month to*. Year is ignored.
* runs only if someone is at home, uses *Person at home*
* switch HVAC_Mode to *heat* and Temperature to *Set Temperature value* when schedule begins and reset to *Reset Temperatur value* when schedule ends.
* can use Boost Mode with Timer

## History

## Version 0.15.0

* change from date "from" "to" to month selector

## Version 0.14.0

* fix lower, normal, upper written zone name

### Version 0.13.0

* try to fix checking on states zone name, which now checks against lower string

### Version 0.12.0

* add trigger every 5 minutes

### Version 0.11.0

* add zone to control

### Version 0.10.3

* fixing not closing thermostat if sensor temp is above target temp. Set temp tp 5°

### Version 0.10.2

* add temperature set and delay for off if sensor temp is above set thermostat temp

### Version 0.10.1

turn off thermostat if temperature is over temp_after

### Version 0.10.0

readd check on sensor temprature to switch off thermostat if overheating

### Version 0.9.0

integrate boost timer into this blueprint
add trigger for persons

### Version 0.8.0

change from target temp to set temp on control temperature to disable/enable thermostat
remove time trigger at 10pm

### Version 0.7.1

fix between month

### Version 0.7.0

add ignore on boost, to enable boost (timer) function

### Version 0.6.0

add a control temperature sensor to disable thermostat if temp is higher than target temp. Reset after schedule.

### Version 0.5.1

define (set to 10pm) trigger to reset temperature

### Version 0.5

add a time trigger to force reset temperature of thermostat

### Version 0.4.2

add some notes and descriptions, for easy understanding

### Version 0.4.1

ease the notes

### Version 0.4

add date from and date to for heating period

### Version 0.3

add device_tracker, only heat if someone is at home

### Version 0.2

reset temperature after heating

### Version 0.1

initial Version
