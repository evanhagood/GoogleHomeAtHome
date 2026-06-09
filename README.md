# GoogleHomeAtHome
A SpringBoot gateway to Home Assistant to control smart home devices in my own home.


A basic overview of the system:

### Remote
- To come as a future embedded project; probably an ESP32 with buttons attached that talk to the Gateway.

### Spring Boot Gateway (this application)
- Handles telemetry between devices, health checks, online checks, and stores device metadata, room locations, and sets up scenes for custom control of smart home devices.

### Manufacturer's API or Matter (depending on what the smart devices support)
- there are a lot of open source (or not) options that do the talking to vendor's API endpoints for you. If you happen to have bulbs or devices that support use without the vendor's cloud services, then setting up your own matter instance is the way to go. If that's not the case, you're locked into using the 3rd party API.

### The lights turn on and off!
- Currently I'm only looking to implement adjust color, temperature, and brightness of my lamps.



## What I might get to in the future
- Adding support for more than just my brand-specific lightbulbs
- Adding support for control when I'm not at home (rent a server?)