![](static/FBD2.png)

## **Feedback**
* Switching from using two UARTS for communication with each person and connection with MQTT server to using one single UART to make the communication work without complicating the code or process.
* Adding more switches for possible debugging tools for LED's, used to have one single push button and one LED, expecting to not use more than two LEDs and no more than three switches.
* Reccomended setup with daisy chain changed to meet requirements such as using channel 2 for board to board communication and using pin eight for GND and pin one for Power (VIN).
* Changing Power input from 9V to 5V with new power source.

## **Decision Making Process**
* I had developed these improvements based on the feedback I was given and with the newer solutions giving me some breathing room by removing some additional steps that weren't needed when I was working with the double UART system. When I removed the second UART, I was able to program it much easier since I would only need one to handle both communication with other boards along with communicating those messages across the MQTT. The other change that I made was adding more debugging tools to help with the debugging program by adding more lights and push buttons to allow for more versatility with testing messages being sent or telling how and if a message was received or passed.
