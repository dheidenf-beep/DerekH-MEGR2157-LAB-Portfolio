# A7 – Linkage Mechanisms

## Objective

The objective of the seventh lab was to design and 3D print a working linkage that performs a distinct motion or task. 


## New Linkage Technology Research

### Miura-Origami Inspired Linkage

The Miura-Origami inspired linkage is a linkage based off of the Miura-Origami fold. 

<img width="2917" height="1176" alt="MiuraOrigamiLinkage" src="https://github.com/user-attachments/assets/955484e8-096a-466b-a464-d859f4ea2b73" />

The Miura-Oragami inspired linkage is composed of 2 pairs of unequal length linking rods. The shape of the linkage gives it the unique property in that it only has 1 degree of freedom. Pulling or pushing on any of the vertices in the linkage automatically causes the entire linkage to fold or unfold. 

The Miura-Orgami linkage is inherently more immune to vibrations but There have been studies into applying low-frequency vibration isolators to further allow it to reduce vibrations. This means the linkage could have potential applications in high-precision engineering or other precise industries such as suspensions or applications requiring low virations.

**References**

* Image Source: [Miura-origami inspired quasi-zero stiffness low-frequency vibration isolator](https://www.sciencedirect.com/science/article/pii/S0020740325003698#sec0001)

* [A STUDY OF THE MULTI-STABILITY IN A NON-RIGID STACKED MIURA-ORIGAMI CELLULAR MECHANISM](https://par.nsf.gov/servlets/purl/10322848)

* [Stiff deployable structures via coupling of thick Miura-ori tubes along creases](https://www.sciencedirect.com/science/article/pii/S0094114X24002787)



### Transforming Coiling Planar Linkage

The Transforming Coiling Planar Linkage is a linkage mechanism designed to be able to expand into a deployable structure through a coiling motion versus a standard linear or radial expansion. The Transforming Coiling Planar Linkage uses the properties of four bar linkages in order to achieve localized angular changes. These designs are replicated to create a truss-like structure that is capable of coiling and uncoiling seamlessly with only 1 degree of freedom over the entire linkage.

<img width="1593" height="1960" alt="TransformingCoilingPlanarLinkage" src="https://github.com/user-attachments/assets/22c92ee2-1dea-43db-8995-6871d5135070" />

There are changes that can be made to the linkage to create different variations such as a linkage that is similar to an Archimedean Spiral depending on the lengths of the individual bars. 

The primary benefit of the Transforming Coiling Planar Linkage is that it can coil into a circular space and expand in a straight line. 

Some of the applications listed in the sources display its uses as a linear actuator and mechanism that could provide seating assistance. 

<img width="1579" height="1265" alt="TransformingCoilingPlanarLinkage2" src="https://github.com/user-attachments/assets/c113002b-7bc3-464a-8a7d-8bfb49187c47" />

The Transforming Coiling Planar Linkage has potential applications in a variety of fields such as manufacturing machines, robotics, and health.

**References**

* Images Source: [Kinematic analysis and experimental verification of transforming planar linkage mechanism](https://link.springer.com/article/10.1186/s40648-025-00289-3#Sec13)

* [The design of coiling and uncoiling trusses using planar linkage modules](https://www.semanticscholar.org/paper/The-design-of-coiling-and-uncoiling-trusses-using-Liu-Wang/b4d4d229bfb2ceba20731750bc09d321997dc2b8)

* [Automated synthesis of planar linkage mechanisms with diverse joint types via spring-connected link models and contrastive graph learning ](https://academic.oup.com/jcde/article/13/4/252/8554182)



## Print-in-Place Connection

For the linkage, I did not want to use any non-3D printed parts. And so there was no assembly needed, I wanted it to be printed in place. This meant I needed to do research to figure out how moving 3D printed parts are printed in place. I looked at various print in place files on 3D print websites such as Thingiverse and Printables. I watched videos on articulated prints and different hinge mechanisms and read about other print in place mechanisms that have been designed. I learned that a common way to print in place linkage mechanisms is to use conical connections or pins. One part has an upside-down cone attached to the body of that link and the other link has a conical hole inside of it that opposite to the upside-down conical pin. This way, the printer is able to print it since the pin is angle and since it is conical, the hole catches on the upside-down cone and is unable to fall out. This is the method I decided to use for my linkage and I started with a proof of concept to determine if I understood what I was doing and how the connection worked.

## Prototype

### Prototype CAD Modeling

Before designing the primary linkage, I wanted to create a proof of concept of a print in place linkage. I decided to create a prototype that was just one connection and two parts in total. 

For the tolerances for the gap between the cone and cone hole, I used the 0.4 mm recommended limit for 3D print in place connections listed on the assignment Canvas Page.

<img width="515" height="59" alt="StartingFDMClearences" src="https://github.com/user-attachments/assets/4bc63a2d-e065-4360-b3c5-d0af77dca1c7" />

All of the other measurements were chosen to be small but there was no math or underlying logic behind it. 
For the thickness, I chose 10 mm. Technically, the thickness I set was 5 mm, but I had a plan as to why it was half. The length I chose was 40 mm and both the base and height were 10 mm.

I began in Solidworks with a rectangle for the main linkage body that would have the upside-down cone.

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

Here I decreased the height of the rectangle to 5mm and set the height of the cone to 6 mm.

<img width="960" height="564" alt="TestLinkage (11)" src="https://github.com/user-attachments/assets/29d73897-f663-4f3b-af5f-339ec99c15c4" />

<img width="960" height="564" alt="TestLinkage (13)" src="https://github.com/user-attachments/assets/e867fe21-ae24-42ed-9b94-2a3d28a3fac0" />

I then began work on the hole that would surround the cone, using the right plane as a reference. I set the height and upper and lower radii to be the same as the cone. I used the 0.4 mm gap to space the hole from the cone itself and the linkage body.

<img width="960" height="564" alt="TestLinkage (14)" src="https://github.com/user-attachments/assets/224bab61-3867-4c30-92d3-20f0a54faed4" />

<img width="960" height="564" alt="TestLinkage (16)" src="https://github.com/user-attachments/assets/30ac4837-13eb-450e-a4b6-32be81e4fd43" />

Then, using a construction centerline centered on the cone, I revolved the hole around.

<img width="960" height="564" alt="TestLinkage (18)" src="https://github.com/user-attachments/assets/bce1a979-cc69-4648-9220-d9f39686611f" />

<img width="960" height="564" alt="TestLinkage (20)" src="https://github.com/user-attachments/assets/d85a5c85-6510-4310-afe4-00f27ffa673f" />

For the next linkage body attached to the hole, I needed to create a reference to sketch off of. I created a reference plane that was tangent to the outside of the hole and parallel to the end of the first linkage body.

<img width="960" height="564" alt="TestLinkage (21)" src="https://github.com/user-attachments/assets/ffddb551-1a5e-43c7-9120-8241dba615f1" />

I then created a rectangular shape with the same dimensions for the base, height, and width as the first linkage body. 

<img width="960" height="564" alt="TestLinkage (24)" src="https://github.com/user-attachments/assets/c366f692-f8fd-4900-a330-1af6021ba784" />

To extrude the sketch, I first extruded one way about half the length of the first rectangular prism. I then had to extrude the other way up to the surface of the hole to create a continuous shape.

<img width="960" height="564" alt="TestLinkage (25)" src="https://github.com/user-attachments/assets/638651ca-1c77-47b0-b758-69fd9987dff6" />

<img width="960" height="564" alt="TestLinkage (26)" src="https://github.com/user-attachments/assets/9b1eeaae-f043-4a93-a7b7-843ac6323e8a" />

<img width="960" height="564" alt="TestLinkage (28)" src="https://github.com/user-attachments/assets/95b717d4-4bfe-419e-b228-486a6394471d" />

<img width="960" height="564" alt="TestLinkage (30)" src="https://github.com/user-attachments/assets/555c3f9d-ed44-4d8f-9685-2a2f82c2e8dc" />

With the second rectangular prism extruded, I had finished the prototype and moved on to printing it.


### Prototype Preprocessing

For printing the prototype, I mainly stuck with the simplest parameters in the Prusa Slicer to see how it would perform with 0.4 mm of clearance for the moving connection. The print time was about 15 minutes.

<img width="960" height="564" alt="TestLinkage (31)" src="https://github.com/user-attachments/assets/bce3ff25-f874-4854-93bc-2da5e2bf9607" />

<img width="960" height="564" alt="TestLinkage (32)" src="https://github.com/user-attachments/assets/bd65cc06-2548-4d2a-9c4a-de220a959953" />

<img width="960" height="564" alt="TestLinkage (33)" src="https://github.com/user-attachments/assets/d661fd69-36fc-4f08-9ed9-8c7cc7ce529e" />

The only thing I changed was to add organic supports to the model since most of it was hanging off the edge.


### Prototype 3D Printing

For the 3D printing of the prototype, I used printer 3 in the Duke Centennial Print Lab using PLA filament. 

<img width="4000" height="3000" alt="PrototypePicture (4)" src="https://github.com/user-attachments/assets/5a57afbd-a532-495e-bbe3-c49fba531cb7" />

* The Print rendered on the Prusa Printer

<img width="4000" height="3000" alt="PrototypePicture (2)" src="https://github.com/user-attachments/assets/50781cdb-cb46-4066-927a-e7a14b9b3f33" />

* The Printer Starting the First Layers

<video width="100%" controls>
  <source src="PrototypePrint.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

<img width="4000" height="3000" alt="PrototypePicture (5)" src="https://github.com/user-attachments/assets/5ea7cd22-ea83-4ae9-9355-b68b684e7635" />

<img width="4000" height="3000" alt="PrototypePicture (8)" src="https://github.com/user-attachments/assets/bcf0a63a-0d07-40a3-b188-e5530df2737f" />

* The print starting in the second linkage piece

<img width="4000" height="3000" alt="PrototypePicture (13)" src="https://github.com/user-attachments/assets/891aa678-01c6-4884-a30f-ab020dbec7bd" />

* The finished print.

The print didn't have any issues that I noticed, meaning it was time to test if the prototype worked.



### Prototype Components

| Component | Linkage Section A | Linkage Section B |
|-----------|-------------------|-------------------|
| Function | Conical Pin that Section B Rotates Around | Rotates around the Pin on Section A |
| Creation | 3D Printed | 3D Printed |

### Prototype Evaluation

<img width="4000" height="3000" alt="PrototypePicture (14)" src="https://github.com/user-attachments/assets/394758fd-9eaa-4866-841c-fffd5c1ac651" />

Once the print of the prototype was finished, I took off the supports and tested it. I was worried that since there were few supports on the second upper piece, that it might've adhered to the bottom part. But that seemingly didn't happen and the prototype worked exactly as I was hoping. The Two parts of the linkage were free to move about the conical pin connection.

<img width="4000" height="3000" alt="PrototypePicture (15)" src="https://github.com/user-attachments/assets/8ffdb585-a9f7-48ee-8b3d-79bf14224708" />

<video width="100%" controls>
  <source src="PrototypeEvaluate.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

This meant my proof of concept worked and I just needed to scale it up to a bigger linkage.


## Scissor Linkage

For my actual linkage, I decided to print a basic scissor linkage. A scissor linkage being a series of crossing links that are attached together and expand and contract upwards or downwards depending on whether the links at the bottom are moved left or right. They are very useful for allowing a lot of vertical expansion while being able to fold down into a compact space. 

The reason I designed a scissor linkage came from my time on my robotics team in high school. For the robot to complete it's tasks, it often needed to be able to expand and contract both horizontally and vertically. To do this, the scissor link is often one linkage we'd look at. This gave me a lot of experience dealing with and creating scissor linkages that I decided to use here since scissor links are very simple and scalable, which was good because I wanted something small and simple to design and print. For the scissor lift design, I went with a part that had only four different pieces.

<img width="332" height="400" alt="ScissorLinkReference" src="https://github.com/user-attachments/assets/3feba3bb-7b89-4ff7-bf74-70a817ae36af" />

[Scissor Link Reference Image](https://handling.com/guide/scissor-lift-design-and-dimensions/)

### Scissor Linkage CAD Modeling

For the scissor linkage CAD model, I wanted to put in parameters for all my dimensions because everything needed to be very consistent in terms of the lengths and dimensions.

<img width="780" height="503" alt="ScissorLinkageCAD (9)" src="https://github.com/user-attachments/assets/b67cce11-8c9f-4af9-81ca-9a3343ab3edb" />

Here I set the base as 5 mm (which is half of the true thickness since I would extrude on both sides of a plane), the length as 60 mm, the height as 5 mm, and I put in the parameters for the cone such as the upper and lower radii, the clearance gap which I kept at 0.4 mm, and I made the distance the cone was from the edge of the linkage body driven by the upper (larger) radius.

From there, the modeling for the first link was the same as modeling the prototype.

<img width="960" height="564" alt="ScissorLinkageCAD (1)" src="https://github.com/user-attachments/assets/8d6e325c-c4e2-4cf0-95ac-2b6a1c173134" />

<img width="960" height="564" alt="ScissorLinkageCAD (2)" src="https://github.com/user-attachments/assets/0310c14a-1be8-4651-a6c1-4b2069bee9ce" />

<img width="960" height="564" alt="ScissorLinkageCAD (3)" src="https://github.com/user-attachments/assets/940e4050-78d0-402c-8415-9748bc1a3ee6" />

<img width="960" height="564" alt="ScissorLinkageCAD (6)" src="https://github.com/user-attachments/assets/170b1f02-eea7-4441-8b54-9b193daef1d8" />

The primary difference was that there needed to be two cones, one in the center and one near the edge. I tried looking up ways to copy features in Solidworks, but I couldn't find a good method so I created all the pegs manually.

<img width="960" height="564" alt="ScissorLinkageCAD (10)" src="https://github.com/user-attachments/assets/880bc1b2-6377-4ede-8a8e-6cc37ed0f7fa" />

<img width="960" height="564" alt="ScissorLinkageCAD (11)" src="https://github.com/user-attachments/assets/43681c1a-4595-4736-83f4-3c44fc09a891" />

<img width="960" height="564" alt="ScissorLinkageCAD (12)" src="https://github.com/user-attachments/assets/c4fc8640-1407-4663-85e4-2aecbf615293" />

<img width="960" height="564" alt="ScissorLinkageCAD (14)" src="https://github.com/user-attachments/assets/9e97ad49-1fec-4dfb-8cce-ced923ee44ef" />

I then modeled the holes around the cones to connect to the respective links.

<img width="960" height="564" alt="ScissorLinkageCAD (17)" src="https://github.com/user-attachments/assets/b49ba34d-3599-4939-9cca-6476c117b13d" />

<img width="960" height="564" alt="ScissorLinkageCAD (18)" src="https://github.com/user-attachments/assets/12f6d722-db2d-44ab-b992-b23bf1b79408" />

<img width="960" height="564" alt="ScissorLinkageCAD (19)" src="https://github.com/user-attachments/assets/2053571e-3787-43dc-8845-8b0ac2e1a2f0" />

Once I had the first Hole in, I decided to try figuring out How to make the rest of the rectangular prism the hole is in the center of. 
This took a lot of tinkering of using planes and trying to figure out the diameter. The problem I was running into was if I just used a plane tangent to the edge of the hole and extruded out the length, I needed to know how far to go so as to get half of the length on each side of the hole since the hole was in the middle of the link. 

<img width="960" height="564" alt="ScissorLinkageCAD (21)" src="https://github.com/user-attachments/assets/d7838256-1cc3-41a4-b810-36a9ab76392c" />

<img width="960" height="564" alt="ScissorLinkageCAD (26)" src="https://github.com/user-attachments/assets/d87a1867-6b8a-4e5f-830a-a3db2338fd4c" />

I tried figuring out the diameter of the hole so I could math out how far I needed to go on each end. However, due to the slopes of the cones being separated by 0.4 mm and vertically offset by 0.4 mm made the math very difficult, and I ended up being unable to figure out the total diameter. I didn't want to use an estimation from Solidworks' measuring tool either due to how precise the linkage needed to be in order to line up properly. 

My next thought was creating a plane and sketch in the middle again. 

<img width="960" height="564" alt="ScissorLinkageCAD (27)" src="https://github.com/user-attachments/assets/1d84ec58-4dfa-49e5-93cb-c811dea77dca" />

This turned out to be the solution. I was able to offset the extrusion by a set, whole number amount, while still intersecting the hole. I could then extrude the rectangle the rest of the length and I would just have to extrude the other way up to the outside surface of the hole. 

<img width="960" height="564" alt="ScissorLinkageCAD (28)" src="https://github.com/user-attachments/assets/240bb25a-e7e9-43eb-9b55-22139d7a80dd" />

This meant there were no decimals I had to worry about and everything could be parametrically driven. I just had to do it on both sides of the hole with two individual offsets.

<img width="960" height="564" alt="ScissorLinkageCAD (29)" src="https://github.com/user-attachments/assets/2c891aca-af03-435d-a5e2-b6c8ec9cf2db" />

<img width="960" height="564" alt="ScissorLinkageCAD (30)" src="https://github.com/user-attachments/assets/bceb165c-83fc-4b42-9431-68f2e0f933da" />

I could then use this method for all of the other links, which I proceeded to do. This way there was no uncertainty and everything lined up perfectly. 

I continued on with the other link, making it only half the length because I was only making the first 4 links of a scissor linkage.

<img width="960" height="564" alt="ScissorLinkageCAD (31)" src="https://github.com/user-attachments/assets/c5711caa-cfe9-4e3b-abe0-20d86c820237" />

<img width="960" height="564" alt="ScissorLinkageCAD (32)" src="https://github.com/user-attachments/assets/5a6adc6a-e6ef-4b68-9edb-fb9eabda4855" />

<img width="960" height="564" alt="ScissorLinkageCAD (33)" src="https://github.com/user-attachments/assets/e45e0fe0-9e4f-4fd3-a741-b7fc99d22772" />

Here is one of the many times I was very glad I made all of my dimensions parametric. The links felt a little close together for me so I decided to increase the length from 60 mm to 80 mm. And all I had to do was change the one global variable and everything updated automatically.

<img width="780" height="503" alt="ScissorLinkageCAD (34)" src="https://github.com/user-attachments/assets/ec1e6036-24ba-415d-ad35-7e886e447b05" />

<img width="960" height="564" alt="ScissorLinkageCAD (35)" src="https://github.com/user-attachments/assets/53c0e9af-eace-4f4a-a549-755331c9c727" />

The next links were rinse and repeat. I created a plane intersecting through the middle of the link and built the cone off of it. 

<img width="960" height="564" alt="ScissorLinkageCAD (37)" src="https://github.com/user-attachments/assets/5ceec046-152e-4ad3-836b-4e836da122cb" />

<img width="960" height="564" alt="ScissorLinkageCAD (40)" src="https://github.com/user-attachments/assets/ccb6aa66-14e9-40e6-a4f3-043704b18381" />

<img width="960" height="564" alt="ScissorLinkageCAD (41)" src="https://github.com/user-attachments/assets/eb030da2-5f09-41f7-8b8c-af898a77499e" />

<img width="960" height="564" alt="ScissorLinkageCAD (42)" src="https://github.com/user-attachments/assets/fc3fc84f-c588-40f4-9647-a915de99e178" />

Next was the part that dictated whether I made the linkage correctly or not. I needed to create 2 holes around the each cone and extrude a piece between them to connect them. However, if I did something wrong, that piece would likely not line up. I doubled checked and Solidworks gave the correct distance between the centers of the two cones and everything seemed to line up.

<img width="960" height="564" alt="ScissorLinkageCAD (43)" src="https://github.com/user-attachments/assets/5badee56-501f-43b9-8fec-5491d0893313" />

<img width="960" height="564" alt="ScissorLinkageCAD (45)" src="https://github.com/user-attachments/assets/a6dd13e5-cb3c-459e-84b1-937bb5703ffc" />

<img width="960" height="564" alt="ScissorLinkageCAD (46)" src="https://github.com/user-attachments/assets/04108454-a5c7-4b1e-b1fe-52d899bd8799" />

<img width="960" height="564" alt="ScissorLinkageCAD (50)" src="https://github.com/user-attachments/assets/2ec4c3ea-e77c-4dec-88ac-1477d2bc9576" />

I created the rectangle and extruded the sketch. And everything lined up perfectly. All of the calculations worked out.

<img width="960" height="564" alt="ScissorLinkageCAD (51)" src="https://github.com/user-attachments/assets/cdb3c77e-6a0d-4595-be3d-ddaafa876ffb" />

<img width="960" height="564" alt="ScissorLinkageCAD (52)" src="https://github.com/user-attachments/assets/8124e5b5-1394-4ca1-8e7d-9b12e8b7691b" />

<img width="960" height="564" alt="ScissorLinkageCAD (53)" src="https://github.com/user-attachments/assets/cf058ed7-3ff1-47fc-b821-85effd938b88" />

<img width="960" height="564" alt="ScissorLinkageCAD (54)" src="https://github.com/user-attachments/assets/6997adad-5cc7-41a9-b740-b8bf8d79587d" />

This meant I was finished with the CAD modeling (for now) and could move on to the preprocessing and printing of the scissor link.


### Scissor Linkage 3D Print Iterating

To get the scissor link printed game me a myriad of issues. But to start, I loaded it into the Prusa Slicer and sliced it. 

<img width="960" height="564" alt="ScissorLinkageCAD (55)" src="https://github.com/user-attachments/assets/7440f4c8-fdf6-47ef-8838-a642ebc0b420" />

I modified the parameters to use a lower Elephant's foot compensation, changing it from 0.2 mm to 0.1 mm. Since I had parts of the cones near the bottom of the print bed, I didn't want the first layer to expand and adhere to the conical pins and prevent them from spinning. I also changed the seam placement to "random" to prevent the seams from building up and potentially causing the linkage to be unable to move.

<img width="960" height="564" alt="ScissorLinkageCAD (57)" src="https://github.com/user-attachments/assets/9806d659-7fc5-4129-a4f3-a8fdc93bae0a" />

<img width="960" height="564" alt="ScissorLinkageCAD (60)" src="https://github.com/user-attachments/assets/bb878a77-dc21-46aa-85ae-103d0e41dae4" />

<img width="960" height="564" alt="ScissorLinkageCAD (56)" src="https://github.com/user-attachments/assets/b83eb276-a45a-4307-8691-0f73f262918d" />

<img width="960" height="564" alt="ScissorLinkageCAD (58)" src="https://github.com/user-attachments/assets/73d1b91d-4133-4096-91c5-1769b072c4ce" />

Here, the conical pins can be seen without any supports despite not touching the print bed. I decided to try printing it and seeing what happened. 

I printed it using printer 3 again in the Duke Centennial Print Lab.

<img width="4000" height="3000" alt="Try1Picture (1)" src="https://github.com/user-attachments/assets/887620aa-dec3-4217-b2f9-0afcacaa2c52" />

<img width="4000" height="3000" alt="Try1Picture (3)" src="https://github.com/user-attachments/assets/4a0a6d9d-f95d-48c1-8ece-197e358d0df1" />

<img width="4000" height="3000" alt="Try1Picture (7)" src="https://github.com/user-attachments/assets/a8a49cc8-d136-4615-8d73-54039696d5d1" />

The print started off fine. It printed the base of the cones seemingly fine. But it wasn't long after that the base of the cone it printed came off the print bed.

<img width="4000" height="3000" alt="Try1Picture (9)" src="https://github.com/user-attachments/assets/e5ed8255-3eb6-4d67-8993-7a1077f76dc3" />

<video width="100%" controls>
  <source src="Try1VideoFail.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

This problem persisted no matter how I sliced the linkage. The bases of the conical pins would always pop off the print bed. 

I tried painting on supports. It didn't actually create any supports.

<img width="960" height="564" alt="ScissorLinkageCAD (59)" src="https://github.com/user-attachments/assets/cd7e20d6-db6e-4eba-920d-4f5069a65d35" />

I tried adjusting the settings of the supports.

I tried lower the speeds by changing it from the "speed" preset to the "structural" preset. 

<img width="960" height="564" alt="ScissorLinkageCAD (62)" src="https://github.com/user-attachments/assets/24d47b35-9df4-4ea4-9183-4d4ddd5de8fa" />

However, nothing was working. I decided to return the CAD model and create new extrudes on those two conical pins that were 0.4 mm thick so that they would be flush with the rest of the model and be built directly on the print bed. 

<img width="960" height="564" alt="ScissorLinkageCAD (64)" src="https://github.com/user-attachments/assets/e1af1bd9-59b9-4b46-a201-a2334ae3a7e6" />

<img width="960" height="564" alt="ScissorLinkageCAD (65)" src="https://github.com/user-attachments/assets/5e235c6b-4481-4870-98c3-c864db8a2b30" />

<img width="960" height="564" alt="ScissorLinkageCAD (66)" src="https://github.com/user-attachments/assets/584bacb0-e0fd-409a-9470-589cc08a12ca" />

<img width="960" height="564" alt="ScissorLinkageCAD (67)" src="https://github.com/user-attachments/assets/6e016d45-b280-4ce1-bc7b-8dc616642d24" />

With this final version, using the same parameters as before (the same supports, elephants foot compensations, random seam positions, and structural build mode), I tried printing it again.


## Final Linkage

The final linkage print turned out well. Having the conical pins adhere to the build plate fixed the issue and the print then proceeded somoothly. The print time was about 40 minutes.

<img width="4000" height="3000" alt="Try2Picture (2)" src="https://github.com/user-attachments/assets/f5e5ee92-816d-4738-8890-2c122f155973" />

<img width="4000" height="3000" alt="Try2Picture (4)" src="https://github.com/user-attachments/assets/37be7b5b-718d-4f67-b667-6bdde8764122" />

<video width="100%" controls>
  <source src="Try2Video1.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

<img width="4000" height="3000" alt="Try2Picture (5)" src="https://github.com/user-attachments/assets/45bea64c-2ec8-48a3-a3b4-ae191c9a9093" />

<img width="4000" height="3000" alt="Try2Picture (6)" src="https://github.com/user-attachments/assets/71926e2c-22d5-4ee1-a732-702b60b3c6bf" />

* It was facinating watching the printer put in the bridge for the upperlinks without supports. The filament floated there as it was built on to. I was worried it could affect the final product but it cause no issues.

<video width="100%" controls>
  <source src="Try2Video2.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

<img width="4000" height="3000" alt="Try2Picture (7)" src="https://github.com/user-attachments/assets/94b71b11-e45c-496c-95fa-289a60ab3625" />

<img width="4000" height="3000" alt="Try2Picture (10)" src="https://github.com/user-attachments/assets/3bcbae6d-18f1-4991-86dd-26562eeb4d9b" />

<img width="4000" height="3000" alt="Try2Picture (12)" src="https://github.com/user-attachments/assets/56f05b6a-c340-44f4-872a-142de6829df0" />

<img width="4000" height="3000" alt="Try2Picture (14)" src="https://github.com/user-attachments/assets/1ab45e60-1b81-4ee1-a0c2-b2d5a81fa9ef" />

Once I had the final product, all that was left was to remove the supports and test it.


### Final Linkage Components

| Component | Linkage Section A | Linkage Section B | Linkage Section C | Linkage Section D |
|-----------|-------------------|-------------------|-------------------|-------------------|
| Function | 2 conical Pins that connect B and C | Hole and pin to Rotate around A and Connect to D | Half Length With a Pin and Hole to connect A and D | 2 Pins that connect B and C |
| Creation | 3D Printed | 3D Printed | 3D Printed | 3D Printed |


### Final Linkage Evaluation

<img width="4000" height="3000" alt="Try2Picture (16)" src="https://github.com/user-attachments/assets/35525327-1eea-4872-a11c-94c7c18b3518" />

The final linkage worked as intended. With the supports removed, I just needed to apply a little force to loosen it. It then could move with little friction.

<img width="4000" height="3000" alt="Try2Picture (17)" src="https://github.com/user-attachments/assets/2522b093-d7ec-4fde-a8ff-3dff33c4558e" />

<img width="3000" height="4000" alt="Try2Picture (20)" src="https://github.com/user-attachments/assets/a1b35043-d9b0-4054-8e1c-b8f119535427" />

The linkage could fold up and expand like it should. It felt pretty sturdy too, there never felt like there was a risk the pins were going to break. Obviously, with enough force they would but for simply opening and closing the linkage, it felt structurally sound.

<video width="100%" controls>
  <source src="Try2Video3.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

I was very happy with the end result. It took a lot of work to get it to the final point but now I understand how moving parts are printed in place so much better. And the linkage also acts as a fidget toy.


## Lessons Learned

* **Time: How many hours did the project take from start to finish? Break them down into research, CAD, slicing, printing, post-processing and assembly. How did the total compare with what you expected?**

**Total Time:** 14 Hours

Reasearch: New Linkages - 2 Hours
           3D Print Linkages - 2 Hours

CAD Modeling: 4 Hours

Slicing: 1 Hour

Printing: 2 Hours

Documentation: 5 Hours

I expected the time for this assignment to be on the longer side since this was an entirely new concept and it felt like a big jump from previous labs.


* **Biggest mistake: What was your most significant mistake or failure? What was the root cause, how did you find it, and how did you fix it?**

The biggest mistake was not initially having the two downward facing conical pins extend down to the print bed. The problem caused a lot of issues because the base of the pin would come off the print bed and get in the way, causing the print to fail. I ended up being unable to fix this purely in the slicer. I ended up having to edit the CAD file to add in extra pieces to the bottom of the pins to allow them to adhere to the print bed. I figured the extra material would extrude out once the linkage was removed but it actually causes the links and pins to sit flush.


* **Tolerances: Did your first-print clearances work? What would you change, and by how much?**

The first print clearences I used of 0.4 mm worked well. However, it may be possible to decrease the clearences by 0.1 or 0.2 mm to try and ruduce the rattling of the model since every connection has a decent amount of allowable movemnt. Though the issue is always finding the limit of when the gap will be filled in and the part will be unable to move at all anymore.


## References

[Center Finder Tool With Cabinet Pull Marking Companion](https://www.thingiverse.com/thing:7035457)

[Expanding Star](https://www.printables.com/model/1000576-expanding-star)

[Elephant foot compensation](https://help.prusa3d.com/article/elephant-foot-compensation_114487)

[How to 3D Print Interlocking Parts and Assemblies](https://formlabs.com/blog/how-to-3d-print-interlocking-joints/)

[How To Make Articulated Print In Place Designs | Articulated Shark](https://www.youtube.com/watch?v=XV_pcDC14hE)

[Linkage Designs](https://mechanicaldesign101.com/linkage-designs/)

[Learn 15 Print-in-Place Mechanisms in 15 Minutes](https://www.youtube.com/watch?v=AAKsl8zW-Ds&t=2s)

[Linkage 3D Files from Cults3D](https://cults3d.com/en/tags/linkage)

[Print In Place Scissor mechanism](https://www.reddit.com/r/3Dprinting/comments/xekbyx/print_in_place_scissor_mechanism/)

[3D Printed Scissor Lift Video](https://www.youtube.com/shorts/ZsNt6xYCAH8)

[Preassembled scissor arm](https://www.thingiverse.com/thing:60216)

[Seam position](https://help.prusa3d.com/article/seam-position_151069)

[Trammel of Archimedes](https://www.instructables.com/Trammel-of-Archimedes/)
