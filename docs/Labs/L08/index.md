# A8 – Design and Print Something Useful

## Objective

The objective of the eighth lab is to design and create something useful.

## Reading and Writing

According to the article, "[Great Questions Lead to Great Design: A Guide to the Design-thinking Process](https://www.toptal.com/designers/product-design/design-thinking-great-questions)", asking "smart questions" is a way to dig deeper into the root cause of an issue, foster creativity and new ideas, and encourage team collaboration. By asking "smart questions," designers can better understand the root cause of the issue they are trying to solve. Better understanding of the underlying issue helps inform solutions for the issue to be more accurate and applicable to the issue. Asking "smart questions" can also encourage creativity by asking the designer what they considered, what they didn't, and why they chose the solution that they did. Open ended questions are a good way to open up pathways to new ideas and innovations. And finally, "smart questions" are a way to encourage team collaboration and discussion on a design, what the design is for, why the design is needed, and different ways to consider approaching the design.

## Design Purpose

For my design, I worked with my parents who run the quilt shop Quilt-n-Code in Burnsville NC to design something useful for the business. 

### Problem

The problem I made my design to solve was that my parents had been creating these 3D printed name tags or signs that they wanted to use to display prices or details about products. So I designed a stand that would be able to hold these 3D printed signs. It is also able to just hold paper or cardboard if there are signs that need to be displayed that are not 3D printed, so long as they're of the appropriate size.

I designed the stand to be parametrically based on the dimensions of the signs to make it easier to adjust the size for larger or smaller signs. 

I started by measuring the test sign I was given that also functions as a name tage.

<img width="3000" height="4000" alt="Sign-Measurement (2)" src="https://github.com/user-attachments/assets/0a655665-39d1-474c-9162-94aed9f24c88" />

<img width="4000" height="3000" alt="Sign-Measurement (4)" src="https://github.com/user-attachments/assets/fc2f2bcf-8a5e-4994-8367-31f6d51e2052" />

<img width="4000" height="3000" alt="Sign-Measurement (7)" src="https://github.com/user-attachments/assets/f94c69fe-d8a0-41de-86af-27f683c0173c" />

I found the dimensions of the 3D printed sign to be 3.5 inches by 2 inches by 0.2 inches.

## Stand CAD Model

The CAD model was designed parametrically based on the signs dimensions, allowing the dimensions to be changed very easily for larger or smaller signs. Nearly all the parameters were derived from the base, height, and thickness of the sign using the Global Variables and Equations in Solidworks.

<img width="780" height="503" alt="QnC-Stand-CAD (1)" src="https://github.com/user-attachments/assets/be71f240-c006-4e62-8360-c5e8dc2cbcaf" />

For the design of the stand, I was thinking a simple L shape that was slanted with a component on the front in which to put the sign.

I started with a rectangular base that I set to be the dimensions of the sign parametrically.

<img width="960" height="564" alt="QnC-Stand-CAD (4)" src="https://github.com/user-attachments/assets/264dfac2-e92d-40a9-ade4-5c40dccef0c0" />

<img width="960" height="564" alt="QnC-Stand-CAD (5)" src="https://github.com/user-attachments/assets/2c3c15d4-78f3-4c9e-815d-56641e43d4a6" />

<img width="960" height="564" alt="QnC-Stand-CAD (3)" src="https://github.com/user-attachments/assets/4e901f93-177d-47de-a10e-b80c663d8518" />

I then extruded it up, using the "wall thickness" variable to determine the thickness of the stand. 

<img width="960" height="564" alt="QnC-Stand-CAD (6)" src="https://github.com/user-attachments/assets/ac17db45-f66d-42b6-bae4-a0a77ccda9b6" />

<img width="960" height="564" alt="QnC-Stand-CAD (7)" src="https://github.com/user-attachments/assets/e83977d1-7697-4ec7-9765-048d1cbf9b70" />

I then created a second parallelogram at an angle relative to the first. 

<img width="960" height="564" alt="QnC-Stand-CAD (11)" src="https://github.com/user-attachments/assets/dabe4f2b-c6cf-4afd-bc95-ab9f8a56dac5" />

I set the angle at 70 degrees and created a variable for it so that it could be changed later if desired.

I then extruded the part across the same distance as the base. 

<img width="960" height="564" alt="QnC-Stand-CAD (12)" src="https://github.com/user-attachments/assets/3b7b5359-43ca-4359-9d35-86964c5427f0" />

<img width="960" height="564" alt="QnC-Stand-CAD (13)" src="https://github.com/user-attachments/assets/c5cc81f2-f4c9-48a6-be18-d5cb61d0afa9" />

