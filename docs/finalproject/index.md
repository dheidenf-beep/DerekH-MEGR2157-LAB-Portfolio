# Final Project – Cable Manager

## Objectives

The objective of the final project is to determine a real problem to solve and then design a solution to that problem using the different additive manufacturing methods from the lab. 

## Research

### Spiral Design Process

The spiral design process is a risk-based process for designing new parts or systems. The model is broken up into 4 stages: planning, risk assessment, engineering or prototyping, and evaluation. During the planning stage, the goal is defined and a plan is made to achieve that goal. During The risk assessment phase, risks are evaluated in relation to cost, performance, and scheduling with the best solution being selected. A prototype is then engineered and created based on the design and risk assessment outcomes. The model is then evaluated by customers or other people not necessarily involved with the design. Feedback form the design evaluation is then used to restart the process and design a new prototype that is better than the previous iteration. 

The Spiral Design Process is a good way to evaluate a models final designs through prototyping, allowing a quicker identification of problems and before the final design. For my final project, the spiral design process helps to speed up the iteration process by designing and creating an actual prototype and letting it be evaluated by my peers to receive feedback on how I can improve the design.

### FDM Anisotropic

Standard Fusion Deposition Modeling parts are inherently anisotropic due to the fact that the parts are printed in layers. Anisotropic parts are described as parts have properties that differ depending on direction or orientation. FDM parts are anisotropic parts due to the layered construction method. The presence of layers changes how the plastic withstands stress and deformation depending on the orientation of the force to the seams. The printed layers are stronger than the seams connecting since the plastic is all one melted and fused piece. FDM parts have higher strength when the force is parallel to the layers instead of perpendicular which pulls on the seams.

### SLA Shrinkage

Resin parts printed by sterolithography printers have a much higher dimensional accuracy on average compared to other manufacturing processes such as FDM. However, due to the chemical properties of the resin, parts can shrink an average of 1.5 to 3% after being printed and cured. Generally, resins that are more brittle tend to shrink less on average than more elastic polymers. SLA printers use higher accuracy lasers to cure resin and if these lasers are not precisely aligned, it can cause dimensional inconsistencies. Other factors such as temperature, haze on the resin tank, and outside light can affect the dimensional accuracy. Many modern SLA slicers attempt to account for the shrinkage by scaling up the part. This can also be done manually to ensure the final product is around the desired size. Depending on the printer and calibration of the laser, SLA can reach very fine details but the shrinkage and changes in the resin cause SLA part sizes to be inconsistent at times, requiring higher clearances to account for it.

### Laser Cutting Kerf

The primary method of accounting for laser cutting kerf is to offset the dimensions of the part being cut by the kerf. This way, the extra material will be obliterated by the laser, leaving the part with the desired dimensions. However, kerf can be difficult to determine as it depends on the material, material thickness, and the properties of the laser. Testing fits or tolerances on parts is good for determining correct tolerances and appropriate dimensions accounting for kerf. Kerf can cause joints to fit together loosely and decrease total dimensional accuracy for parts that require small tolerances.


## Problem to Solve

### Problem 1 - Disorganized Silverware

All of the silverware I use in my dorm had just been thrown into a draw with no semblance organization or a way to organize it. While this could be easily solved by simply buying a holder for the silverware, that's less fun than designing an elaborate, overengineered solution.

### Problem 2 - Headphone Placement

I don't have a permanent place for my headphones when I am not using them, which makes them prone to falling onto the floor and breaking. Being able to reduce this would be preferable so I don't have to keep buying more headphones.

### Problem 3 - Unwieldy Cables

I have several long USB-C and other cables on my desk for charging my phone and various devices. However, when I am not using these cables, they tend to wonder all over the place, down onto the floor and into crevices I can't reach in. This requires me to have to go fishing for cables every time I want to use one. This isn't helped by the fact that the excess length of the cable is really good at weighing down the rest of the cable, making it harder to leave it on a surface without it falling off. 

### Chosen Problem to Solve

