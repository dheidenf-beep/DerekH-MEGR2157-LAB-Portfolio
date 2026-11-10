# A11 – SLA Snapfit Design

## Objective

The objective of this lab was to create a working snapfit using the SLA printers and resin.

## Snapfit Research

For my snapfit, I wanted to use cantilever snapfits. Using the provided documents, I researched cantilever snapfits and then how to print moving parts with SLA printers.

For my Design, I used inspiration I got from the Formlab website document on SLA printing snapfits.

<img width="1698" height="827" alt="SLASnapfitScreenshot (39)" src="https://github.com/user-attachments/assets/213ae945-e626-4ce5-b507-6196df90e482" />

I decided to repurpose the concept of the snapfit to be a small container. I decided to design it around some small sticky notes I have.

I measured the sticky notes to have a width of about 15 mm and a height of 50 mm. The snapfit container would consist of a base which had the actual snapfits and the lid or enclosure. I intended to correct one mistake with I made on my first FDM snapfit which was to model the snapfits as cantilever beams but then not being able to press down on the farthest most edge of the clip. 

I also wanted the snapfit to come out easier. Doing some research showed that different angles on the clip could make it harder or easier to remove. I decided to go with a 45 degree angle on both sides of the clip so that the clip would ideally be easier to pull out. 

As for clearances, the Preform website provided a couple different clearances.

<img width="911" height="277" alt="SLASnapfitScreenshot (40)" src="https://github.com/user-attachments/assets/2f387a52-8311-4828-9ff4-90ab8528e879" />

Since the snapfit was not meant to be permanent but also not meant to be a moving fit, I selected the 0.2 mm clearance. 

I used the equations for cantilever snapfits from the "Snapfit Design Guide" provided to us for the assignment. 

<img width="920" height="658" alt="SnapfitEqns" src="https://github.com/user-attachments/assets/66ade4ed-125e-4f42-9b68-af2966ba2ec1" />

After determining which parameter to solve for, I ended up using the top strain equation and plugging it into the bottom equation to find the needed length for my desired deflection of 2 mm. The 2 mm deflection came from the wall thickness. 

<img width="1275" height="1615" alt="A11SLASnapfitWork_page-0001" src="https://github.com/user-attachments/assets/3ff05294-f29e-44c5-8f26-1df786dadda4" />

I plugged this into Solidworks to derive the numerical length.

SLA Resin can affect the allowable deflection and overall geometry due to how the resin is printed and the material properties. The material properties change with different curing rates and temperatures, affecting flexibility and stiffness. Part orientation due to SLA printing in layers. Depending if the force is applied parallel or perpendicular to the layers can affect how the part will need to be designed and printed.

## CAD Design

For the design of the CAD model, I first started by laying out my equations to make the model parametric. 

<img width="780" height="503" alt="SLASnapfitScreenshot (32)" src="https://github.com/user-attachments/assets/4ca0c74b-4e7d-4082-9d82-d99f318723ac" />

The height and base values were for the dimensions of the prongs and the length was parametrically derived from the given equation for strain of cantilever beams and deflection of cantilever beams. The other parameters, such as the diameter and height of the cap was derived from the post-it notes I was modeling around. I followed the Formlab recommended to make the wall thickness at least 2 mm. The clearance was chosen above from the Formlabs website to be 0.2 mm. Other parameters like "force" and "t" (which was the thickness of the base) were arbitrarily chosen by me. The elastic modulus was derived from the Formlabs datasheet on V5 Gray resin.

<img width="541" height="396" alt="image" src="https://github.com/user-attachments/assets/d707f590-41f6-4ea6-a64f-400b31ee6537" />

I had a couple issues with the equations near the end, which is why some (like the clearance and base) are slightly off. The clearance should be 0.2 mm and the base should be 3 mm. 


### Snapfit Base

For the base I started with a circle and extruded it up to be a thin disk. 

<img width="960" height="564" alt="SLASnapfitScreenshot (3)" src="https://github.com/user-attachments/assets/07f7aecb-2136-4d45-8da1-1582c5d5c586" />

