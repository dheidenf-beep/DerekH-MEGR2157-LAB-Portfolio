# A10 – SLA RC 2 Fit

## Objective

The objective of this lab was to use a stereolithography (SLA) 3D printer and create a part with an RC 2 running and sliding fit using the tolerances outlined in the Machinery's Handbook 32nd Edition.


## Research and Planning 

### Fit Research

The tolerances and clearances were initially derived from the Machinery's Handbook 32nd Edition. The fit was meant to be an RC 2 running and sliding fit which is meant to be a fit for parts that are able to spin but should not run freely. 

The tolerance changed a lot throughout from trial and error and advice from classmates. Particularly a group of classmates who designed a coupon testing a variety of tolerances.

My nominal tolerance changed throughout the process but I eventually settled on a 0.25 inch shaft that had a minimum clearance of 0.2 thousandths of an inch and a max clearance of 0.85 thousandths of an inch. I used the largest clearances I could for my first print and increased the diameter of the hole by the 0.85 thousands of an inch.

However, based on my classmates tests and a failed first print, I would end up increasing the tolerance to 12 thousandths of an inch to ensure sufficient clearance for the fit. 

### SLA Size Change

According to several sources, SLA prints are normally known to shrink about 3% after being fully cured. I tried to account for this in my equations by making my hole and shaft 3% larger. However, further research indicated that the PreForm slicer already accounts for shrinkage. I would end up eventually trying two prints: one with the accounting of shrinkage and one without. 

### Part Drawing

For my design, I didn't have much time so I went very simple. I created a basic mechanism that resembles a switch or a lever, like a light switch. The fit just allows the lever arm to rotate about the axle on the base within the constraints set by the extra walls on the base.

<img width="1675" height="1587" alt="LeverArmSLADrawing" src="https://github.com/user-attachments/assets/8122791c-5b16-41fb-a179-24ec689248c8" />

### RC2 Fit Applications

RC 2 sliding and running fits are the second tightest running sliding fits after RC 1 fits. RC 2 fits, from the description in the Machinery's Handbook, are meant to be for parts that allow movement but are not meant to run freely. This applies mainly to applications that need some movement but aren't spinning fast or need precision and friction to hold in place. Mechanisms that are manually adjusted benefit from RC 2 fits. RC 2 fits can be found in switches for a sliding fit that only moves occasionally, telescoping mechanisms which need precision and don't move a lot, and pulleys or gears that are for manually adjusting systems. The RC 2 fit provides a good middle ground between not allowing parts to move at all and not allowing parts to move too much for more precise or manual applications.

## Iteration 1

### CAD Design

To start the model, I began with the equations I would be using. I parametrically set everything I could, only having four independent variables. These variables were the height, length, width, and clearance. I also included a variable to attempt to account for the shrinkage that multiplied the shaft and hole dimensions by 1.03 or increasing the size by 3%, which was the theorized shrinkage. I used the highest clearance I could and started with dimensions I figured weren't too small and weren't too big. However, I would end up spending a lot of time iterating the dimensions.

<img width="780" height="503" alt="SLAFitScreenshot (15)" src="https://github.com/user-attachments/assets/c1ece5d0-15bd-4438-8bc3-775e76db3a06" />

I kept the whole structure very simple. I started with a rectangle that was extruded to a quarter of the width. 

<img width="960" height="564" alt="SLAFitScreenshot (2)" src="https://github.com/user-attachments/assets/ef890ed4-0003-4bca-b75d-e15d6d0fcb8c" />

<img width="960" height="564" alt="SLAFitScreenshot (4)" src="https://github.com/user-attachments/assets/f6cd2252-2ed5-41f5-8842-f2c7094a0d14" />

<img width="960" height="564" alt="SLAFitScreenshot (5)" src="https://github.com/user-attachments/assets/5b0a2a7f-6a23-4602-8a47-c2852a5ff6fb" />

Then, I created the shaft using the parametric diameter which started at a nominal size of 0.5 inches before clearance and shrinkage. Next, I extruded it the rest of the width, or three quarters of the width. 