The problem I chose to solve was the issue of the really long cables on my desk. This one seemed like it had the most opportunity for interesting solutions.

## Part 1

### Problem Outline

I have too many long cords on my desk that tend to get end up on the floor or other inconvenient places. My plan is to design a system to keep the cords more accessible so that I do not need to keep fishing every time I want to plug in my phone. 

### Prototype Concept

For my first idea, I wanted to create a stationary spool that would be able to wind up the cord. However, when I printed a test spool, I determined that the spool idea wasn't going to work or it would require a very complicated solution. 

So, instead, I came up with something simpler. The design would be a simple wire holder that would rest on the desk with multiple slots for several wires. The design would utilize FDM printing for the upper portion to hold the wires and a larger base laser cut out of wood that would rest against the wall or something else to prevent the whole build from sliding off the desk due to the weight of the wires, since the FDM and wood parts aren't very heavy. 

<img width="1275" height="1549" alt="MEGR-2157-L3D-FinalProjectWrittenPapers_page-0007" src="https://github.com/user-attachments/assets/c5934f43-f3a6-4e97-8ebd-b2349eb15590" />


### Prototype CAD Design

#### Cable Measurements

The cables I used to test were braided and non-braided USB-C cord. Since my design ideas required the holding of the cables, I measured the cables with calipers to get a better idea of how big I needed to make the slots for the cables.

<img width="4000" height="3000" alt="CableMeasure (6)" src="https://github.com/user-attachments/assets/4cdd81ed-0e23-4b37-a635-3a4d3790eb55" />

<img width="4000" height="3000" alt="CableMeasure (13)" src="https://github.com/user-attachments/assets/162ba811-183a-465e-b979-0c80730607f9" />

I measured the cables in three places, near the ends and once in the middle, and averaged the measurements. 

For the braided cord, the average diameter/thickness was 0.148 in. or 3.76 mm.
For the regular cord, the average diameter was 0.1208 in. or 3.07 mm.

I use the braided cord more frequently so I went with the 3.76 mm.


#### Spool - Initial Idea

Briefly mentioning the first design, the original plan was to create a spool to wind up the wire. The spool would be 3D printed and the frame would be laser cut from wood. The design of the spool itself was very simple, just a spool with a slot in it to hold the wire and prevent it from retracting back in. 

<img width="960" height="564" alt="SpoolPic (11)" src="https://github.com/user-attachments/assets/4acf2fb6-85be-4f1b-a874-7a941883ecb3" />

<img width="4000" height="3000" alt="SpoolActPic (9)" src="https://github.com/user-attachments/assets/4833ca20-f523-4ccd-9104-b7f3a1cfb0c8" />

However, there were several issue with the spool idea. First, the PLA didn't have the friction required to role up the USB-C cord I was using to test. It did start retracting the cable if it was wrapped around the spool a couple times initially. However, it would pull on both ends of the so hard that there was no way I could create a stationary spool that only retracts one end. So instead, I came up with a new, simpler idea.

#### Cable Holder - Better Idea

My next idea was to create a simple 3D printed holder with slots for the wires to slip into. The holder would sit on a wood, laser cut base to give it stability and prevent it from tipping. 

The CAD model was fairly straightforward. I started by defining my equations and creating a side profile to extrude.

<img width="586" height="217" alt="CableHolderEqns" src="https://github.com/user-attachments/assets/48912e2b-36ba-4838-905c-f70333aa0900" />

<img width="960" height="564" alt="CableHolderPic (2)" src="https://github.com/user-attachments/assets/4a81d05b-24a6-4880-9f8a-55aa27646845" />

<img width="960" height="564" alt="CableHolderPic (3)" src="https://github.com/user-attachments/assets/44e905f6-4c9a-43b5-8fcc-ed5887a1a25f" />

I then extruded cut the holes for the cables to rest in, giving a bit of clearance so the wire would just sit in the hole and not be fit in.

<img width="960" height="564" alt="CableHolderPic (4)" src="https://github.com/user-attachments/assets/d82bc093-4037-4890-9305-8591c1a0955d" />

