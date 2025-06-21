title: A320 EFIS + FCU
author: Harry Liu
description: A complete Electronic Flight Instrument System and Flight Control Unit panel for MSFS flight simulation, based off the A320
created_at: 2025-06-13

2025-06-15:

I had no idea what to do. Apparently the Arduino Leonardo board I had was not supported by Mobiflight. My idea rn is to:

1. Watch tutorials (youtube, mobiflight documentation) and other references
2. Decide on what type of connection (PCB for structure only / soldering board thing / fully PCB)
3. Experiment with existing resources (buttons) and try to connect that to Mobiflight
4. Design a PCB, referencing existing models

I dont want to mess it up and then have it not work once I ordered.

2025-06-16:

Today I downloaded Mobiflight and started referencing a button tutorial. I don't really know what to do so I'll watch some tutorials.

Time skip, its 9PM now, I think Im beginning to learn about kicad. So far chatgpt's a great helper helping my decide on what parts to use. Im just trying to find specific symbols for them. I found this really great library but some symbols weren't included. 

10 PM: I cant find the TM 1637 4 digit display thing so I just used a generic 4 digit input. I currently figured out that I need to wire the ground and the 5V thing to all the displays.

2025-06-20:

Today I continued drawing the schematic, linking up all of the 4 / 6 digit displays. I also bought a board with atmega2560 which is compatiable. However, I bought a cheap version with a processor called CH340 that needed a driver. I was able to download the driver easily but spent a long time trying to get mobiflight and the arduino IDE to recognise the board. Turns out, I used the wrong cable. It worked once I switched my cable to a cooler-looking one.

