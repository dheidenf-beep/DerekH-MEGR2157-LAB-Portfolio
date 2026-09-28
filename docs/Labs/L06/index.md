# A6 – Design Fits For an Artifact

## Objective

The objective of lab 6 was to design a snap fit based on the parameters of a real object, in this case an old electrical component. The object I chose was an old, broken decora light switch. 

![Switch Image](SwitchImg2.jpg)

The assignment required the use of a caliper to take measurements of the chosen part and design the snap fit using those measurements. 


## Measurements

The first step in designing the snap fit for the chosen part was to a caliper to take measurements of the part. I took measurements of practically every part of the switch I thought would be useful and took images of the measurements to save time and not mix up the numbers if I wrote them down.

Initially, I planned on creating a snap fit for the metal yoke so I started with those measurements.

![Measure 1](measure1.jpg)

![Measure 2](measure2.jpg)

![Measure 3](measure3.jpg)

![Measure 4](measure4.jpg)

![Measure 6](measure6.jpg)

![Measure 7](measure7.jpg)

![Measure 8](measure8.jpg)

However, the yoke of the switch is not very straight and it is also very thin, which doesn't give a lot for a snap fit to clip onto. So instead, I decided to make something clip on the main body on the little lip that is present on both sides. This meant I needed to take more measurements of the body of the switch.

![Measure 11](measure11.jpg)

![Measure 12](measure12.jpg)

![Measure 14](measure14.jpg)

![Measure 15](measure15.jpg)

![Measure 16](measure16.jpg)

![Measure 20](measure20.jpg)

![Measure 21](measure21.jpg)

![Measure 22](measure22.jpg)

With all of the measurements taken, I could draw a picture and determine the dimensions I needed for my CAD model.

## Attempt 1

### Attempt 1 Drawing

Once I had the measurements, I could draw a picture. I drew a front and side view of the outlet to give me a better idea of the dimensions. 

**_SWITCH DRTAWINFG ONE_**

For my snap fit, I wanted it to go from the back of the outlet, opposite of the switch side, and hook on to the ledges protruding out on both sides. Due to the shape of the switch, I couldn't directly measure the distance from the ledge to the bottom of the switch. This meant I had to use math to subtract the other distances I didn't need. On the bottom of the outlet, there are these parts or notches that stick out at the ends, which I didn't want the snap fit to go over. This meant I had to make it a smaller width to not collide with the notches. There is also a part that sticks up on the ledges in the middle that also made me reduce the width further. For the lip width, I ended up with a measurement of 0.1365 inches, the length was 1.229 inches, and the width ended up being 0.703 inches.

Using these measurements I knew the inside distance from the lip of the snap fit to the bottom and the width of the inside of the snap fit along with the needed deflection and thickness. I decided to calculate the height and size of the area of the lips on the snap fit using the beam bending stress and deflection equations. I used similar forces to the previous lab, but reduced them some due to how rigid my last snap fit was.

For this snap fit, I chose a transverse force of 0.25 lbf and a shear force of 1.5 lbf using a safety factor of 3 and PLA as my material.

**_MATH_**

For the height, I got a larger height requirement for the stiffness equation of 0.902 inches which is what I went with. For the length the lips needed to be, I solved for 0.139 inches based on the shear force I chose.

I didn't use any tolerances. I used the exact measurements I got. I figured I would test it and if the exact measurements didn't work, I could reevaluate. When I was measuring with the caliper, I would always round up if the dial looked as though it was between two numbers. I figured this would give me the gap that was necessary for the part to fit around the switch snugly. 

With the measurements acquired, I had everything I needed to know to start modeling.


### Attempt 1 CAD

For the CAD modeling, I reused the flexure piece of my previous snap fit. 

![Switch Snap Fit 1](SwitchFit1.png)

However, when I tried to switch from metric to imperial units, the model did not like it.

![Switch Snap Fit 2](SwitchFit2.png)

![Switch Snap Fit 3](SwitchFit3.png)

The snap fit lost the fillets which I would forget to put back on the final product.

To make it as easy as possible in case I made a mistake, I put every measurement and equation into Solidworks

![Attempt 1 Equations](Attempt1Eqns.png)

This turned out to be immediately helpful because I made a small error when calculating my height which the Solidworks equation caught.

I then just had to change all of the measurements to use the new constraints.

![Switch Snap Fit 4](SwitchFit4.png)

![Switch Snap Fit 5](SwitchFit5.png)

I realized I needed to invert the direction of the lips so the snap fit would actually hook on.

![Switch Snap Fit 6](SwitchFit6.png)

![Switch Snap Fit 7](SwitchFit7.png)

I made the slope of the lip determined by x or the length of the lip in case the math changed.

![Switch Snap Fit 8](SwitchFit8.png)

Here, I forgot I already reduced the thickness to account for the notches in the bottom so I ended up accounted for them again which made my print less thick, which wasn't necessarily a bad thing.

![Attempt 1 Equations 2](Attempt1Eqns2.png)

With that done, all of the parameters were in place and CAD model was finished once it was extruded.

![Switch Snap Fit 9](SwitchFit9.png)

![Switch Snap Fit 10](SwitchFit10.png)

![Switch Snap Fit 11](SwitchFit11.png)

Next, I could move on to the preprocessing and print for the first attempt.


### Attempt 1 Preprocessing

For the preprocessing of the model in the Prusa Slicer, I didn't alter a whole lot. I reduced the infill to 10% but kept with the standard grid pattern because it worked for my last snap fit. The build orientation utilized the flat space to reduce time and the layer lines were parallel to the force that the snap fit may experience. No supports were necessary and the print time was only about 16 minutes. I did not need to alter the size or change any scaling as that would screw up the measurements. I kept the wall thickness at the default 2 layers because I didn't want the part to completely fall apart. 