<img width="960" height="564" alt="CableHolderPic (6)" src="https://github.com/user-attachments/assets/d4cc3982-5a54-49d3-9d28-ecf75f254adc" />

The final part was creating the pieces in the bottom that would fit into the wood. 

<img width="960" height="564" alt="CableHolderPic (8)" src="https://github.com/user-attachments/assets/45fc6211-d013-4fb3-b312-fd0d9b86beaf" />

I made these the ideal thickness and width not accounting for the laser cutter kerf since there is no kerf on the 3D printer.

<img width="960" height="564" alt="CableHolderPic (9)" src="https://github.com/user-attachments/assets/15207f16-b109-407c-b514-4b5e5ba100af" />

With a little more tinkering with the measurements, I finished with the first design of the cable holder.

-----------------------------

In order to ensure the wood would fit with the cable holder, I created a test fit coupon with 8 different sized slots starting at +0.2 mm and decreasing by 0.1 mm each step down to -0.5 mm. I chose 0.5 mm to stop at because that was the clearance I used on my laser cut assignment. 

<img width="960" height="564" alt="CableHolderPic (11)" src="https://github.com/user-attachments/assets/7bc3b0a6-5e1e-4273-bb28-cb1c86916f80" />

* The hexagon was just so I knew which side was which.

<img width="960" height="564" alt="CableHolderPic (12)" src="https://github.com/user-attachments/assets/999705fb-9eca-4a8a-a067-2183a3ae0ccb" />

<img width="960" height="564" alt="CableHolderPic (13)" src="https://github.com/user-attachments/assets/37289117-95f9-4c33-a05c-2593cf8d1654" />

I preemptively designed the wood stands which were just rectangles with a slot cut into it. I used 0.2 mm as my kerf because that was the number I used for my original laser cutter assignment and I used the same laser cutter to cut out these pieces. 

<img width="960" height="564" alt="CableHolderPic (15)" src="https://github.com/user-attachments/assets/a0a0ab2b-627c-4095-b36c-20b50970ad5e" />

<img width="960" height="564" alt="CableHolderPic (16)" src="https://github.com/user-attachments/assets/c3067825-2573-4fd9-a221-8a972ebae6ca" />

I created the dimensions with the clearance built in that I would adjust after testing the fit coupon. 

Since I could, I also created an assembly to view the parts together. 

<img width="960" height="564" alt="CableHolderPic (17)" src="https://github.com/user-attachments/assets/c77ed728-906a-471b-807e-6e0e2b993064" />


#### FDM Printing

For the printing of the cable holder, I kept it fairly basic. The orientation was straight up, even though that meant a bunch of supports would have to be printed underneath the base. Teh primary reason I kept this orientation was to try and keep the slots that would go into the wood as accurate as possible. The only parameters I changed was switching the supports to organic supports and increasing the infill to 20% and also changing the pattern to be triangles. I kept it on the "0.20 mm STRUCTURAL" setting to make sure the print didn't come off the print bed. The print took around 14 minutes and was printed on printer 15. 

<img width="960" height="564" alt="CableHolderPic (20)" src="https://github.com/user-attachments/assets/12112dcc-24b1-4662-8dd2-c0dabb8f403f" />

<img width="4000" height="3000" alt="CableHolderActPic (3)" src="https://github.com/user-attachments/assets/f8840f1a-f8cb-4826-90f8-1810be5331bd" />

<img width="4000" height="3000" alt="CableHolderActPic (7)" src="https://github.com/user-attachments/assets/e765b3e6-4b0c-4dae-903e-389e9b3bee59" />

<img width="4000" height="3000" alt="CableHolderActPic (9)" src="https://github.com/user-attachments/assets/1faf3fb3-265f-4810-ad53-f1f1785c37f0" />

The print came out well, the only trouble I had was with removing the immense amount of supports on the bottom.


#### Laser Cutting

