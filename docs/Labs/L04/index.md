# A4 – Benchmark a Parameter

## Objective

The goal of the fourth lab was to design a CAD model to test a parameter and the limits of the Prusa Core One 3D Printers in the Duke Centennial 3D lab. 

I chose to design a test for the limits of embossing or embedding text into a flat 3D print. Testing the width of the embossing seemed more feasible if I wanted to find the lowest limit, so that is what I tested.

## Recommended Text Embossing Limits

I used the ProtoLabs Design Rules for 3D printing documentation to retrieve my numbers for the limits of embossing or engraving details into a 3D print. 

**_INSERT DESIGN RULES PDF_**

The recommended minimum limits for embossed details on 3D prints are to have a 0.6 mm wide gap and 2 mm depth. I decided to use this as the starting point and determine how thin the engraving could get. I planned on creating a rectangle with six of the same engravings but each having a lower width by 0.1 mm. This meant the widths would step down from 0.6 to 0.5 to 0.4 mm etc. until reaching 0.1 mm wide. This way, I could see when the embossing would no longer be visible and would be filled in by the printer.

### Prediction

For the testing the embossing limits, my prediction was that the printer would be able to go down to about 0.4 mm. I didn't really have any reasoning behind it but the Prusa Core One Printers are very precise so I predicted it would be able to get to a finer level of detail. 

## CAD Design

### Mark 1 Design

For the initial design of the embossing test model, I started with a rectangle which would have the engravings in a straight line. I used the initial dimension of 20 mm by 40 mm with a height or thickness of 2.5 mm.

![Iteration 1 - Screenshot 1](Itrn-1-Screenshot-2.png)

![Iteration 1 - Screenshot 2](Itrn-1-Screenshot-3.png)

For the actual engraving, I figured the easiest thing to do would be a single letter or number. I decided to do a capital D because it's the first letter of my name and also it is a good test of the printers ability to print straight and curved lines. A capitol D is also relatively straight forward to create with lines as well.

![Iteration 1 - Screenshot 3](Itrn-1-Screenshot-6.png)

![Iteration 1 - Screenshot 4](Itrn-1-Screenshot-7.png)

* I first created an "outer" D shape and scaled it so it would be 8 mm tall and 6 mm wide. However, I quickly increased the dimensions to a height of 10 mm, width of 7 mm, the semicircle had a radius of 5mm, and the small straight edge had a length of 2 mm.

![Iteration 1 - Screenshot 5](Itrn-1-Screenshot-5.png)

![Iteration 1 - Screenshot 6](Itrn-1-Screenshot-6.png)

![Iteration 1 - Screenshot 7](Itrn-1-Screenshot-7.png)

![Iteration 1 - Screenshot 8](Itrn-1-Screenshot-9.png)

* I created an "Inner" D shape that was needed to make sure the extrude would actually be an engraving versus a big D shaped hole. The inner D was the same as the outer D except the distance from the edges would change on each iteration of the D's to achieve the smaller width I was testing. The first D had an engraving width of 0.6 mm meaning the edges of the inner D were 0.6 mm away from the edges of the outer D.

![Iteration 1 - Screenshot 9](Itrn-1-Screenshot-10.png)

![Iteration 1 - Screenshot 10](Itrn-1-Screenshot-11.png)

![Iteration 1 - Screenshot 11](Itrn-1-Screenshot-12.png)

* I realized the the height of the rectangle I initially made was too tall so I went back and edited the sketch to make it 12 mm tall which would give a distance of 1 mm from the edges of the D to the edges of the rectangle.

* To create the other 5 D's, I used the "create linear pattern" command in Solidworks to copy the outer and inner D's five times. Although, initially, I miscounted and only copied 4 until I realized my mistake and added the sixth one.

![Iteration 1 - Screenshot 12](Itrn-1-Screenshot-13.png)

![Iteration 1 - Screenshot 13](Itrn-1-Screenshot-14.png)

![Iteration 1 - Screenshot 14](Itrn-1-Screenshot-15.png)

* I made sure that each D had a distance of 1 mm between the edges. I then manually incremented the distance between the edges of each D, lowering the distance by 0.1 mm each time.

![Iteration 1 - Screenshot 16](Itrn-1-Screenshot-16.png)

![Iteration 1 - Screenshot 17](Itrn-1-Screenshot-17.png)

![Iteration 1 - Screenshot 18](Itrn-1-Screenshot-18.png)

* I realized I needed one more copy for the 0.1 mm width test.

![Iteration 1 - Screenshot 19](Itrn-1-Screenshot-19.png)

![Iteration 1 - Screenshot 20](Itrn-1-Screenshot-20.png)

![Iteration 1 - Screenshot 21](Itrn-1-Screenshot-21.png)

