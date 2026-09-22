# A5 – Design a Snap fit

## Objective

The goal of the fifth lab was to design mathematically and 3D print a snap fit. The constraints for the snap fit was that it needed to be able to bend given a transverse force at the end of the flexure component of between 0.25 lbf and 5 lbf. The flexure is treated as a cantilever beam in this case with the force assumed to be at the free end of the flexure. The snap fit is required to hold a maximum axial force between 5 - 10 lbf. The shear stress from the axial load and the normal stress from the transverse load must not exceed the yield strength and ultimate shear strength of the material. The stress will be calculated using a safety factor of 3.5. 


## Research


### Printing Orientation



### Material Properties

The material I chose for the snap fit was PLA. Using the [data sheet from the MATWEB website](https://www.matweb.com/search/DataSheet.aspx?MatGUID=ab96a4c0655c4018a8785ac4031b9278&ckck=1), I used the lowest values for the yield strength, elastic modulus, and ultimate shear strength. This gave me a value of 8 MPa for the yield strength, 0.00232 GPa or 2.32 MPa for the elastic modulus, and 0.160 MPa for the ultimate shear strength. I calculated the maximum safe values for the yield strength and ultimate shear strength using the safety factor of 3.5. This gave me maximum values of 2.28 MPa for the maximum stress and 0.046 MPa for the ultimate shear strength. I used the beam bending equations for deformation and stress in the Machinery's Handbook.

**_INSRT SF WORK_**


## Calculations and CAD Parameters

Before performing the calculations, I drew a lot of different versions of the snap fit to get an idea of sizing. And I also forgot I needed to use the deflection equation to find the length.

**_INSRT INITIAL DREWINGS_**

To start the calculations, I first solved the deflection equation for length. I also solved the maximum stress equation, plugging in the moment of inertia and the distance from the edges to neutral axis. After that, I solved for all the maximum values given the 3.5 safety factor.

**_INSRT PG 1 WRK_**

I chose a force of 2 lbf for my transverse force which I converted to 8.9 newtons. I chose an axial or shear force as 5lbf or 22.24 newtons. I initially chose the base of the flexure prongs to be 10mm and the height to be 5mm with a deflection of 5mm. I then solved for the length.

**_Initial Len Wokr_**

Using the Numbers I had, I calculated a length of 7.43mm, which was very small for the length of the prongs, especially since the height (thickness) was 5mm. I calculated the stress and it was under the maximum but I didn't want the length to be that short, so I redid the calculations this time with an increase b, h, and deflection values. 

**_2nd try len work_**

This second length the I calculated was 23.53 mm, which was better. It was under the maximum stress. However, for the shear stress value of the ledges on the prongs that hold the pieces together, the shear stress was very large which was making the length (x) that the clips needed to be very large. Once the length of clips started approaching 10mm, which was about half the length, I stopped and recalculated the length. This time, increasing the height once again

**_3rd try len work_**

For the third try, I achieved a length of 35.30 mm and a needed clip length of 13 mm. I felt mostly satisfied with these measurements. Although the snap fit would be very large.

**_Last Snap Fit Drewing_**

I kept these numbers and moved into parametrically designing the snap fit components. 


## Snapfit Iteration 1

For the first iteration, I used Solidworks parameters and equations to model the length, height, and base, using normal dimensioning for the rest of the measurements. 

![Solidworks Eqns 1](SolidworksEqns1.png)


### Iteration 1 CAD Modeling

#### Iteration 1 Clip Modeling

To start, I began with the clip part of the snap fit or the "receiver." I began with a basic sketch and took advantage of symmetry to try and make the process move faster.

![Iteration1 1](SnapfitIteration1-1.png)

![Iteration1 2](SnapfitIteration1-2.png)

* I set the edge thickness to parametrically be the height and the length of the the whole clip to be the calculated length plus the height. 

![Iteration1 3](SnapfitIteration1-3.png)

* I then extruded the sketch, setting the extrusion thickness to be the b or base value.

![Iteration1 4](SnapfitIteration1-4.png)

![Iteration1 5](SnapfitIteration1-5.png)

* To finish the clip, I filleted all of the corners to prevent stress concentrations. I had to use different kinds of fillets because sometimes edges would be too close together and the fillets would try and overlap, causing errors.

![Iteration1 6](SnapfitIteration1-6.png)

![Iteration1 7](SnapfitIteration1-7.png)

![Iteration1 8](SnapfitIteration1-8.png)

![Iteration1 9](SnapfitIteration1-9.png)

![Iteration1 10](SnapfitIteration1-10.png)

![Iteration1 11](SnapfitIteration1-11.png)

![Iteration1 12](SnapfitIteration1-12.png)

#### Iteration 1 Flexure Modeling

* I used the "export equations" feature to quickly move the equations into the flexure 3D print file.

![Iteration1 13](SnapfitIteration1-13.png)

* To save time, I once again utilized symmetry and took a very similar design approach with the flexure that I did with the clip.

![Iteration1 14](SnapfitIteration1-14.png)

![Iteration1 15](SnapfitIteration1-15.png)

* I once again parametetrically set the height values and the length value.

![Iteration1 16](SnapfitIteration1-16.png)

![Iteration1 17](SnapfitIteration1-17.png)

* Once I finished the sketch, I extruded the sketch and set the thickness to be the base value.

![Iteration1 18](SnapfitIteration1-18.png)

![Iteration1 19](SnapfitIteration1-19.png)

* After extruding the sketch, I once again filleted all of the sharp corners.

![Iteration1 20](SnapfitIteration1-20.png)

![Iteration1 21](SnapfitIteration1-21.png)

![Iteration1 22](SnapfitIteration1-22.png)

![Iteration1 23](SnapfitIteration1-23.png)

* To determine of my models seemed reasonable and would work with each other, I put to two pieces in an assembly.

![Iteration1 24](SnapfitIteration1-24.png)

* This turned out to be a very good idea because the clip was too short vertically to fit the flexure.

![Iteration1 25](SnapfitIteration1-25.png)

* This meant I needed to iterate the measurements on the clip to get it to fit the flexure.

![Iteration1 26](SnapfitIteration1-26.png)

* I used the flexure measurements as reference.

![Iteration1 27](SnapfitIteration1-27.png)

![Iteration1 28](SnapfitIteration1-28.png)

![Iteration1 29](SnapfitIteration1-29.png)

![Iteration1 30](SnapfitIteration1-30.png)

![Iteration1 31](SnapfitIteration1-31.png)

However, once I had the pieces assemble, I became dissatisfied with the length again. There wasn't any space to get your fingers in to be able to push down on the flexure to get it out of the clip.

So, I increased the base from 20mm to 30mm.

![SolidworksEqns2](SolidworksEqns2.png)

This change increased the length substantially from 35.30mm to 53.88 mm.

![Iteration1 32](SnapfitIteration1-32.png)

* However, this meant I had to heavily alter the clip as well.

![Iteration1 33](SnapfitIteration1-33.png)

* I increased the height so it would be able to fit the larger clip.

![Iteration1 34](SnapfitIteration1-34.png)

![Iteration1 35](SnapfitIteration1-35.png)

I decided to load the parts into the Prusa Slicer to get an idea of the scale and it was immense.

![Iteration1 36](SnapfitIteration1-36.png)

This was way too large for a snap fit. I decided to drop the transverse force from 2 lbf to the smallest value of 0.25 lbf. Converting to newtons gave a new force of 1.112055 N. This allowed me to drastically shrink the proportions of the models. I returned the height to 10 mm and base to 20 mm.

![SolidworksEqns3](SolidworksEqns3.png)

![Iteration1 37](SnapfitIteration1-37.png)

![Iteration1 38](SnapfitIteration1-38.png)

* At this point, I began making more dimensions based on the equation parameters.
* I set the height of the clip to be a function of h, which I would later iterate on further.

![Iteration1 39](SnapfitIteration1-39.png)

![Iteration1 40](SnapfitIteration1-40.png)

![Iteration1 41](SnapfitIteration1-41.png)

![Iteration1 42](SnapfitIteration1-42.png)

* Here I changed the dimension from being the height of the whole clip to the distance between the clips.

![Iteration1 43](SnapfitIteration1-43.png)

![Iteration1 44](SnapfitIteration1-44.png)

![Iteration1 45](SnapfitIteration1-45.png)

* I decided to decrease the internal length of the clip because it did not need to be as long as the whole length of the flexure.

![Iteration1 46](SnapfitIteration1-46.png)

![Iteration1 47](SnapfitIteration1-47.png)

![Iteration1 48](SnapfitIteration1-48.png)

To finish the clip, I needed borders so that the flexure wouldn't fall out. I first increase the thickness of the flexure to be 1 plus the base value to provide some clearence. Than, I made two identical rectangles on the outside edges.

![Iteration1 49](SnapfitIteration1-49.png)

![Iteration1 50](SnapfitIteration1-50.png)

![Iteration1 51](SnapfitIteration1-51.png)

* I made the rectangles go from the center point of the clip to the point when the flat edge tapers off.
* I didn't extrude the edges very far, only 5 mm.

* I did also fillet the edges on the rectangle to prevent stress concentrations.

![Iteration1 52](SnapfitIteration1-52.png)

![Iteration1 53](SnapfitIteration1-53.png)

![Iteration1 54](SnapfitIteration1-54.png)

![Iteration1 55](SnapfitIteration1-55.png)

* I mirrored the rectangle to the other side.

![Iteration1 56](SnapfitIteration1-56.png)


The Completed Clip and Flexure:

![Iteration1 57](SnapfitIteration1-57.png)

![Iteration1 58](SnapfitIteration1-58.png)

![Iteration1 59](SnapfitIteration1-59.png)

With the Snap fit pieces modeled, I moved into properly preprocessing the models for printing.


### Iteration 1 Preprocessing

For the printing of the first iteration of the Snap fit model, I didn't change the parameters in the Prusa Slicer that much. 

![Iteration1 60](SnapfitIteration1-60.png)

For the infill, I kept it at the base 15%. I did change the infill pattern to be triangular because I figured some stability would be good. However, I wasn't sure how it would affect the flexibility. I kept the outer wall parameter at 2 outer perimeters because it was the recommended minimum in the Prusa Slicer and I didn't want to risk the model falling apart from having just one outer perimeter. To speed up the print a bit, I also switched from the "0.15 mm BALANCED" mode to the "0.20 mm SPEED" mode. This reduced the printing to from 2 hours 42 minutes to an hour and 34 minutes. The clip also required supports. I used organic supports and left the slicer to auto select where supports were needed.

Originally, I wanted to print the clip facing upwards to reduce the amount of supports needed. 

![Iteration1 61](SnapfitIteration1-61.png)

But I quickly realized that this would cause the axial load to be directly pulling on the seams of the clip which are the weakest part of FDM prints. To fix this, I turned the clip 90 degrees, which required more supports but meant the axial load would be acting parallel to the seams of the clip, which is the stronger direction of FDM prints.

![Iteration1 62](SnapfitIteration1-62.png)

With all the parameters set, I got started printing the model.


### Iteration 1 Printing




### Iteration 1 Evaluation




## Snapfit Iteration 2

Following the failure of the first iteration, I quickly got to work on a second iteration.

I was confused as to why the lengths of the flexure felt short. I double checked my math several times and that I was using the same equations but I didn't find any errors. 

Instead, I used the new force I had settled on of 1.112055 newtons and lowered the deflection substantially from 10 mm to 3 mm. 

I mostly found my numbers using Solidworks equations but I verified the work with my final numbers on paper. 

**_FINAL CLAC WRK_**

The new calculated work came out to be 31.51 mm.

### Iteration 2 CAD Modeling

For the new iteration, I changed the base to be 20 mm, the height to be 10 mm, and the deflection to 3 mm.

![SolidworksEqns4](SolidworksEqns4.png)

I also added a new parameter called x_min which calculated the minimum length that the clips on the flexure would need to be to be able to withstand the shear stress. I used this to parametrically determine the length of the clips on both the flexure and clip. I added an extra 0.5 mm to stay a little below the maximum safe shear stress.

![Iteration2 1](SnapfitIteration2-1.png)

* I modeled the length of the clip to be the calculated length plus 3 mm to give extra space to the flexure.

![Iteration2 2](SnapfitIteration2-2.png)

* On the flexure, I did the same. I used the x_min plus 0.5 to determine the length of the clips and the deformation value to drive the height of the clips on both parts.

![Iteration2 3](SnapfitIteration2-3.png)

* I set the distance between the prongs on the flexure to be 2 times the deflection value plus the value of h to give plenty of space for the flexure to bend.

![Iteration2 4](SnapfitIteration2-4.png)

* I used the same process on the clip to determine the distance between the clips.

![Iteration2 5](SnapfitIteration2-5.png)

![Iteration2 6](SnapfitIteration2-6.png)

![Iteration2 7](SnapfitIteration2-7.png)

* Finally I filleted both parts and stuck them in an assembly to make sure they fit.

![Iteration2 8](SnapfitIteration2-8.png)

![Iteration2 9](SnapfitIteration2-9.png)

![Iteration2 10](SnapfitIteration2-10.png)

* The final task was to put back on the walls of the clip. I repeated the same method for iteration 2 as I did iteration 1.

![Iteration2 11](SnapfitIteration2-11.png)

![Iteration2 12](SnapfitIteration2-12.png)

* I extruded the walls to only be 3 mm thick since the whole assembly was smaller.

![Iteration2 13](SnapfitIteration2-13.png)

* I made the thickness of the clip be the base plus 2 mm to leave plenty of space for the flexure.

![Iteration2 14](SnapfitIteration2-14.png)

![Iteration2 15](SnapfitIteration2-15.png)

![Iteration2 16](SnapfitIteration2-16.png)

![Iteration2 17](SnapfitIteration2-17.png)

![Iteration2 18](SnapfitIteration2-18.png)

With iteration 2 modeled, I once again moved into preprocessing it for printing.


### Iteration 2 Preprocessing

The preprocessing for iteration 2 was mostly the same as for iteration 1. The only changes made were changing the infill percentage from 15% down to 10% and keeping the infill as the grid pattern. The thought process behind this choice was to have more air gaps and a hopefully more flexible infill.

Every other parameter in regards to walls or supports were the same.

![Iteration2 19](SnapfitIteration2-19.png)

![Iteration2 20](SnapfitIteration2-20.png)

The print time for iteration 2 was about half as much as for iteration 1 at 1 hour and 8 minutes.


### Iteration 2 Printing




### Iteration 2 Evaluation



## Lessons Learned



* [Snapfit Iteration 2 Clip Download](Snapfit-Clip-5-Walls.SLDPRT)

* [Snapfit Iteration 2 Flexure Download](Snapfit-Flexure-4.SLDPRT)


* [STL Snapfit Iteration 2 Clip Download](Snapfit-Clip-5-Walls.STL)

* [STL Snapfit Iteration 2 Flexure Download](Snapfit-Flexure-4.STL)


## Resources

Machinery's Handbook 32nd Edition

