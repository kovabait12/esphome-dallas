# What is this?
This is a fix for some fake dallas temperature sensors for esphome.

# What is different?
Now the component waits twice as long for the temperature sensor to convert the temperature to a digital value and forces the scratchpad checksum to be valid.

# How to use?
Add this before your code:

'''code
external_components:
  - source: github://kovabait12/esphome-dallas
    components: dallas-temp
'''