<img width="960" height="564" alt="SLASnapfitScreenshot (4)" src="https://github.com/user-attachments/assets/3cd83bb6-eeb9-4f42-9b70-adbf9de10bd4" />

I then marked out where the prongs would go. They needed to be at least 2 mm away from the edge for the walls of the cap, plus the clearance. I put them two millimeters away from the most extreme points on the circle and then accounted for the prongs scraping against the circular area of the cap in the cap model.

<img width="960" height="564" alt="SLASnapfitScreenshot (5)" src="https://github.com/user-attachments/assets/6ebcda3d-758a-431f-b9c4-aa60bc31886d" />

<img width="960" height="564" alt="SLASnapfitScreenshot (6)" src="https://github.com/user-attachments/assets/246baa22-c9b2-49d4-a980-157103799e8b" />

The prongs were extruded up to the parametrically determined length and then another 6 mm or so for the clip length. 

The clips started as rectangles that Had the base dimensions of the clip length and width of the main prong body. I extruded them out 2 mm since all of the walls on the model are 2 mm thick. 

<img width="960" height="564" alt="SLASnapfitScreenshot (7)" src="https://github.com/user-attachments/assets/6a7e6973-ed5f-4da8-83f7-4f91cae22db0" />

I could then extrude cut in the 45 degree angles to ideally improve the insertion and removal of the base of the design into the cap. 

<img width="960" height="564" alt="SLASnapfitScreenshot (8)" src="https://github.com/user-attachments/assets/910d9653-8aa6-434b-89f0-44160a42c8f6" />

<img width="960" height="564" alt="SLASnapfitScreenshot (9)" src="https://github.com/user-attachments/assets/73f9dd61-d433-43cd-a9a3-c0c232203604" />

<img width="960" height="564" alt="SLASnapfitScreenshot (10)" src="https://github.com/user-attachments/assets/f7f84ce9-9159-40ba-be11-3862cf4d18e5" />

<img width="960" height="564" alt="SLASnapfitScreenshot (11)" src="https://github.com/user-attachments/assets/e3ff1e50-2bf0-4899-b4ce-44b38373f798" />

The last thing I needed to add were fillets to prevent stress concentrations. I chose a 0.5 mm fillet for the edges on the clip side and a 1 mm fillet for the fillets surrounding the base of the clips.

<img width="960" height="564" alt="SLASnapfitScreenshot (29)" src="https://github.com/user-attachments/assets/3c6b6d32-e808-40cd-ab33-25f752d53e56" />

With the base done, I could move onto the cap of the design. 


### Snapfit Enclosure/Cap

For the enclosure, I once again started with a circle I extruded into a cylinder. I then extruded out the center of the cylinder to create the 2 mm thick walls. 

<img width="960" height="564" alt="SLASnapfitScreenshot (12)" src="https://github.com/user-attachments/assets/f7f144df-07f1-4d20-a4f6-ae778d14e7db" />

<img width="960" height="564" alt="SLASnapfitScreenshot (13)" src="https://github.com/user-attachments/assets/e13db62a-c17e-4fcc-8ab2-ffb83d524dc9" />

In order to put in the holes for the snapfit, I would need to be able to work on the inside surface of the cylinder. This required me to create reference planes tangent to the inside curve and parallel to the front plane.

<img width="960" height="564" alt="SLASnapfitScreenshot (16)" src="https://github.com/user-attachments/assets/47e2f052-f43a-4984-bc73-7e2709e1ca38" />

<img width="960" height="564" alt="SLASnapfitScreenshot (17)" src="https://github.com/user-attachments/assets/6afeaf22-7e78-4462-b736-32ffcc5dd900" />

Once I had the plane, I cut out a rectangular groove the width of the prongs (plus the clearance) on the inside of the cylinder to account for the straight, rectangular geometry of the prongs. This was so that the prongs ideally wouldn't be subjected to any more stress than was calculated for. 

<img width="960" height="564" alt="SLASnapfitScreenshot (18)" src="https://github.com/user-attachments/assets/11fefe18-b641-415c-94d2-8d47f2842285" />