Next, I began working on the section that would be on the front of the stand that would actually hold the sign. I used several rectangles to create the shape.

<img width="960" height="564" alt="QnC-Stand-CAD (14)" src="https://github.com/user-attachments/assets/e221a40e-a6a5-41dd-a1e5-f4b1142acf1a" />

<img width="960" height="564" alt="QnC-Stand-CAD (15)" src="https://github.com/user-attachments/assets/31bf2229-6c1e-46c8-b2c1-2071b838ece9" />

<img width="960" height="564" alt="QnC-Stand-CAD (16)" src="https://github.com/user-attachments/assets/332a3bde-261a-4de9-ba75-31ad1c758061" />

I adjusted some of the equations to make sure there was some tolerance in the gap between the edges and the sign. I didn't want to risk it being too small and preventing the sign from going in. And the sign didn't need to be held super tightly either.

<img width="780" height="503" alt="QnC-Stand-CAD (19)" src="https://github.com/user-attachments/assets/e1a22d7d-2acb-4d76-84e2-fb95dc4e1559" />

There ended up being about 0.05 inches of clearance that I would later increase to 0.1 inches. I didn't have a real reason for choosing these tolerances, I figured that an extra 0.1 inches would be enough to allow something to slide in and out of freely.

<img width="960" height="564" alt="QnC-Stand-CAD (20)" src="https://github.com/user-attachments/assets/c2102597-d31d-4c4f-8452-b02a16446457" />

The next step was to extrude it out.

<img width="960" height="564" alt="QnC-Stand-CAD (22)" src="https://github.com/user-attachments/assets/58065b49-ca45-4658-9a9f-f57faf43d528" />

<img width="960" height="564" alt="QnC-Stand-CAD (23)" src="https://github.com/user-attachments/assets/afc78da3-b472-433f-890e-a3782cab9036" />

After that, I created another section out of rectangles that was double the width to prevent the sign from falling out.

<img width="960" height="564" alt="QnC-Stand-CAD (24)" src="https://github.com/user-attachments/assets/a5aa9a38-621c-45df-84fc-a3fbed2cfe3c" />

<img width="960" height="564" alt="QnC-Stand-CAD (25)" src="https://github.com/user-attachments/assets/8d972928-b1b9-43f2-b2a6-c9f050fc25d2" />

With that, the first design for the stand was finished.

<img width="960" height="564" alt="QnC-Stand-CAD (30)" src="https://github.com/user-attachments/assets/e21ff821-3c9c-439b-bebd-2a869d063782" />

However, I was informed that I misinterpreted how my parents wanted the stand to be designed. They wanted a more complex frame to hold the sign, as illustrated in the drawing they sent. 

<img width="1536" height="2048" alt="QnC_Stand-Drawing" src="https://github.com/user-attachments/assets/c71d9755-ba74-4836-8266-01ecb426316a" />

So I went back and undid what I had made to originally hold the sign but I could at least reuse the base and adjust the height.

<img width="960" height="564" alt="QnC-Stand-CAD (33)" src="https://github.com/user-attachments/assets/8f79c2ed-070f-4e80-8801-e1c8298c0d5d" />

<img width="960" height="564" alt="QnC-Stand-CAD (34)" src="https://github.com/user-attachments/assets/43dccfa5-aa5d-4167-849e-f2b4ddede77a" />

I lowered the height and created a rectangle to work off of on the angled part of the stand.

<img width="960" height="564" alt="QnC-Stand-CAD (36)" src="https://github.com/user-attachments/assets/a25b04d6-0fd9-4bce-b0e8-691dfcc32196" />

I again made it dependent on the parameters I had set so it would change and update automatically if the size changed.

<img width="960" height="564" alt="QnC-Stand-CAD (37)" src="https://github.com/user-attachments/assets/a2dfd40d-55bd-41b7-95d3-35e573584219" />

<img width="960" height="564" alt="QnC-Stand-CAD (38)" src="https://github.com/user-attachments/assets/7318728f-730b-42c5-80ca-e749118bb901" />

<img width="960" height="564" alt="QnC-Stand-CAD (39)" src="https://github.com/user-attachments/assets/891b1efb-c127-48f3-8e1a-359f4ba200ed" />

Next, I extruded a hollow rectangle from the top of the rectangle I just made.

<img width="960" height="564" alt="QnC-Stand-CAD (40)" src="https://github.com/user-attachments/assets/ce44a2c3-014c-4188-9c8a-9e1a7062c2df" />