<img width="960" height="564" alt="SLAFitScreenshot (6)" src="https://github.com/user-attachments/assets/15944bfd-c37c-43f4-a4de-9a89151db59a" />

<img width="960" height="564" alt="SLAFitScreenshot (7)" src="https://github.com/user-attachments/assets/e9ce78f3-1fbe-4074-9f77-646430da7a46" />

<img width="960" height="564" alt="SLAFitScreenshot (8)" src="https://github.com/user-attachments/assets/81c9c614-790c-4df6-b077-f50740b1830e" />

Next, I made two stoppers for the lever arm on with side of the rectangle and made the thickness of them one tenth of the total length. The walls were extruded to the same length as the cylinder. 

<img width="960" height="564" alt="SLAFitScreenshot (9)" src="https://github.com/user-attachments/assets/c762fc09-899f-4498-8562-c3480def1c87" />

<img width="960" height="564" alt="SLAFitScreenshot (10)" src="https://github.com/user-attachments/assets/876f5e89-2b38-46c5-a50f-4808d1fd051b" />

<img width="960" height="564" alt="SLAFitScreenshot (12)" src="https://github.com/user-attachments/assets/f658db3c-ad16-41a1-acbd-55f16220c9a0" />

The next step was to design the lever arm. I started with a hollow shaft that had an inner diameter the same as the shaft diameter plus the clearance with the shrinkage accounted for. The hole had a 0.1 inch thick rim that would fit around the shaft.

<img width="960" height="564" alt="SLAFitScreenshot (16)" src="https://github.com/user-attachments/assets/b8e8247f-38fe-4688-ad7f-07bf8c82b1f7" />

<img width="960" height="564" alt="SLAFitScreenshot (17)" src="https://github.com/user-attachments/assets/6fa89c09-a745-48ad-97f4-68c80a590b10" />

<img width="960" height="564" alt="SLAFitScreenshot (18)" src="https://github.com/user-attachments/assets/4625725f-7cd3-4f0b-b224-e79c3f7ced8e" />

I decided not to extrude it to the full length of the shaft and instead only to half the width. 
Next, I added a rectangle portion sticking out of it to be the actual switch. I made the length or "height" of this rectangle be the Length of the rectangle. It was then extruded to be the same thickness as the hole.

<img width="960" height="564" alt="SLAFitScreenshot (20)" src="https://github.com/user-attachments/assets/7efe2228-4769-4b0a-9b21-083615eedb39" />

<img width="960" height="564" alt="SLAFitScreenshot (21)" src="https://github.com/user-attachments/assets/b76edd08-1814-478f-8242-a828fc8d3634" />

<img width="960" height="564" alt="SLAFitScreenshot (22)" src="https://github.com/user-attachments/assets/f8d7f5aa-7fdf-4579-a57b-d7280b833583" />

Finally, I created an assembly to see how the parts fit together.

<img width="960" height="564" alt="SLAFitScreenshot (23)" src="https://github.com/user-attachments/assets/2832b82a-f78a-4f77-a1cb-25e8f92c421b" />

The parts fit together nicely and with how I mated the parts, they could even move like a lever.

<img width="960" height="564" alt="SLAFitScreenshot (24)" src="https://github.com/user-attachments/assets/7b22126e-e7b9-4b09-9a72-8839850dee4b" />

<img width="960" height="564" alt="SLAFitScreenshot (25)" src="https://github.com/user-attachments/assets/168c05ea-2fe1-48ec-bdd9-9cc94bbadc13" />

With this design, I moved onto the preprocessing.


### Preprocessing

When I loaded the first designs into the slicer, I realized how large they actually were compared to the bed. I decided to immediately decrease the size of the parts. 

<img width="780" height="503" alt="SLAFitScreenshot (27)" src="https://github.com/user-attachments/assets/a9fa3b5e-1ff0-4860-9bc7-b745c914aceb" />

I decreased the width, height, length, and shaft diameter which necessitated a new clearance. 

<img width="960" height="564" alt="SLAFitScreenshot (29)" src="https://github.com/user-attachments/assets/dc33e415-a72c-4291-9940-ffa576638a13" />

