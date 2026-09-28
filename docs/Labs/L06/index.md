# A6 – Design Fits For an Artifact

## Objective

The objective of lab 6 was to design a snap fit based on the parameters of a real object, in this case an old electrical component. The object I chose was an old, broken decora light switch. 

**_INSRT IMG OF SWITCH_**

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

### Drawing

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

![Switch Snap Fit 1](SwitchFit1.jpg)

However, when I tried to switch from metric to imperial units, the model did not like it.

![Switch Snap Fit 2](SwitchFit2.jpg)

![Switch Snap Fit 3](SwitchFit3.jpg)

The snap fit lost the fillets which I would forget to put back on the final product.

To make it as easy as possible in case I made a mistake, I put every measurement and equation into Solidworks

![Attempt 1 Equations](Attempt1Eqns.jpg)

This turned out to be immediately helpful because I made a small error when calculating my height which the Solidworks equation caught.

I then just had to change all of the measurements to use the new constraints.

![Switch Snap Fit 4](SwitchFit4.jpg)

![Switch Snap Fit 5](SwitchFit5.jpg)

I realized I needed to invert the direction of the lips so the snap fit would actually hook on.

![Switch Snap Fit 6](SwitchFit6.jpg)

![Switch Snap Fit 7](SwitchFit7.jpg)

I made the slope of the lip determined by x or the length of the lip in case the math changed.

![Switch Snap Fit 8](SwitchFit8.jpg)

Here, I forgot I already reduced the thickness to account for the notches in the bottom so I ended up accounted for them again which made my print less thick, which wasn't necessarily a bad thing.

![Attempt 1 Equations 2](Attempt1Eqns2.jpg)

With that done, all of the parameters were in place and CAD model was finished once it was extruded.

![Switch Snap Fit 9](SwitchFit9.jpg)

![Switch Snap Fit 10](SwitchFit10.jpg)

![Switch Snap Fit 11](SwitchFit11.jpg)

Next, I could move on to the preprocessing and print for the first attempt.


### Attempt 1 Preprocessing

For the preprocessing of the model, I didn't alter a whole lot. I reduced the infill to 10% but kept with the standard grid pattern because it worked for my last snap fit. No supports were necessary and the print time was only about 16 minutes. I did not need to alter the size or change any scaling as that would screw up the measurements. I kept the wall thickness at the default 2 layers because I didn't want the part to completely fall apart. 

![Attempt 1 Preprocessing 1](Attempt1Pre1.jpg)

![Attempt 1 Preprocessing 2](Attempt1Pre2.jpg)

![Attempt 1 Preprocessing 3](Attempt1Pre3.jpg)

With the preprocessing and slicing finished, I started printing the model.


### Attempt 1 Printing




### Attempt 1 Evaluation


## Decide


## Lessons Learned

