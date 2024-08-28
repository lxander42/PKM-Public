---
created: 2024-03-16
modified: 2024-03-16
tags:
  - project-idea
---
## Problem
I have this old retro gaming TV (pictured below) but it has an antenna input, I need to figure out how to get this to HDMI, or be controlled by a Raspberry PI. 

![](../../../5INBOX/Pasted%20image%2020240316192909.png)

![](../../../5INBOX/Pasted%20image%2020240316192919.png)

Model number is E09344, I can't find any electrical schematics online. 

## Open questions
- [[../../../3RESOURCES/THOUGHTS/How do CRT TVs work]]

After some youtubing, it seems like all the answers are just contained in this guy's video: [Hooking An Old TV to HDMI Players (youtube.com)](https://www.youtube.com/watch?v=iq9scofun-s)

I basically need an HDMI->Composite->RF modulator setup.
That, or I can use the [isotope-engineering/PiMod-Zero: Raspberry Pi Zero RF Modulator Hat (github.com)](https://github.com/isotope-engineering/PiMod-Zero) to use a Raspberry pi to do RF modulation.