<img width="960" height="564" alt="SLAFitScreenshot (30)" src="https://github.com/user-attachments/assets/6f06b7ed-1796-4a98-b7a2-9a484e6eb886" />

<img width="960" height="564" alt="SLAFitScreenshot (31)" src="https://github.com/user-attachments/assets/5003dbeb-e990-4a98-b17a-d86a8cf3e311" />

Once I had the new sized parts, I started experimenting with different ways to organize the parts and how the time and needed supports changed. 

<img width="960" height="564" alt="SLAFitScreenshot (32)" src="https://github.com/user-attachments/assets/6bb10cc4-9506-4565-8be6-8a378173a127" />

<img width="960" height="564" alt="SLAFitScreenshot (33)" src="https://github.com/user-attachments/assets/a03c0f99-209d-412e-b07b-092e023d2102" />

<img width="960" height="564" alt="SLAFitScreenshot (34)" src="https://github.com/user-attachments/assets/3ee813a1-3ee6-4f36-b649-e57defcac3d5" />

<img width="960" height="564" alt="SLAFitScreenshot (35)" src="https://github.com/user-attachments/assets/fec42bb6-181f-4c8a-9587-9af4e67b95b4" />

I decided on a 30 degree angle for the parts with mini brim and otherwise default settings for wall thickness and supports. However, the print time was still over an hour and I didn't want to wait that long so I went through 6 size iterations to find one that had a more reasonable time to print.

<img width="960" height="564" alt="SLAFitScreenshot (36)" src="https://github.com/user-attachments/assets/53cd6001-db2d-4aa1-9c00-737a32f3b2fe" />

<img width="960" height="564" alt="SLAFitScreenshot (37)" src="https://github.com/user-attachments/assets/6463b399-dbbf-45e1-b3c0-ae5abaa2fbf1" />

<img width="960" height="564" alt="SLAFitScreenshot (39)" src="https://github.com/user-attachments/assets/e7a09509-ed08-42e9-9753-b54dfb540523" />

<img width="960" height="564" alt="SLAFitScreenshot (40)" src="https://github.com/user-attachments/assets/db7e8d65-1f8b-46b0-a040-5d16942f2019" />

<img width="960" height="564" alt="SLAFitScreenshot (41)" src="https://github.com/user-attachments/assets/39a96b3d-780a-4e88-8be8-87fd7c74455d" />

<img width="960" height="564" alt="SLAFitScreenshot (42)" src="https://github.com/user-attachments/assets/6fb6b4ef-98f7-4e3a-8954-7d72c7b1b15d" />

These were the final dimensions I settled on when I decided to give up since the print time was staying very constant around 30 minutes. I primarily tried to get an orientation that was 
close together to save time. And the 30 degree angle gave the model more horizontal width over height which would also make the print go faster. The model was also printed at the lowest resolution layer thickness at 0.100 mm thick per layer. This was also to try and save as much time as possible. 

<img width="780" height="503" alt="SLAFitScreenshot (43)" src="https://github.com/user-attachments/assets/2282804c-7193-478a-867b-c865ec6a2d6b" />

With the final size and orientation, I moved on to actually printing it.


### Printing

The first iteration was printed with V5 gray resin. The print took around 30 minutes and a little under 3 milliliters of total resin. It was printed on the SLA printer named "HallowedDodo." 

<img width="3000" height="4000" alt="SLA-Photo (2)" src="https://github.com/user-attachments/assets/87e432bc-8341-4d50-a3ba-2d71cd837c60" />

<img width="3000" height="4000" alt="SLA-Photo (4)" src="https://github.com/user-attachments/assets/c03a5e4e-0921-4752-823a-f1637e7fd532" />

<img width="3000" height="4000" alt="SLA-Photo (7)" src="https://github.com/user-attachments/assets/a878b1c1-c9d7-4a0d-8caf-4b0f93f63cd6" />

<img width="3000" height="4000" alt="SLA-Photo (9)" src="https://github.com/user-attachments/assets/8afc61dd-cc47-4371-baf5-8d426a91aeb5" />

<img width="3000" height="4000" alt="SLA-Photo (11)" src="https://github.com/user-attachments/assets/99fab60a-897f-4e2e-8150-b0e5b00eaada" />