* Pictured above are the dimensions and widths of the engravings for all 6 of the D's.

* I then corrected the length of the rectangle so that all the D's would fit and there wouldn't be a floating sketch.

![Iteration 1 - Screenshot 22](Itrn-1-Screenshot-22.png)

* Next, I performed an emboss cut of 2 mm on all of the D's to put in the actual engravings.

![Iteration 1 - Screenshot 23](Itrn-1-Screenshot-23.png)

![Iteration 1 - Screenshot 24](Itrn-1-Screenshot-24.png)

![Iteration 1 - Screenshot 25](Itrn-1-Screenshot-25.png)

![Iteration 1 - Screenshot 26](Itrn-1-Screenshot-26.png)

![Iteration 1 - Screenshot 27](Itrn-1-Screenshot-27.png)

![Iteration 1 - Screenshot 28](Itrn-1-Screenshot-28.png)

With the Engravings in place, I would move on to exporting the file as an STL and slicing it.

### Mark 1 Preprocessing

When I loaded the STL into the Prusa Slicer, I finally saw how small the model was. In the CAD software just looking at the numbers, I knew it would be small but I wasn't able to visualize it. And when I sliced it, I saw how close the print lines were in between the D's in the 1 mm gap. There was no room for any infill, and the D's would just be separated by two walls. 

![Iteration 1 - Screenshot 29](Itrn-1-Screenshot-29.png)

![Iteration 1 - Screenshot 30](Itrn-1-Screenshot-30.png)

![Iteration 1 - Screenshot 31](Itrn-1-Screenshot-31.png)

I decided that the distances between the D's were two small and I wanted to give more space between each one and the edges.

I tried to modify the pattern in Solidworks to increase the separation distance, but I kept running into constraint problems. In the end, I gave up and started over again.

### Mark 2 Design

For the mark 2 design of the embossing test model, I decided to created a larger rectangle and create a 2 x 3 grid of D's. Since I already had practice from the first model, this second one was much the same and went significantly faster. 

* Once again, I started with a rectangle, this time one that was 26 x 27 x 3 mm.

![Iteration 2 - Screenshot 1](Itrn-2-Screenshot-1.png)

* I went with the same dimension for the D's (height of 10 mm, width of 7 mm, semicircle radius of 5mm, and the small straight edge length of 2 mm).

![Iteration 2 - Screenshot 2](Itrn-2-Screenshot-2.png)

* The primary change I made was that now the distance between the outer edge of the D and the edge of the rectangle was 2 mm.

* I also realized I did my math wrong and I needed to increase the width of the base rectangle from 27 to 31 mm.

![Iteration 2 - Screenshot 3](Itrn-2-Screenshot-3.png)

![Iteration 2 - Screenshot 4](Itrn-2-Screenshot-4.png)

* I once again used the linear pattern command but this time, I had to create 3 copies in the x-direction and 2 in the y-direction.

![Iteration 2 - Screenshot 5](Itrn-2-Screenshot-5.png)

![Iteration 2 - Screenshot 6](Itrn-2-Screenshot-6.png)

* I kept a distance of 2 mm between each of the D's as well.

* Then, I repeated the process of creating "inner" D's starting with the top left and shrinking the distances between edges to create smaller and smaller engravings.

![Iteration 2 - Screenshot 7](Itrn-2-Screenshot-7.png)

![Iteration 2 - Screenshot 8](Itrn-2-Screenshot-8.png)

![Iteration 2 - Screenshot 9](Itrn-2-Screenshot-9.png)

![Iteration 2 - Screenshot 10](Itrn-2-Screenshot-10.png)

![Iteration 2 - Screenshot 11](Itrn-2-Screenshot-11.png)

![Iteration 2 - Screenshot 12](Itrn-2-Screenshot-12.png)

* Then, I extrude cut all the D's to create the engravings.

![Iteration 2 - Screenshot 13](Itrn-2-Screenshot-13.png)

![Iteration 2 - Screenshot 14](Itrn-2-Screenshot-14.png)

![Iteration 2 - Screenshot 15](Itrn-2-Screenshot-15.png)

![Iteration 2 - Screenshot 16](Itrn-2-Screenshot-16.png)

With the engravings in place on the mark 2 model, it was time to put it into the Prusa Slicer and see how it looked.

### Preprocessing Mark 2 Design

The mark 2 design had much more space between the engravings and the edges which I felt better about. I decided to go with this version and I started changing some of the parameters.

![Iteration 2 - Screenshot 17](Itrn-2-Screenshot-17.png)

![Iteration 2 - Screenshot 18](Itrn-2-Screenshot-18.png)

* The first parameter I changed was to change print mode from '0.20 mm SPEED' to '0.15 mm BALANCED.' I did this because I wanted some more precision over speed. And with the 0.15 mm extude width, I assumed that it would help the printer gain some precision when printing the thin gaps.

