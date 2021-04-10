# WiperModule
Simple relay board to control automotive wiper motor from digital outputs

This board was created when I needed a way to control a MK2 VW wiper motor using outputs from my PDM.

Many PDMs require either external relays to drive wiper motors or use specific outputs designed to handle the wiper motor braking functionality.

Rather than include this specific feature on the PDM, I opted to create a simple relay board that can be placed inbetween the PDM and the wiper motor.

This setup also allows me to use 1 high current output to drive the motor at low speed or high speed, and one low current output to control that speed.

Wires are connected to the board using Deutsch DT 4 pin connectors 

# Wiring

 Pin | Function
 ----| --------- 
 1   | Fast Input
 2   | Ground
 3   | Park Switch
 4   | Slow Input

# Connection Table
Slow Input Level | Fast Input Level | Slow Output Connection | Fast Output Connection
---------- | ---------- | ----------- | -----------
L | L | Ground | Not Connected
H | L | Slow Input | Not Connected
L | H | Ground | Not Connected
H | H | Not Connected | Slow Input

# Renderings
 ![Top](/Renders/WiperModuleTop.jpg)

 ![Bottom](/Renders/WiperModuleBottom.jpg)