The final product was very small. The cleaning and curing were not too big of an issue, just a little more time. About 5 minutes for the initial washing and 15 minutes for the curing. The surface finish and quality was good and smooth except for the areas with supports that ended up a little rougher once they were removed. 


### Fit Test

The fit ultimately did not end up working. I could not even force the parts together let alone slide the lever arm. I attempted to file down the shaft but after fifteen minutes, the parts still wouldn't fit together. This made me need to reassess and try printing the model again.

<img width="3000" height="4000" alt="SLA-Photo (11)" src="https://github.com/user-attachments/assets/99fab60a-897f-4e2e-8150-b0e5b00eaada" />

<img width="3000" height="4000" alt="SLA-Photo (12)" src="https://github.com/user-attachments/assets/f2c24a2b-3763-4851-9ffc-8288e198a704" />

<img width="3000" height="4000" alt="SLA-Photo (13)" src="https://github.com/user-attachments/assets/d1cb5780-9588-48b0-99ab-b964a4aa6004" />


## Iteration 2

### CAD Design

For the second iteration, I worked with a classmate who had made a coupon of different clearances in an attempt to figure out a good clearance for parts by testing since the numbers from the Machinery's Handbook were completely unreliable. For the a shaft with a nominal thickness of 0.25 inches, the tested thickness on the coupon was 12 thousands of an inch or 0.012 inches. This was quite an increase from the clearance I took from the Handbook which was 0.00085 inches. With this new number, I updated the dimensions of my model. I also decided to remove the variable accounting for shrinkage since the Preform Slicer claims to already account for it. 

<img width="780" height="503" alt="SLAFitScreenshot (43)" src="https://github.com/user-attachments/assets/83fff890-84f6-48fe-8e67-65ea2af87cfe" />

<img width="780" height="503" alt="SLAFitScreenshot (44)" src="https://github.com/user-attachments/assets/02d78359-6ba7-4e78-b3cf-9a25e5e73ce8" />

With these final dimensions and clearances, I tried printing it again. 


### Preprocessing

For the second iteration, I laid the parts parallel to the build plate, which saved about 10 minutes of print time bring it down to 24 minutes. I left the supports and wall thickness on default settings and used a mix of the auto-layout tool and manually moving the parts to try and find a decent configuration which made them close enough together. I used the "mini brim" setting again instead of a full brim, even though it didn't save much time, it saved about 0.5 ml of resin. 

<img width="960" height="564" alt="SLAFitScreenshot (45)" src="https://github.com/user-attachments/assets/bff5434b-119a-4875-ba78-ae15184c9412" />

<img width="960" height="564" alt="SLAFitScreenshot (46)" src="https://github.com/user-attachments/assets/4fc2e613-93ee-4f69-8272-51b1b3625cef" />

<img width="960" height="564" alt="SLAFitScreenshot (47)" src="https://github.com/user-attachments/assets/a175a6c1-341f-4a40-a031-f1501ccf5066" />

I once again chose the smallest layer thickness of 0.100 mm for time and since the model really didn't need to be detailed. 

### Printing

For the second iteration print, the model was printed on the SLA print named "MaturelImpala." It was printed out of clear V5 resin with a print time of about 24 minutes. 

<img width="3000" height="4000" alt="SLA-Photo (17)" src="https://github.com/user-attachments/assets/bf15f052-57ed-4985-901a-46e42a5cea56" />

<img width="4000" height="3000" alt="SLA-Photo (20)" src="https://github.com/user-attachments/assets/02825ac2-6598-4984-9ae3-ede6b75dd599" />

<img width="4000" height="3000" alt="SLA-Photo (23)" src="https://github.com/user-attachments/assets/fe5fd8a6-a198-4bc5-8d10-22dd439f849b" />

The print turned out good again. I got a little worried when the model first came out of the resin because it was hard to tell whether it was actually there and complete because of the clear resin. The clear resin looked very nice and clear initially, but over time and with curing and processing, it became more cloudy and less transparent. The surface quality was good except for the parts the supports were attached to. I'm not sure if I was less careful with removing the supports the second time but the surface came out very rough and the supports took some extra material with it from the main body. 