![Iteration 2 - Screenshot 19](Itrn-2-Screenshot-19.png)

* The next settings I changed were the infill type and infill density. I changed the infill to the 'line' type because, based off of my research during the previous lab, the line infill collects less filament when printing the infill. This is because it only prints the lines going one direction each pass, it alternates between the two sets of perpendicular lines. The standard grid infill prints another layer of all the lines each pass. This can cause filament to collect at the intersections of the lines. I used the line infill to try and avoid the extra collection of infill that could potentially fill in the gaps.

![Iteration 2 - Screenshot 20](Itrn-2-Screenshot-20.png)

![Iteration 2 - Screenshot 21](Itrn-2-Screenshot-21.png)

![Iteration 2 - Screenshot 22](Itrn-2-Screenshot-22.png)

Those were all the parameters I changed for the print. With the model set and sliced, I could move on to printing it.


## Printing

The Mark 2 test desing was sliced and the GCode was exported onto a USB Drive to be loaded onto the printer. The print use PLA and was printed on printer 7. I didn't notice any problems as the model printed.

![Penrose Image 2](Penrose-Print-Img-2.jpg)

* The Print Preview

<video width="100%" controls>
  <source src="docs/Labs/L04/Penrose-Print-Vid-1-Cut.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

[Click here to view video if it doesn't load automatically](Penrose-Print-Vid-1-Cut.mp4)

* The Printer starting on the model, beginning the infill.

![Penrose Image 4](Penrose-Print-Img-4.jpg)

![Penrose Image 11](Penrose-Print-Img-11.jpg)

![Penrose Image 12](Penrose-Print-Img-12.jpg)

* The printer about 25% done.

![Penrose Image 2](Penrose-Print-Img-2.jpg)

<video width="100%" controls>
  <source src="docs/Labs/L04/Penrose-Print-Vid-2-Cut.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

[Click here to view video if it doesn't load automatically](Penrose-Print-Vid-2-Cut.mp4)

* The Print Finishing

![Penrose Image 19](Penrose-Print-Img-19.jpg)

![Penrose Image 21](Penrose-Print-Img-21.jpg)

![Penrose Image 23](Penrose-Print-Img-23.jpg)

The finished model turned out better than I expected. The size of the model helped hide a lot of the seams I wasn't happy with and while the illusion isn't really there, you can tell what it's going for. Overall, I was very pleased with the end result. 

## Lessons Learned

This design project was a good exercise in trying to use a CAD software to design something that had weird angles and strange overlapping geometry. Learning how to use reference planes would've likely solved most of my problems. However, I chose to use trial and error regarding the order of extruded cuts and the surfaces on which I cut to achieve a design I was satisfied with. A constructive method might've been better too, but that wouldn't eliminate the weird angles. I did learn that I overestimated the scale of what I made. A lot of the finer angles and details are mostly lost in the 3D print due to the printer printing in a very geometric way. It lessons the visibility and details of the angles meaning a lot of the work was I put in was rendered obsolete when it was printed but the effort was still worth it to learn my limitations with CAD software and especially Solidworks. Learning about infills and wall thicknesses also taught me a lot about the use cases for different wall and infill parameters while also demonstrating to me once again the flexibility of 3D printing and additive manufacturing.

The modeling process of the Penrose Triangle took around 6 hours.

## Resources

[Penrose Triangle](https://en.wikipedia.org/wiki/Penrose_triangle)

[Prusa 3D Infill Patterns](https://help.prusa3d.com/article/infill-patterns_177130)

[3D printing infill patterns to save time, material and money](https://realvision.pro/2022/10/05/3d-printing-infill-patterns/)

[Hilbert Curve](https://en.wikipedia.org/wiki/Hilbert_curve)

[Path planning for the infill of 3D printed parts utilizing Hilbert curves](https://www.sciencedirect.com/science/article/pii/S235197891830221X)

[Infill in 3D Printing: Definition, Main Parts, and Different Types](https://xometry.pro/en/articles/3d-printing-infill/)

[What is the Strongest Infill Pattern?]( https://theprintedfuture.com/what-is-the-strongest-infill-pattern/)

[The effects of infill patterns on the mechanical properties of 3D printed PLA parts fabricated by FDM](https://www.researchgate.net/publication/359334862_The_effects_of_infill_patterns_on_the_mechanical_properties_of_3D_printed_PLA_parts_fabricated_by_FDM)

[Designing Wall Thickness for 3D Printing: Minimums, Maximums, Best Practices](https://bigrep.com/posts/designing-wall-thickness-for-3d-printing/)

[Wall Thickness in 3D Printing: Recommendations, Minimum and Maximum Values](https://www.raise3d.com/blog/3d-printing-wall-thickness/)