<img width="960" height="564" alt="SLASnapfitScreenshot (19)" src="https://github.com/user-attachments/assets/39180be6-068f-4a02-8b20-e2756ca022c9" />

I then created another hole in the cylinder for the prongs to slide into that was set to be a distance the length of the prongs from the base of the cylinder. 

<img width="960" height="564" alt="SLASnapfitScreenshot (20)" src="https://github.com/user-attachments/assets/c3ee3203-480b-44a7-8a24-c0a38f954380" />

<img width="960" height="564" alt="SLASnapfitScreenshot (21)" src="https://github.com/user-attachments/assets/1b0efc4f-a4e0-4766-aa17-96943b090400" />

Next, I created the opposite 45 degree angles for the angles on the prongs to set into.

<img width="960" height="564" alt="SLASnapfitScreenshot (22)" src="https://github.com/user-attachments/assets/50e1ae9d-4cf8-4366-96df-e99354026bbc" />

<img width="960" height="564" alt="SLASnapfitScreenshot (23)" src="https://github.com/user-attachments/assets/8351fd13-19c5-4b12-9730-0cee0f6ee1bc" />

<img width="960" height="564" alt="SLASnapfitScreenshot (24)" src="https://github.com/user-attachments/assets/468adb53-9a2c-4b86-88c8-a6a5c27fd73e" />

I finally added 0.5 mm fillets to all of the edges to reduce stress concentrations. 

<img width="960" height="564" alt="SLASnapfitScreenshot (25)" src="https://github.com/user-attachments/assets/84d8b982-2a6e-425c-9e4e-1f99e0239cf0" />

To finish it off, I added a top to the cap to seal it off. 

<img width="960" height="564" alt="SLASnapfitScreenshot (41)" src="https://github.com/user-attachments/assets/eb18a3b4-addd-48e3-bcd9-4fde165bc7ec" />

To verify the models worked, I put them together in an assembly. The first couple iterations were a bit off and the Solidworks equations started giving me trouble for some reason. 

<img width="960" height="564" alt="SLASnapfitScreenshot (31)" src="https://github.com/user-attachments/assets/f8f28da9-66a0-4ae6-b4bf-fb988da7eaf3" />

After a lot of adjusting of dimensions and playing around with it, I eventually got something that looked like it would fit together well. 

<img width="960" height="564" alt="SLASnapfitScreenshot (42)" src="https://github.com/user-attachments/assets/73bb5450-0684-4d7b-b9a2-bb2c42ccd52e" />

<img width="960" height="564" alt="SLASnapfitScreenshot (43)" src="https://github.com/user-attachments/assets/b7973ed0-0d02-4ece-b225-c6823993d2d5" />

<img width="960" height="564" alt="SLASnapfitScreenshot (44)" src="https://github.com/user-attachments/assets/f0c77218-54ea-4dba-8fb3-d9c8c8b86083" />

Once I was happy with the design, I moved onto the preprocessing stage. 


## Preprocessing

First, the models were loaded into the Formlab slicer.

<img width="960" height="564" alt="SLASnapfitScreenshot (45)" src="https://github.com/user-attachments/assets/3cdc6bc3-066a-46b4-bd00-7f03a045398b" />

I figured the preprocessing for the model wouldn't be too hard and I would just print the pieces standing straight up. However the cap ran into the problem of having suction forces on the inside requiring it to be at an angle. I tested a couple different orientations that would remove the suction forces but also wouldn't print any supports inside the cap. 

<img width="960" height="564" alt="SLASnapfitScreenshot (47)" src="https://github.com/user-attachments/assets/22ae6011-606c-4fc3-b385-21fc5c5c00ce" />

<img width="960" height="564" alt="SLASnapfitScreenshot (46)" src="https://github.com/user-attachments/assets/301ee2d9-f06c-4ddd-b967-9759af2582a6" />

The one I decided on was a 45 degree angle with the top of the cap away from the build plate.

<img width="960" height="564" alt="SLASnapfitScreenshot (33)" src="https://github.com/user-attachments/assets/a01216b4-edf1-4a09-a683-981500f91d22" />