<img width="960" height="564" alt="QnC-Stand-CAD (42)" src="https://github.com/user-attachments/assets/12d7c015-576c-41d7-afb3-f54058412f96" />

<img width="960" height="564" alt="QnC-Stand-CAD (43)" src="https://github.com/user-attachments/assets/2ebdaa05-c0d6-485b-a214-4d57ec46dad2" />

I then cut a hole out of the front so the sign would be visible when inside.

<img width="960" height="564" alt="QnC-Stand-CAD (47)" src="https://github.com/user-attachments/assets/81836b5f-2542-4d8d-88b3-dda596166fcc" />

<img width="960" height="564" alt="QnC-Stand-CAD (52)" src="https://github.com/user-attachments/assets/d2320105-9dd1-448b-b8aa-dc790d1ed6b7" />

Finally, I did some final small modifications such as adjusting the height to be smaller.

<img width="780" height="503" alt="QnC-Stand-CAD (51)" src="https://github.com/user-attachments/assets/11d9c314-3200-4fcb-affa-13960e92fd4d" />

<img width="960" height="564" alt="QnC-Stand-CAD (54)" src="https://github.com/user-attachments/assets/833d99f3-21f7-4df1-85bc-98599660ed70" />

And with that, I had created something satisfactory for my parents so I moved on to printing it.


## Preprocessing

For the preprocessing, I loaded the model into the Prusa Slicer. I did not change the parameters very much and left the wall thickness, layer settings, and infill on the default settings. This left the infill at 15% grid, the wall thickness at about 1 mm, and the layer height at 0.2 mm. The only thing I changed was turning on auto generated organic supports since a lot of the model has large overhangs. I did also change the print mode to "BALANCED" because I figured too much speed might cause issues with the overhangs. Beyond that, I didn't touch any of the specific settings of supports or print mode. I left the overhang threshold at 35 degrees which worked out well and the auto generated supports placed supports where I figured they were needed.

<img width="960" height="564" alt="QnC-Stand-Slice (4)" src="https://github.com/user-attachments/assets/ea480f9c-4f88-47df-81cd-7bd4ad4fb67f" />

<img width="960" height="564" alt="QnC-Stand-Slice (7)" src="https://github.com/user-attachments/assets/bf79ecec-41fd-4cac-9749-c5c3028e000f" />

The print would take about an hour and a half and had 355 layers and a volume of 37,095 mm. I did not edit the position of the model or the rotation, it was standing up on the base and I didn't see how any other position might be more optimal. I left it as is and began printing it.


## Printing

### Attempt 1

For the printing, I printed the model on printer 13 with PLA filament. 

<img width="4000" height="3000" alt="QnC-Stand-Print-Attempt (3)" src="https://github.com/user-attachments/assets/4c7f24d8-c641-410d-aeef-8a26953993da" />

<video width="100%" controls>
  <source src="QnC-Stand-Print-Attempt1-Vid-1.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

<img width="4000" height="3000" alt="QnC-Stand-Print-Attempt (6)" src="https://github.com/user-attachments/assets/64727e61-f38d-4324-9dce-344d46f32eb7" />

<img width="4000" height="3000" alt="QnC-Stand-Print-Attempt (11)" src="https://github.com/user-attachments/assets/a2daaad0-02b1-4af9-b9c0-a442de1f8c0a" />

<img width="4000" height="3000" alt="QnC-Stand-Print-Attempt (14)" src="https://github.com/user-attachments/assets/d33373f1-8173-439f-a2a6-b9c215f1a1d2" />

<video width="100%" controls>
  <source src="QnC-Stand-Print-Attempt1-Vid-2.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

<img width="4000" height="3000" alt="QnC-Stand-Print-Attempt (16)" src="https://github.com/user-attachments/assets/25139a16-b785-4aee-9e32-2ff5ab4463ca" />

The print proceeded with no issues, and came out looking good.

<img width="4000" height="3000" alt="QnC-Stand-Print-Attempt (18)" src="https://github.com/user-attachments/assets/b1cdb9cd-42be-4f55-8439-35119b99dad4" />

<img width="4000" height="3000" alt="QnC-Stand-Print-Attempt (19)" src="https://github.com/user-attachments/assets/f0f1d6c2-357f-4cfb-bf61-c67a0893b2cd" />

The supports came off usually just using my hands but I did use some pliers for the supports on the back that were more tucked away. The supports didn't really affect the surface finish at all but the different layers on the bottom of the overhangs were very noticeable. 

<img width="4000" height="3000" alt="QnC-Stand-Print-Attempt (21)" src="https://github.com/user-attachments/assets/f867351c-9f18-489f-87e4-44981014b065" />

