# EMDRbuzzers
An open-source project for creating vibrating paddles for bilateral stimulation in the Eye Movement Desensitization and Reprocessing (EMDR) protocol.

DISCLAIMER: EMDR is a specialized procedure that should not be attempted by anyone not trained in the method by an EMDRIA-approved organization. It is also not considered ethical to use such a technique on yourself.

As electronic EMDR equipment can be both enormously useful and enormously expensive (with simple vibration BLS equipment costing upwards of 50-100 USD), I wanted to create an open-source alternative. My main goal in this exercise was to provide options to customize the project according to the maker's level of electronics knowledge and their own needs for the equipment. 

<h1>Design Options</h1>
This project will cover two potential options for creating this device, corresponding to three levels of skill.

- Simpler: Order the PCB and parts separately in order to save on manufacturing costs. Use a 3d printer (either your own or one from a local maker space or library) to create the enclosure.
- Involved: Flash a ATTiny-85 microcontroller to further reduce costs (compared to purchasing a full Arduino Nano) and reduce the size footprint of the finished device.

I'll be honest with you. If you want a single set of emdr tappers with all the bells and whistles, just buy one. The overall cost for a single unit may even rival a professional model online when you add in shipping costs.

However, the benefit of all of three options is that they are usually produced in bulk. While you may pay the manufacturer around 50 USD (including shipping), that is usually for multiple assembled boards (often around 5 of them). This brings the cost per unit down signifcantly if you are in need of multiple devices. This would become more cost effective if you have a group practice of EMDR clinicians or if you want to mail a client a set of buzzers for use over telehealth. Never hurts to have backups, too. All for the price of one or two cheap tapper sets online.

In the simpler option, you can order a set of the printed circuit boards (PCBs) for relatively cheap (around 20 USD for 5 PCBs after shipping). Then you can find the parts (often from the same website to save on shipping, unless you'd like to hunt for a bargain elsewhere) and assemble it yourself. It will be easier to solder a PCB than to handwire it yourself, so you can reap the cost benefits without too much extra effort. These savings are even better if you have access to a 3D printer, which are becoming increasingly more accessible if you're able to poke around local resources like libraries, maker spaces, and universities.

If you really want to cut costs, though, we're going to need to stop buying an arduino board for every buzzer. We don't need many I/O pins and the program is small, so we can get away with using a simple microcontroller without all the bells and whistles. This will require us to flash the firmware onto an ATTiny-85, but this can be done relatively simply if you have a single Arduino and a breadboard. These ATTiny-85's cost around 1.50 USD each, bringing costs down. See the cost breakdown below.

<h1>Parts and Tools</h1>

For either of these, you will need:
- A soldering iron
- Solder
- Screwdriver

**Involved (5 units)**
| Equipment | Quantity | Approx. Cost | Example Link |
| --------- | -------- | ------------ | ------------ |
| PCBs + Shipping | 5 | $20 | https://jlcpcb.com |
| Arduino Nano | 5 | $18 | https://a.co/d/fy4D3Uy |
| 9V Battery Connector | 5 | $5.15 | https://a.co/d/67JnN00 |
| 200ohm Resistors | 10 | $1.00 | https://www.digikey.com/short/vbt50w0v |
| Red LEDs | 10 | $1.60 | https://www.digikey.com/short/cvtcr9rd |
| Vibration Motors | 12 | $14.00 | https://a.co/d/hR1sUoz |

Total: $59.75 -> 11.95/unit

**Expert (5 units)**
| Equipment | Quantity | Approx. Cost | Example Link |
| --------- | -------- | ------------ | ------------ |
| PCBs + Shipping | 5 | $20 | https://jlcpcb.com |
| ATTiny-85-20SF | 5 | $7.50 | https://mou.sr/4hANUs1 |
| 2xAAA Battery Holders | 5 | $5.15 | https://mou.sr/4ivnF7D |
| 200ohm Resistors | 10 | $1.00 | https://www.digikey.com/short/vbt50w0v |
| Red LEDs | 10 | $1.60 | https://www.digikey.com/short/cvtcr9rd |
| Vibration Motors | 12 | $14.00 | https://a.co/d/hR1sUoz |

Total: $49.25-> 9.85/unit