![Attempt 1 Preprocessing 1](Attempt1Pre1.png)

![Attempt 1 Preprocessing 2](Attempt1Pre2.png)

![Attempt 1 Preprocessing 3](Attempt1Pre3.png)

With the preprocessing and slicing finished, I started printing the model.


### Attempt 1 Printing

The model was printed on printer 3 in the Duke Centennial print lab. I tried printing it once on another printer but the filament in that printer wasn't loaded. Apart from that, there weren't any issues with the print.

![Attempt 1 Print Image 1](Attempt1Print1.jpg)

![Attempt 1 Print Image 2](Attempt1Print2.jpg)

![Attempt 1 Print Image 3](Attempt1Print3.jpg)

![Attempt 1 Print Image 4](Attempt1Print4.jpg)

<video width="100%" controls>
  <source src="Attempt1Video1.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

![Attempt 1 Print Image 5](Attempt1Print5.jpg)

![Attempt 1 Print Image 7](Attempt1Print7.jpg)

![Attempt 1 Print Image 8](Attempt1Print8.jpg)

![Attempt 1 Print Image 9](Attempt1Print9.jpg)

<video width="100%" controls>
  <source src="Attempt1Video2.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

The print came out good. There weren't any issues with it visually. 


### Attempt 1 Evaluation

Once the print finished, I test it on the switch. The snap fit wasn't very flexible still but it managed to snap onto the switch.

![Attempt 1 Evaluate 1](Attempt1Evaluate1.jpg)

![Attempt 1 Evaluate 2](Attempt1Evaluate2.jpg)

However, even though the print width and lips of the snap fit worked great and it didn't hit the protrusions on the back of the switch, there was an issue with the depth of it and it didn't quite touch the switch like I wanted it to.

![Attempt 1 Evaluate 3](Attempt1Evaluate3.jpg)

This caused the snap fit to just fall off the switch. Since it wasn't really holding on, that meant I had to edit it. I rechecked my math and tried again to figure out where I went wrong.


## Attempt 2


### Attempt 2 Drawing

For the second attempt, I started back at the measurements. The width and dimensions of the lips of the snap fit were fine so that meant there was something wrong with the just the depth or length of the snap fit. I redrew the switch and redid the math for the length calculation.

**_OINSERT DRAWING 2_**

It turns out, the 1.299 inches I had used for the length was the length of the whole switch, not just the distance from the ledge to the bottom, hence why it was too long. Redoing the calculation cave me a new length of 0.866 inches. I then plugged this number directly into solidworks to get the new numbers automatically.


### Attempt 2 CAD Modeling

Once I had the corrected length, it was very easy to correct the model since everything was done parametriclly. I just inserted the new number and Solidworks did everything else for me. 

![Attempt 2 Equations 1](Attempt2Eqns1.png)

* Before

![Attempt 2 Equations 2](Attempt2Eqns2.png)

* After

![Attempt 2 Model](Attempt2CAD.png)

Once the model updated with the new height calculations, I could immediate start preprocessing again.


### Attempt 2 Preprocessing

I used the same exact parameters for Attempt 2 as I did Attempt 1. I considered lowering the infill more but decided against it. The orientation and everything was the same as Attempt 1. The time ended up being 2 minutes shorter at 14 minutes instead of 16 due to the lost volume from shortening the length.

![Attempt 2 Sliced](Attempt2Slice.png)

![Attempt 2 Sliced 2](Attempt2Slice2.png)


### Attempt 2 Printing

The same printer, printer 3, was used to print attempt 2. The printing went smoothly and was nearly identical to attempt 1. 

![Attempt 2 Printing 1](Attempt2Print1.jpg)

![Attempt 2 Printing 2](Attempt2Print2.jpg)

![Attempt 2 Printing 3](Attempt2Print3.jpg)

![Attempt 2 Printing 4](Attempt2Print4.jpg)

<video width="100%" controls>
  <source src="Attempt2Video.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

The model printed with no issues. 


### Attempt 2 Evaluation

Once the second attempt model was finished printing, I tested snapping it on the switch. 

![Attempt 2 Evaluate 1](Attempt2Evaluate1.jpg)

This time, The length was correct and the snap fit snapped on to the switch with a very sung fit.

![Attempt 2 Evaluate 2](Attempt2Evaluate2.jpg)

![Attempt 2 Evaluate 3](Attempt2Evaluate3.jpg)

![Attempt 2 Evaluate 4](Attempt2Evaluate4.jpg)

The snap fit could support the switch and wasn't able to slide off, which was what I was looking for. I tested taking it on and off several times and it was very consistent though still very rigid. Overall, I was very satisfied with the end result.


## Lessons Learned

The primary lesson I learned for this lab was using a caliper and determining the measurements. Due to the weird shape of the switch I chose, I wasn't able to directly measure all of the distances I needed. This led me to measuring the full length and the distances I could to certain components, and then subtracting the distances to get the one I wanted. It took a lot of drawing, measuring, and trial and error but I eventually figured it out. I have also been trying to adapt using parametric equations and constraints in Solidworks for every measurement which has been cutting down on the CAD model finagling substantially and I will continue to do so for future CAD models due to how much easier it makes it.

[Attempt 2 Solidworks File Download](Snapfit-Flexure-Outlet2.SLDPRT)

[Attempt 2 STL Download](Snapfit-Flexure-Outlet2.STL)

Time Spent: 5 Hours


## Resources

Machinery's Handbook 32nd Edition

[Matweb Material Properties of PLA](https://www.matweb.com/search/DataSheet.aspx?MatGUID=ab96a4c0655c4018a8785ac4031b9278&ckck=1)

Solidworks

