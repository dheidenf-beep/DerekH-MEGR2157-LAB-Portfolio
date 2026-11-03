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

**_INSERT DREWING_**

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

I decided on a 30 degree angle for the parts with mini brim and otherwise default settings. However, the print time was still over an hour and I didn't want to wait that long so I went through 6 size iterations to find one that had a more reasonable time to print.

<img width="960" height="564" alt="SLAFitScreenshot (36)" src="https://github.com/user-attachments/assets/53cd6001-db2d-4aa1-9c00-737a32f3b2fe" />

<img width="960" height="564" alt="SLAFitScreenshot (37)" src="https://github.com/user-attachments/assets/6463b399-dbbf-45e1-b3c0-ae5abaa2fbf1" />

<img width="960" height="564" alt="SLAFitScreenshot (39)" src="https://github.com/user-attachments/assets/e7a09509-ed08-42e9-9753-b54dfb540523" />

<img width="960" height="564" alt="SLAFitScreenshot (40)" src="https://github.com/user-attachments/assets/db7e8d65-1f8b-46b0-a040-5d16942f2019" />

<img width="960" height="564" alt="SLAFitScreenshot (41)" src="https://github.com/user-attachments/assets/39a96b3d-780a-4e88-8be8-87fd7c74455d" />

<img width="960" height="564" alt="SLAFitScreenshot (42)" src="https://github.com/user-attachments/assets/6fb6b4ef-98f7-4e3a-8954-7d72c7b1b15d" />

These were the final dimensions I settled on when I decided to give up since the print time was staying very constant around 30 minutes. Better than an hour or more, however. 

<img width="780" height="503" alt="SLAFitScreenshot (43)" src="https://github.com/user-attachments/assets/2282804c-7193-478a-867b-c865ec6a2d6b" />

With the final size and orientation, I moved on to actually printing it.


### Printing

The first iteration was printed with gray resin. The print took around 30 minutes and a little under 3 milliliters of total resin. The final product was very small. 


The fit ultimately did not end up working. I could not even force the parts together let alone slide the lever arm. I attempted to file down the shaft but after fifteen minutes, the parts still wouldn't fit together. This made me need to reassess and try printing the model again.


## Iteration 2

### CAD Design



### Preprocessing


### Printing


## Lessons Learned

**Time Spent: **

### CAD File Downloads

[Lever Base]()

[Lever Arm]()

[Lever Assembly]()

### Resources

