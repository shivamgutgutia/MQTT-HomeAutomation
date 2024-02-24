
# Home Automation Simulation using MQTT


The simulation demonstrates how you can control home appliances from your phone using a simple protocol called MQTT. It's like using your phone as a remote control for things like lights or thermostats. Moreover, you can make it even better by adding sensors. These sensors can automatically trigger actions, like turning off lights when nobody's in the room or adjusting the temperature based on the weather outside. It's a way to make your home smarter and more convenient using technology.


## Run Locally

* Download Cisco Packet tracer here

* Clone the repository

```bash
  git clone https://github.com/shivamgutgutia/mqttHomeAutomation.git
```

* Open the pkt file

* Wait for 30 seconds for all the devices and connections to turn on

* Use the admin mobile to control all the devices over the home network


## Documentation

* Terms:
    * Rooms - ROOM1 , ROOM2 , ROOM3, HOME
    * Devices - LAMP (LAMP1, LAMP2) , FAN, AC, HUMIDIFIER, COFFEE, ALL
    * Messages - on, off

* Each room is subscribed to it's specific topic (ROOM1, ROOM2 and KITCHEN) and a common topic HOME

* Devices can be controlled by sending one of the Messages (on or off) to any room 

* Topics follow the format - <Room type>/<Device Type>

* Example:
    * Example 1 
        * Topic: ROOM1/LAMP1
        * Message: on 
        * Turns the lamp1 in the first room on

    * Example 2
        * Topic: HOME/ALL
        * Message: off
        * Turns all devices in the house off

## Authors

- [@shivamgutgutia](https://www.github.com/shivamgutgutia)
- [@suvosibanerjee](https://www.github.com/suvosibanerjee)