The other issue I read about that I wanted to account for so my print didn't fail was that SLA printers can struggle printing tall and spindly parts due to suction forces when the build plate rises up and another layer of resin is added. I was worried that the prongs on the base would break off. So, I set the base to be at a 45 degree angle. I also messed with the support settings some to try and get reinforcing supports on the prongs but I couldn't get them to generate. 

<img width="960" height="564" alt="SLASnapfitScreenshot (35)" src="https://github.com/user-attachments/assets/f6215e56-3ef2-4233-afd3-1b18aae412e9" />

<img width="960" height="564" alt="SLASnapfitScreenshot (36)" src="https://github.com/user-attachments/assets/06195e0c-06d4-4015-a2cc-77901a122217" />

<img width="960" height="564" alt="SLASnapfitScreenshot (34)" src="https://github.com/user-attachments/assets/ec945e0b-dcba-4980-8057-bb9288586a3e" />

After a lot of iterating, I decided to try and print and see what happens. The layout orientation wasn't chosen for a specific reason and was done by the auto-layout feature. The design would be closer to anisotropic due to the printing orientation it needed to reduce suction forces. 


## Printing

The design was printed on the Form 4 SLA printer named: "HallowedDodo"

<img width="960" height="564" alt="SLASnapfitScreenshot (38)" src="https://github.com/user-attachments/assets/e24c6e20-5d52-40bf-96b8-030f5511f1ca" />

It was printed using gray V5 SLA Formlab resin. It had the largest layer thickness of 0.100 mm to reduce time. The print took about an hour and 20 minutes and approximately 22 milliliters of resin. 

The first time trying to print the design was stopped because the printer warned of debris on the print bed. I got to see how that issue was dealt with by the Super Fab Lab staff who helped me clean the printer and restart the print. 

The second attempt didn't run into any issues. Nothing snapped off and everything looked good. 

<img width="3000" height="4000" alt="SLASnapfitPhoto (1)" src="https://github.com/user-attachments/assets/b7c3ec04-4fdd-430c-aa96-9773509682c2" />

<img width="3000" height="4000" alt="SLASnapfitPhoto (3)" src="https://github.com/user-attachments/assets/a52104c3-751b-49d5-87cb-9a5b83e45453" />

<img width="4000" height="3000" alt="SLASnapfitPhoto (4)" src="https://github.com/user-attachments/assets/4a564ace-91cf-438f-8904-1493b1cae101" />

<img width="4000" height="3000" alt="SLASnapfitPhoto (5)" src="https://github.com/user-attachments/assets/61f6770c-bc70-4e0c-924a-82068ceed73a" />

<img width="4000" height="3000" alt="SLASnapfitPhoto (7)" src="https://github.com/user-attachments/assets/b102f21b-c4a2-4dbd-9238-8d8d5b2c58db" />

<img width="3000" height="4000" alt="SLASnapfitPhoto (11)" src="https://github.com/user-attachments/assets/740c9f11-3c03-421c-a4ba-aca2713df129" />

<img width="3000" height="4000" alt="SLASnapfitPhoto (10)" src="https://github.com/user-attachments/assets/b331487d-2615-419b-aff9-b6f750966594" />


### Post-Processing

I removed the print bed and set it into the cleaner with the parts still attached (although, the cap was slightly too tall so I did take it off). The cleaning took about 5 minutes. 

<img width="4000" height="3000" alt="SLASnapfitPhoto (13)" src="https://github.com/user-attachments/assets/afdbe696-de1a-4e03-a618-2c27bcf133ec" />

<img width="4000" height="3000" alt="SLASnapfitPhoto (16)" src="https://github.com/user-attachments/assets/7f461eb6-dc10-410a-ba8f-f8bb3d7a9402" />

Next I removed the supports from the pieces and set them into the curing chamber. The curing process took about 25 minutes because it took a while for it to heat up.

<img width="3000" height="4000" alt="SLASnapfitPhoto (17)" src="https://github.com/user-attachments/assets/90bdd468-0444-4353-ba70-62ffb553e310" />