For the laser cutting, I first printed the fit coupon to determine the best clearance to get a reasonably tight fit. The wood was cut using the standard parameters for 3 mm thick wood. These parameters were 20% speed, 100% power, and 20% frequency.

<img width="796" height="584" alt="CableHolderPic (22)" src="https://github.com/user-attachments/assets/2e8c9189-59cc-4700-a25f-2aac90027f34" />

<img width="4000" height="3000" alt="CableHolderActPic (15)" src="https://github.com/user-attachments/assets/6b7e9127-b171-4093-974a-a4505642d952" />

<img width="4000" height="3000" alt="CableHolderActPic (16)" src="https://github.com/user-attachments/assets/048c1b1c-8423-4bae-ba09-d3a768654062" />

<img width="3000" height="4000" alt="CableHolderActPic (18)" src="https://github.com/user-attachments/assets/3fe654b9-c707-4e56-88a0-fd9bc4ec7017" />

The clearance that seemed to give the best fit was -0.3mm clearance. So I applied this to the wood stands and laser cut them out. 

<img width="960" height="564" alt="CableHolderPic (23)" src="https://github.com/user-attachments/assets/c9324c44-8749-441c-a65e-71a91262176b" />

<img width="960" height="564" alt="CableHolderPic (24)" src="https://github.com/user-attachments/assets/1882c7d1-9620-4108-94c2-a8bf3c618655" />

<img width="960" height="564" alt="CableHolderPic (25)" src="https://github.com/user-attachments/assets/ebe98b9a-772e-4800-b2b5-55d4b5569b02" />

<img width="4000" height="3000" alt="CableHolderActPic (19)" src="https://github.com/user-attachments/assets/2dad6ebf-4ba1-49ec-a4e5-48d33af2cbe3" />

<img width="4000" height="3000" alt="CableHolderActPic (20)" src="https://github.com/user-attachments/assets/53fb5a57-ce64-4a37-8359-4292b1234a19" />


### Prototype Evaluation

The prototype ended up being smaller than I anticipated, which seems to happen quite a lot. This made it unable to reach the wall across the gap between my desk and the wall. However, if you do put it up against something like a book, the concept is there, although the slots for the wires could also be larger.

<img width="3000" height="4000" alt="CableHolderActPic (21)" src="https://github.com/user-attachments/assets/db57b31f-849e-4984-8389-2412b859238a" />

The fits that came out on the wood stands were still a tad loose, meaning -0.4 mm of clearance would likely be better for the fit.

<img width="4000" height="3000" alt="CableHolderActPic (23)" src="https://github.com/user-attachments/assets/58bbc237-56ca-4b93-ab99-11fc2faf1fe5" />

Overall, the concept is there but it could definitely use improving for the final design.


### Part 1 Problem Presentation

