# A4 – Design Something Small

## Objective

The goal of the third lab was to design and then print a small object of our choosing. 

I chose to design the Penrose Triangle, otherwise know as the Impossible Tribar. 

![Penrose Triangle](Penrose-Triangle.webp)

[(Penrose Triangle](https://en.wikipedia.org/wiki/Penrose_triangle)

The Penrose Triangle is an optical illusion that depends entirely on being able to view the object from a certain perspective in 3 dimensions. However, the assignment limited the height of the designed object to be less than 0.5 inches tall and no more than 1.5 x 1.5 inches. I challenged myself to see if I could recreate a 3 dimensional optical illusion while keeping a similar effect. 

## Infill and Wall Thickness Research



## Design

When starting the design in Solidworks, I figure it was going to be very easy. I was just going to have three different heights on the edges to try and mimic the rectangular prisms that the Penrose Triangle is composed of. I also wanted the edges to be angled to even further try and mimic the shape but I would later run into difficulties and would have to rethink things.

To start, I made a 2D sketch of a triangle with a smaller triangle in the center for the cutout and extruded that up. I went for a more subtractive modeling approach over an additive one. 

![Penrose Screenshot 4](Penrose-Screenshot-4.png)

* The important thing I had to keep in mind was keeping the middle triangle equidistant from the edges of the outer triangle. I did this by using smart dimensions and constraints so the middle triangle would be perfectly in the center of all the edges of the outer triangle. 



![Penrose Screenshot 5](Penrose-Screenshot-5.png)

![Penrose Screenshot 7](Penrose-Screenshot-7.png)

To split each section of the triangle in half, I used a bunch of midpoint lines so I would be able to get the exact center. 

![Penrose Screenshot 8](Penrose-Screenshot-8.png)

Using the construction lines as I guidance, I could then extrude cut half of the edges to try and mimic the illusion of the Penrose Triangle using depth.

![Penrose Screenshot 10](Penrose-Screenshot-10.png)

![Penrose Screenshot 11](Penrose-Screenshot-11.png)

![Penrose Screenshot 12](Penrose-Screenshot-12.png)

![Penrose Screenshot 13](Penrose-Screenshot-13.png)

![Penrose Screenshot 14](Penrose-Screenshot-14.png)

![Penrose Screenshot 16](Penrose-Screenshot-16.png)

![Penrose Screenshot 20](Penrose-Screenshot-20.png)

At this point, I decided to abandon the idea of making the edges slanted relative to each other to make them look like rectangular prisms. However, I did want the edges to look like they tapered off into each other and appear to disappear behind each other.

However, I would quickly run into the reoccurring issue of this design, that being: weird angles. Everything was on a weird angle which made it very difficult to do anything geometrically. And I couldn't figure out how to make reference planes work with the angles. 

![Penrose Screenshot 21](Penrose-Screenshot-21.png)

![Penrose Screenshot 22](Penrose-Screenshot-22.png)

![Penrose Screenshot 23](Penrose-Screenshot-23.png)

![Penrose Screenshot 24](Penrose-Screenshot-24.png)

* The moment I figured out these angles would cause me a massive headache.

![Penrose Screenshot 26](Penrose-Screenshot-26.png)

I decided to keep the sketches on the outside edges because while the slants wouldn't be straight, it would at least be more consistent than trying to go from the end. 

![Penrose Screenshot 27](Penrose-Screenshot-27.png)

![Penrose Screenshot 28](Penrose-Screenshot-28.png)

I didn't like the flat surface that was created at the corner so I tried redoing the sketches in the opposite order to make the edges and slants fit together better.

![Penrose Screenshot 30](Penrose-Screenshot-30.png)

![Penrose Screenshot 31](Penrose-Screenshot-31.png)

However, this created a lip where the two slants meet that I also didn't like. 

![Penrose Screenshot 37](Penrose-Screenshot-37.png)

I messed around with cut extrudes for a long time before I got to this which I was satisfied with. I also was spending too much time on this single corner and knew I had to move on. I worked on making the same slope on the other edges. 

![Penrose Screenshot 38](Penrose-Screenshot-38.png)

![Penrose Screenshot 39](Penrose-Screenshot-39.png)

![Penrose Screenshot 40](Penrose-Screenshot-40.png)

![Penrose Screenshot 42](Penrose-Screenshot-42.png)

* Here I raised the height of the sketch because if I had left it with the corners being coincident, I would have ended up with a flat face again. I tried to raise it to the height which would create a clean intersection between the edges when cut.

![Penrose Screenshot 44](Penrose-Screenshot-44.png)

I decided to leave the lowest edge alone, because the lowest edge being flat worked with the perspective. Also, trying to get an extrusion in there would've been more difficulty than it was worth.

Instead, I came back to the idea of have the edges slanted slightly along the length. To do this, at the corners, I would extrude cut a small piece out so that I could work on the edge at a 90 degree angle. That way, when I made a sketch to cut out the angle, it would actually be straight relative to the edge.

![Penrose Screenshot 46](Penrose-Screenshot-46.png)

![Penrose Screenshot 47](Penrose-Screenshot-47.png)

![Penrose Screenshot 49](Penrose-Screenshot-49.png)

![Penrose Screenshot 51](Penrose-Screenshot-51.png)

* I went back and made it so the whole edge would be slanted rather than just half.

![Penrose Screenshot 52](Penrose-Screenshot-52.png)

![Penrose Screenshot 53](Penrose-Screenshot-53.png)

![Penrose Screenshot 54](Penrose-Screenshot-54.png)

![Penrose Screenshot 57](Penrose-Screenshot-57.png)

I tried to do the same thing on the lower edge. However, I foresaw it not going well and decided to move on to the upper edge.

![Penrose Screenshot 55](Penrose-Screenshot-55.png)

![Penrose Screenshot 56](Penrose-Screenshot-56.png)

I repeated the same process on the upper edge and then I used sketches and extrudes to rebuild the corners I cut out. Afterwards though, I realized that I could've left the corners cut out since the Penrose Triangle has flat corners, but it didn't occur to me at the time. 

![Penrose Screenshot 59](Penrose-Screenshot-59.png)

![Penrose Screenshot 60](Penrose-Screenshot-60.png)

![Penrose Screenshot 61](Penrose-Screenshot-61.png)

![Penrose Screenshot 62](Penrose-Screenshot-62.png)

![Penrose Screenshot 63](Penrose-Screenshot-63.png)

The weird angles made filling in the corners more annoying than it should have been but with a little trial and error, I got the corners filled in.

![Penrose Screenshot 64](Penrose-Screenshot-64.png)

![Penrose Screenshot 65](Penrose-Screenshot-65.png)

![Penrose Screenshot 66](Penrose-Screenshot-66.png)

![Penrose Screenshot 67](Penrose-Screenshot-67.png)

![Penrose Screenshot 68](Penrose-Screenshot-68.png)

![Penrose Screenshot 69](Penrose-Screenshot-69.png)

With that, I called the design finished and moved it into the slicer for printing and preprocessing. 

## Preprocessing

Once I finished with the design of the Penrose Triangle, I loaded the STL file into the Prusa Slicer. I had designed it to lay flat on the print bed so no change of orientation would be needed.

![Penrose Screenshot 70](Penrose-Screenshot-70.png)

![Penrose Screenshot 71](Penrose-Screenshot-71.png)

The Penrose Triangle at the default size I made it was very small. It would've only taken four minutes to print with all of the default parameters. 

I decided to scale it up by a factor of about 150% to make it a little more substantial and closer to the maximum parameters I could. This way, more infill would be needed and I would have more room to mess with the parameters. I mostly focused on not letting the height go over the max of 0.5 inches or 12.7 millimeters. I scaled it up so the height would be about 9 millimeters instead of 5. 

![Penrose Screenshot 72](Penrose-Screenshot-72.png)

![Penrose Screenshot 74](Penrose-Screenshot-74.png)

![Penrose Screenshot 75](Penrose-Screenshot-75.png)

This increased the print time for 4 minutes to 7 minutes and increased the time of the first layer by about 10 seconds. However, this was still with the default parameters. I needed to change the infill and wall thickness. 

I increased the vertical wall thickness from the minimum of two shells to three shells. I wanted to make sure that the outside walls would have decent strength and be able to hold it's shape. I changed the infill from the default grid pattern to the stars pattern. The star pattern intrigued me because I had never seen it before using the Prusa Slicer and, after having researched it, it sounded like a good mix of the structural integrity and flexibility that were given by the triangle and honeycomb fill patterns. I increased the fill density to 25% to make sure there was enough for the surfaces to adhere to. 

With the final changes made, the print time was still around 7 to 8 minutes with 36 seconds for the first layer.

## Printing

The Penrose Triangle was sliced and the GCode was exported onto a USB Drive to be loaded onto the printer. The printing went smoothly and there were no issues. The print use PLA and was printed on printer 3. 

![Penrose Image 2](Penrose-Print-Img-2.jpg)

* The Print Preview

<video width="100%" controls>
  <source src="docs/Labs/L04/Penrose-Print-Vide-1-Cut.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

[Click here to view video if it doesn't load automatically](Penrose-Print-Vide-1-Cut.mp4)

* The Printer starting on the model, beginning the infill.

![Penrose Image 4](Penrose-Print-Img-4.jpg)

![Penrose Image 11](Penrose-Print-Img-11.jpg)

![Penrose Image 12](Penrose-Print-Img-12.jpg)

* The printer about 25% done.

![Penrose Image 2](Penrose-Print-Img-2.jpg)

<video width="100%" controls>
  <source src="docs/Labs/L04/Penrose-Print-Vide-1-Cut.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

[Click here to view video if it doesn't load automatically](Penrose-Print-Vide-1-Cut.mp4)

* The Print Finishing

![Penrose Image 19](Penrose-Print-Img-19.jpg)

![Penrose Image 21](Penrose-Print-Img-21.jpg)

![Penrose Image FINISHED](Penrose-Print-Img-12.jpg)

The finished model turned out better than I expected. The size of the model helped hide a lot of the seams I wasn't happy with and while the illusion isn't really there, you can tell what it's going for. Overall, I was very pleased with the end result. 

## Communicate

