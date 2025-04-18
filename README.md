# What is this?
This is a fix for some fake dallas temperature sensors to make them work better with esphome.

# What is different?
Now the component waits twice as long for the temperature sensor to convert the temperature to a digital value and forces the scratchpad checksum to be valid.

# How to use?
Add this before your code:

    external_components:
      - source:
          type: git
          url: https://github.com/kovabait12/esphome-dallas
          ref: main
        components: [dallas_temp]

And you don't need to change the rest of your code since the component name is the same.

# How to "uninstall"

Just remove the lines mentioned before and that's it.