## Design Evaluation

The final design came out good. I couldn't find a file or I would have otherwise filed off the support remnants. None of the rest of the print needed filing and fit together very well. The connection wasn't the tightest due to how liberal I was with the clearances because I was paranoid after the last lab. The parts did fit together and would stay together even when shacking. The base would come out if you applied a little force pulling it out, which worked out because I forgot to plan for how someone would get their fingers into the holes to push down on the prongs. But the snapfit would still snap into place and had enough friction to hold the sticky notes I designed it around without the base slipping out.

<img width="3000" height="4000" alt="SLASnapfitPhoto (20)" src="https://github.com/user-attachments/assets/5fe6a55c-13b4-44e5-afd5-477aef8bd8c8" />

<img width="3000" height="4000" alt="SLASnapfitPhoto (22)" src="https://github.com/user-attachments/assets/ec0bfcae-b8b2-48ff-8b6f-2516f9634b64" />

<img width="3000" height="4000" alt="SLASnapfitPhoto (24)" src="https://github.com/user-attachments/assets/21a32bc0-ef3f-4859-87da-16bd69b09074" />

Overall, while it wasn't exactly what I was expecting, I was happy with it and that it worked. 

I didn't test the flexibility before curing the print because I wanted to be as careful with it as I could and I was still worried the prongs might break off. The surface finish was good in all the places except where the supports were which was to be expected. I was also noticing that the when the pieces were going together, they were already beginning to get scratched up. 

There are a couple mechanical differences between SLA and PLA (FDM) parts. A big one is the surface finish. The layers are a lot more noticeable on PLA parts than on SLA parts. This gives SLA parts a better surface finish. There is also the difference in material. Resin acts very differently compared to plastic filament. The tolerances, forces, and stresses need to be accounted for differently based on the which method the part is printed. The supports are also very different. SLA supports tend to leave more noticeable blemishes on the surface of SLA parts, requiring the need to file it down. PLA parts often have supports that are easier to remove and leave less of a mark behind.


## Lessons learned

* What challenges arose designing for resin flexibility and clearance?

It was challenging to figure out the uniform clearance and where to apply it. I ended up being very liberal with applying the clearance everywhere to ensure there would be no issues with the parts not being able to go together after the issues I had with the last lab.

* What did you learn about SLA tolerances and print orientation?

SLA tolerances tend to be more loose than other tolerances due to how resin expands after curing. Print orientation is important for ensuring there are no suction forces or pockets of trapped resin. 

* How do SLA snap fits differ from FDM snap fits?

SLA snapfits have a different material with different properties that can change throughout the curing process. This necessitates more careful consideration of the parameters used in the calculations while FDM snapfits don't change much after printing.

* Comment on cost, time, and resources used from start to finish.

SLA prints take more time, cost slightly more, and uses a lot more steps than FDM printing. However, it does allow SLA printers to reach greater levels precision and detail. SLA Prints are definitely more suited to smaller scale, more detailed parts due to the cost and time it takes to print something.

**Time Spent:** 8 Hours

## Resources

[Plastic_Snap_fit_design.pdf](https://github.com/user-attachments/files/34612662/Plastic_Snap_fit_design.pdf)\

[Snap Fit Joint Design: Types, Applications, Advantages, and Disadvantages](https://www.xometry.com/resources/machining/snap-fit-joint-design/)

[How to Design and 3D Print Snap-Fit Joints for Enclosures, Boxes, Lids, and More](https://formlabs.com/blog/designing-3d-printed-snap-fit-enclosures/)

[How to design parts for SLA 3D printing](https://www.hubs.com/knowledge-base/how-design-parts-sla-3d-printing/)

[Unveiling Resin – 3D Printing Materials Detailed & Compared](https://qmolding.com/resin-3d-printing-materials/)

[3D Print Interlocking Parts: Design Interlocking Joints Guideline](https://qmolding.com/3d-printing-interlocking-parts/)

[Grey Resin V5](https://dental-media.formlabs.com/datasheets/2401898-TDS-ENUS-0.pdf)