But with the supports removed after cleaning the model, the curing was the same taking 15 minutes to fully cure. 

<img width="1631" height="1630" alt="SLA-Photo (26) -2" src="https://github.com/user-attachments/assets/40f230c6-272e-42dd-907f-1fe6db910220" />


### Fit Test

Once the post-processing was finish, I finally tried putting the parts together. 

<img width="1631" height="1630" alt="SLA-Photo (26) -2" src="https://github.com/user-attachments/assets/32b4fd37-353e-492a-9b4c-2416f143269c" />

<img width="4000" height="3000" alt="SLA-Photo (27)" src="https://github.com/user-attachments/assets/203a3ebf-ae03-4273-bd3b-e1fbcd990155" />

The new clearance worked perfectly and the parts were able to slide together fairly easily. The lever arm could turn around the axle but wasn't too lose that it would wildly spin. 

<img width="4000" height="3000" alt="SLA-Photo (28)" src="https://github.com/user-attachments/assets/2c4b890f-1b97-4e90-a9e5-2feeb22db120" />

<img width="4000" height="3000" alt="SLA-Photo (29)" src="https://github.com/user-attachments/assets/531a5d87-c3d9-4c10-b361-25565e55e6f0" />

Measuring the hole and shaft with a caliper gave a dimension for the hole of 0.252 inches and the shaft 0.241 inches. Subtracting these measurements gives a clearance of 0.011 inches. 

<img width="3000" height="4000" alt="SLA-Photo (30)" src="https://github.com/user-attachments/assets/75423f61-f500-4ec1-a279-09459dbafdd3" />

<img width="3000" height="4000" alt="SLA-Photo (33)" src="https://github.com/user-attachments/assets/59fc72e1-e5f3-4b1b-bcb0-046e5e7a2ef3" />

A clearance of 0.011 inches is technically not an RC 2 sliding fit for a nominal 0.25 inch shaft since the clearance ranges from 0.2 to 0.85 thousandths of an inch according to the Machinery's Handbook. However, the dimensions and clearances are meant for metals and not anything related to resin and additive manufacturing. And the fit I ended up with acts like I would expect an RC 2 sliding fit to act, given the description. 


## Lessons Learned

This assignment was more annoying than previous assignments. There was little or no guidance on how to achieve a proper fit since the numbers in the Machinery's Handbook are meant for metals. This gave me and my classmates very little to work with especially considering the conflicting information that we found during our research. If it wasn't for my classmate who made the fit coupon, I doubt I would have been able to make a working fit. I know now that the only way to really figure out the appropriate clearances for an SLA print are to test. There really is no other reliable way since every printer and resin is different. I also learned about the resin printing process, cleaning, and curing. And how SLA is more work than FDM. The differences in print times were crazy to me. To print my model on an FDM printer likely would've taken less than 5 minutes without needing any curing or cleaning. This makes SLA an even more niche manufacturing method for very specialized parts that only a resin like material is suited for.

**Time Spent: ** 8 Hours

### CAD File Downloads

[Lever Base Solidworks Model](SLALeverBase7.SLDPRT)

[Lever Base STL](SLALeverBase8.STL)

[Lever Arm Solidworks Model](SLALeverArm5.SLDPRT)

[Lever Arm STL](SLALeverArm8.STL)

[Lever Assembly](SLALeverAssem3.SLDASM)


### Resources

Machinery's Handbook 32nd Edition

[One Common Failure for SLA: The Material Deformation](https://facfox.com/docs/kb/one-common-failure-for-sla-the-material-deformation)

[Getting Perfectly Crisp and Dimensionally Accurate 3D Prints on a Resin Printer: Fighting Resin Shrinkage and Exposure Bleeding](https://blog.honzamrazek.cz/2022/06/getting-perfectly-crisp-and-dimensionally-accurate-3d-prints-on-a-resin-printer-fighting-resin-shrinkage-and-exposure-bleeding/)

[Warping (SLA)](https://formlabs.com/support/Warping-SLA/)
