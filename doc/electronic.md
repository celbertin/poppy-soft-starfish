# About the electronic


A small bit of electronic hacking is required for now. The cables between motors have two purposes:
- distribute alimentation to each motor
- convey messages to each motor (ordering them to move or asking them for sensors' values)


First, you will need a hub for connecting all arms together on the same communication and power bus.

![Hub](img/electronic/hub_xl_cable.jpg)


Then you need to power the Xl320 motors with 7.5V. Thus the alimentation should be added between the USB2Dynamixel (that deals with communication aspects) and the motors. To this end simply create the following hack.

![Power Board](img/electronic/power-board-xl320.png)

Then connect the USB2Dynamixel on one end and the first motor on the other end. Connect the USB2Dynamixel to your computer or Raspberry Pi. And power the board with 7.5V.

The communication with the motor is TTL, thus configure the USB2Dynamixel in TTL mode as shown below.

![USB2Dynamixel](img/electronic/usb2dynamixel.jpg)