[![Final Project Problem Presentation](http://img.youtube.com/vi/OiNjsAemug4/0.jpg)](http://www.youtube.com/watch?v=OiNjsAemug4)

## Part 2

### Classmate Feedback

Below are the filled out feedback forms from my classmates:

<img width="1262" height="1650" alt="MEGR-2157-L3D-FinalProjectWrittenPapers_page-0001" src="https://github.com/user-attachments/assets/53e42a5b-4975-4713-b68e-2ce5ef2ebc51" />

<img width="1275" height="1606" alt="MEGR-2157-L3D-FinalProjectWrittenPapers_page-0002" src="https://github.com/user-attachments/assets/42da9749-bcbd-461e-abe0-518618088792" />

<img width="1238" height="1650" alt="MEGR-2157-L3D-FinalProjectWrittenPapers_page-0003" src="https://github.com/user-attachments/assets/096bb209-afb3-43e0-bc50-75ce21257401" />

<img width="1248" height="1650" alt="MEGR-2157-L3D-FinalProjectWrittenPapers_page-0004" src="https://github.com/user-attachments/assets/0179f59c-e91f-4f26-8290-f50d460c68b5" />

<img width="1238" height="1650" alt="MEGR-2157-L3D-FinalProjectWrittenPapers_page-0005" src="https://github.com/user-attachments/assets/31ce120f-8439-4a0f-8c26-e3f27432e5f7" />

<img width="1241" height="1650" alt="MEGR-2157-L3D-FinalProjectWrittenPapers_page-0006" src="https://github.com/user-attachments/assets/1f8c703d-6cb7-42be-9104-13399733776d" />

The primary feedback I received was on the ability of the stand to hold the wires, which wasn't great. Since the concept was that the wires would Ideally stay within the channels of the holder so that once the user was done using the wire, it would fall back into the channel and wouldn't fall onto the floor. The suggestion and solutions I was given was to maybe try and make a snapfit the would keep the wires from coming out or create something that would snap onto the wire itself and would hook are attach onto the holder to prevent the wire from coming out. 

I also received feedback on how to fit in multiple sized wires. Currently, the stand was designed around one size of USB-C wire, which makes the use cases for it more specific with a lesser ability of being used generally. 

The last bit of feedback I received was on the stability, which was already an issue. The prototype was so small and light that the wires would just pull the stand down, which obviously isn't helpful when trying to create a wire holder to keep wires off of the floor. Since the manufacturing options I have access all use very light materials, the two options I am really left with are 1: using another non-manufactured component such as tape, Dual Lock, or just a weight or 2: try and increase the size of the base to achieve the original idea of having the base rest against the wall. I figured the tape or Dual Lock ideally would probably be the easiest solution by just creating a more solid wood base for the stand but I decided to also try increasing the size to see if I could get it to rest against the wall.


### Design Revision

With the feedback acquired, I went back into Solidworks to start improving the design. I started by increasing all of the dimensions to make the whole stand bigger.

| Before | After |
|------|----|
| <img width="593" height="397" alt="CableRevisionScrnSt (1)" src="https://github.com/user-attachments/assets/12792495-e160-4779-bd0b-4109cff72bd9" /> | <img width="593" height="397" alt="CableRevisionScrnSt (2)" src="https://github.com/user-attachments/assets/26fc5bb4-1ab4-4b92-8d6e-6c8bcf70be2f" /> |

<img width="960" height="564" alt="CableRevisionScrnSt (3)" src="https://github.com/user-attachments/assets/eac6a2cc-2c18-4c42-9d22-4811999b8a58" />

Needed to edit the holes and the spacing a bit. I also played around a lot with the depth (height?) of the holes to try and get something I thought was reasonable. 

<img width="960" height="564" alt="CableRevisionScrnSt (4)" src="https://github.com/user-attachments/assets/d254fde4-13e8-4bb7-b1eb-5f0fab50073c" />

To solve the issue of the wires coming out of the holes, I created a separate part that would press fit onto the top of the cable holder to lock the wires in. 

<img width="960" height="564" alt="CableRevisionScrnSt (8)" src="https://github.com/user-attachments/assets/a3d063e9-1f78-45e3-83e8-a6224ed9282c" />

<img width="960" height="564" alt="CableRevisionScrnSt (6)" src="https://github.com/user-attachments/assets/58f0c9bb-91c6-4fca-807f-26bc581b9754" />

<img width="960" height="564" alt="CableRevisionScrnSt (7)" src="https://github.com/user-attachments/assets/81dd450c-1af6-4f14-b966-236ab176a797" />

I ended up making it hollow so it would be able to slide down as far as the user wanted it to lock the wires in place.





## Resources

[Spiral Model in Software Engineering](https://www.geeksforgeeks.org/software-engineering/software-engineering-spiral-model/)

[Anisotropic](https://www.sciencedirect.com/topics/engineering/anisotropic)

[How Accurate is SLA 3D Printing? A Technical Look at Tolerances](https://sgd3d.co.uk/3d-printing/sla-3d-printing-accuracy-tolerances/)

[Understanding Kerf and Kerf Offset](https://www.thunderlaserusa.com/knowledge/understanding-kerf-and-kerf-offset)

[Design for Laser Cutting](https://making.stanford.edu/resources/process-guides/laser-cutting/design-laser-cutting)