<img width="4000" height="3000" alt="QnC-Stand-Print-Attempt (22)" src="https://github.com/user-attachments/assets/ba68abf6-766a-4f85-aebd-fa35c9f4a525" />

However, I realized an issue once I tried to put the other 3D printed name tag in.

<img width="4000" height="3000" alt="QnC-Stand-Print-Attempt (23)" src="https://github.com/user-attachments/assets/eda2b613-58e7-4b64-bcd7-c82dea417379" />

It turns out, I had printed it too small and the sign didn't fit. I rechecked my measurements and realized that I had set the width to 3 inches instead of 3.5 inches. This made the stand 0.5 inches smaller than it should have been. Realizing this, I fixed it and tried printing the stand again.


### Attempt 2

Once I realized I had input the wrong width measurement, it was easy to correct the error. Since I had designed everything parametrically, all I had to do was go in and change the 3 to 3.5 and the model automatically updated. 

<img width="780" height="503" alt="QnC-Stand-Slice (8)" src="https://github.com/user-attachments/assets/0c822481-4840-41ea-a853-aec7f6bba1e3" />

<img width="960" height="564" alt="QnC-Stand-Slice (9)" src="https://github.com/user-attachments/assets/f7401eda-8ef3-42de-a1c9-bdca84cd1f9d" />

With that, I printed it again with the same exact settings on the same printer. Since the model was wider now, it took closer to an hour and 45 minutes to print. 

<img width="960" height="564" alt="QnC-Stand-Slice (11)" src="https://github.com/user-attachments/assets/23352660-7ea2-4050-b9cc-6566f0d2ddcb" />

The print once again turned out good and ran into no problems.

<img width="4000" height="3000" alt="QnC-Stand-Print-Attempt2 (1)" src="https://github.com/user-attachments/assets/256d1742-8d96-4e98-820a-9f6780a82555" />

<video width="100%" controls>
  <source src="QnC-Stand-Print-Attempt2-Vid-1.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

<img width="4000" height="3000" alt="QnC-Stand-Print-Attempt2 (2)" src="https://github.com/user-attachments/assets/611fb626-9bdd-4b9b-8da7-46b1c7ce294a" />

<img width="4000" height="3000" alt="QnC-Stand-Print-Attempt2 (3)" src="https://github.com/user-attachments/assets/f3ff95c0-b1f2-40ec-b9d3-113f44f71f68" />

<img width="4000" height="3000" alt="QnC-Stand-Print-Attempt2 (4)" src="https://github.com/user-attachments/assets/114ac54f-8cf8-46d9-b66b-d40d68cd59cb" />

<video width="100%" controls>
  <source src="QnC-Stand-Print-Attempt2-Vid-2.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

<img width="4000" height="3000" alt="QnC-Stand-Print-Attempt2 (6)" src="https://github.com/user-attachments/assets/e0941a23-b861-4bac-8129-740e10af6dc7" />

<img width="4000" height="3000" alt="QnC-Stand-Print-Attempt2 (9)" src="https://github.com/user-attachments/assets/9c741dc0-5b16-4852-bbe8-ea263b2e4ae9" />

The second print of the model looked identical to the first apart from being wider. And the extra width was enough to comfortably fit the sign without it being snug.

<img width="4000" height="3000" alt="QnC-Stand-Print-Attempt2 (10)" src="https://github.com/user-attachments/assets/1efd9f57-bfe0-4361-9009-bd4da93e30ca" />

Overall, the design came out satisfactory and the stand is capable of holding the sign comfortably and it is also able to hold paper or whatever else fits in the slot on the top.


## Lessons Learned

For this lab, I learned more about designing a model for someone else. I tried to make it as versatile as possible, allowing the stand to display really whatever fits in it. While designing that stand, I also kept learning about the parametric design and making it so that every measurement is based on as few static variables as possible. I primarily wanted every dimension to be driven by the dimensions of the sign being inserted. Looking back, there are definitely some dimensions that don't make sense being driven by the dimensions I chose and I will try to implement smarter dimensioning in my next CAD project.

**Time Taken:** 9 Hours

### CAD File Download

[Stand Final Model Desing](QnC-Stand-5.SLDPRT)

[Stand Final Model Desing STL](QnC-Stand-5.STL)

## Resources

* [Great Questions Lead to Great Design: A Guide to the Design-thinking Process](https://www.toptal.com/designers/product-design/design-thinking-great-questions)

* [Quilt-n-Code](https://www.quilt-n-code.com/)
