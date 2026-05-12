---
title: "Progressing Research: Bugs and Mistakes"
date: 2026-05-12
---

Recently I've made some progress on developing a new IR communication board [SwarmB3](https://github.com/paulodowd/SwarmB3) for my research interests in swarm robotics.  It is quite an interesting journey, solving bugs and mistakes from electronics upwards into software.  Because of the variety of my work commitments, I currently feel like I am speed-running a full cycle of prototyping to research outcomes, targeting eventual publication. 

The below photo shows some hardware hacks to try and get things working.  The board on the left is a new board I am designing for teaching in the new academic year. For this board, I discovered that 3 of the GPIO weren't physically connected as intended to the sensors.  I discovered this the hard way, where attempting to read my sensors in software was returning values that didn't change.  When I reviewed my electronic schematic in KiCad, I found a small box indicator rather than a dot indicator, meaning that the electronic connection was not made.  Even though the fix was a few mouse-clicks, I had to wait for another round of PCB production, shipping and delivery.  However, I also discovered that one of the GPIO I wanted to use does not work if the WiFi module is enabled - so my first mistake (not having GPIO connected) became useful in allowing me to test other GPIO to read the sensors.  

![image](https://github.com/paulodowd/paulodowd.github.io/blob/main/assets/imgs/120526/SwarmB3_HardwareBugs.jpg)

On the right is an earlier version of my new communication board.   

I'm finding that with the new AI platforms I am able to make progress much quicker than before.  I am able to share my thoughts, reflections and reasoning with AI at any time - such as when I am waiting for a train.  It is very much like having a collaborator always to hand to help me structure my thoughts.  

I have been surprised by the good quality of the AI responses for electronics questions. I have found that asking AI to render schematics frequently generates obviously incorrect results.  This makes me think of the concept of an unreliable narrator in fiction.  

I've got to the stage where I am now taking measurements of the communication board in application.  When I produce the plots I have been able to observe some unexpected outcomes and I have to ask myself if this is something inherent, or whether it is emerging from my hardware or software design.



```

