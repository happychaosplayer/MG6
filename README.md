# MG6
## Devlog Prompt
1. I think the entire for loop will complete before the Update() method finishes because of c# syntax in which every loop nested inside of the Update() method will have to finish before Update() can be called once per frame. It is also void and has no parameters so the Update() method changing the loops to run once per frame would be impossible.
2. With our logic, if the character's y velocity is positive (moving upwards) then our collider turns off, meaning we can do things like go through the roof and never be able to come back down. Our logic allows this because we set our collider off under certain conditions meaning EVERYTHING is passable, including the ceiling which has the ground tag in my case.
