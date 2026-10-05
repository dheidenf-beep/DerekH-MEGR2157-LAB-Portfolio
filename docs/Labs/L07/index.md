# A7 – Linkage Mechanisms

## Objective

The objective of the seventh lab was to design and 3D print a working linkage that performs a distinct motion or task. 


## Research

### _Linkage 1_



### _Linkage 2_

## Print-in-Place Connection

For the linkage, I did not want to use any non-3D printed parts. And so there was no assembly needed, I wanted it to be printed in place. This meant I needed to do research to figure out how moving 3D printed parts are printed in place. I looked at various print in place files on 3D print websites such as Thingiverse and Printables. I watched videos on articulated prints and different hinge mechanisms and read about other print in place mechanisms that have been designed. I learned that a common way to print in place linkage mechanisms is to use conical connections or pins. One part has an upside-down cone attached to the body of that link and the other link has a conical hole inside of it that opposite to the upside-down conical pin. This way, the printer is able to print it since the pin is angle and since it is conical, the hole catches on the upside-down cone and is unable to fall out. This is the method I decided to use for my linkage and I started with a proof of concept to determine if I understood what I was doing and how the connection worked.

## Prototype

### Prototype CAD Modeling

Before designing the primary linkage, I wanted to create a proof of concept of a print in place linkage. I decided to create a prototype that was just one connection and two parts in total. 

For the tolerances for the gap between the cone and cone hole, I used the 0.4 mm recommended limit for 3D print in place connections listed on the assignment Canvas Page.

<img width="515" height="59" alt="StartingFDMClearences" src="https://github.com/user-attachments/assets/4bc63a2d-e065-4360-b3c5-d0af77dca1c7" />

All of the other measurements were chosen to be small but there was no math or underlying logic behind it. 
For the thickness, I chose 10 mm. Technically, the thickness I set was 5 mm, but I had a plan as to why it was half. The length I chose was 40 mm and both the base and height were 10 mm.

I began with a rectangle for the main linkage body that would have the upside-down cone.

<img width="960" height="564" alt="TestLinkage (2)" src="https://github.com/user-attachments/assets/dcae8a9d-16ea-4ba5-99f3-487709777acd" />

I started this sketch on the right plane. I new I needed to sketch the cylinder in the center width wise of the linkage, so I wanted the right hand plane as my reference. This meant I needed the right hand plane intersecting the center of my rectangular prism. To do this, I extruded the sketch to be 5 mm thick on both sides of the plane, giving the total thickness of 10 mm.

<img width="960" height="564" alt="TestLinkage (3)" src="https://github.com/user-attachments/assets/6fe8b8b4-acbb-4422-926d-eaef4dc53ca1" />

<img width="960" height="564" alt="TestLinkage (4)" src="https://github.com/user-attachments/assets/bdf2dc33-64d4-4a0b-8f8f-21b647c432d8" />

After the rectangular prism was extruded, I could then sketch the upside-down cylinder using the right plane as the reference. 

<img width="960" height="564" alt="TestLinkage (6)" src="https://github.com/user-attachments/assets/3fe82039-9ee5-4629-ab82-ad3e17e91f92" />

<img width="960" height="564" alt="TestLinkage (8)" src="https://github.com/user-attachments/assets/a6e151fe-1070-48e6-a47a-e98b5c05eff5" />

I made the diameter of the base of the cone (technically the top) 8 mm, the bottom diameter 2 mm, and later a height of 6 mm with the center of the cone being 8 mm from the edge. I only realized later that I didn't have to sketch the whole cylinder since I needed to revolve it. But I just put in a centerline and revolved half the cone around it.

<img width="960" height="564" alt="TestLinkage (9)" src="https://github.com/user-attachments/assets/36260e7e-df13-4e37-85b6-58918becfd5e" />

<img width="960" height="564" alt="TestLinkage (10)" src="https://github.com/user-attachments/assets/da335ff7-ad50-40a6-9f22-2e0d71868392" />









### Prototype Preprocessing



### Prototype 3D Printing



## Scissor Linkage

### Scissor Linkage CAD Modeling



### Scissor Linkage Preprocessing



### Scissor Linkage 3D Printing



### Scissor Linkage Iterating



## Final Linkage



## Lessons Learned

* **Time: How many hours did the project take from start to finish? Break them down into research, CAD, slicing, printing, post-processing and assembly. How did the total compare with what you expected?**



* **Biggest mistake: What was your most significant mistake or failure? What was the root cause, how did you find it, and how did you fix it?**



* **Tolerances: Did your first-print clearances work? What would you change, and by how much?**



## References

[Seam position](https://help.prusa3d.com/article/seam-position_151069)

[Elephant foot compensation](https://help.prusa3d.com/article/elephant-foot-compensation_114487)

[Linkage Designs](https://mechanicaldesign101.com/linkage-designs/)

[How to 3D Print Interlocking Parts and Assemblies](https://formlabs.com/blog/how-to-3d-print-interlocking-joints/)

[Linkage 3D Files from Cults3D](https://cults3d.com/en/tags/linkage)

[Expanding Star](https://www.printables.com/model/1000576-expanding-star)

[Trammel of Archimedes](https://www.instructables.com/Trammel-of-Archimedes/)

* [Print In Place Scissor mechanism](https://www.reddit.com/r/3Dprinting/comments/xekbyx/print_in_place_scissor_mechanism/)

[3D Printed Scissor Lift Video](https://www.youtube.com/shorts/ZsNt6xYCAH8)

[Center Finder Tool With Cabinet Pull Marking Companion](https://www.thingiverse.com/thing:7035457)

[Preassembled scissor arm](https://www.thingiverse.com/thing:60216)

[Learn 15 Print-in-Place Mechanisms in 15 Minutes](https://www.youtube.com/watch?v=AAKsl8zW-Ds&t=2s)

[How To Make Articulated Print In Place Designs | Articulated Shark](https://www.youtube.com/watch?v=XV_pcDC14hE)
