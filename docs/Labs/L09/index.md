# A9 – Laser Cutter

## Objective

The objective for this weeks lab was to use a laser cutter in the Super Fab Lab at UNC Charlotte to design and create a series of parts that fit together, accounting for proper tolerances and kerf. 

## Design

### Parameter Testing

#### Kerf Measuring

To Determine the kerf of the laser cutter, I created a 20 x 20 millimeter square in Inkscape and cut it out on the laser cutter. I then measured the width of the square to determine the actual width. I could then subtract the actual width from the ideal width to determine the kerf. 

<img width="4000" height="3000" alt="Clearance-Test (1)" src="https://github.com/user-attachments/assets/88353227-6afa-4606-b460-939973cb712a" />

<img width="4000" height="3000" alt="Clearance-Test (7)" src="https://github.com/user-attachments/assets/095cc612-2185-4f99-87f3-254d87c340f2" />

The width of the actual square came out to be approximately 19.80 mm.

This made the kerf 20mm -19.80 mm = 0.20 mm. So a total of 0.20 mm of material is obliterated by the laser. 

#### Material Measuring

To improve the accuracy of the CAD model dimensions, the thickness of the wood being cut needed to be measured. 

Ideally 3 mm thick sheet of wood.

Measurement 1: 2.84 mm

Measurement 2: 2.70 mm

Measurement 3: 2.69 mm

Average Thickness: 2.74 mm

I would need the average thickness for determining the size of the fits I would need to create.

#### Fit Testing CAD Design

For the fit testing model, I made it very simple with three slots: One slot that is the same width as the desired width, a slot with positive clearance and a slot with negative clearance. 

I started by declaring the global variables.

<img width="780" height="503" alt="Clearance-Test-CAD-Pic (1)" src="https://github.com/user-attachments/assets/be468e98-2a37-46b2-843f-95195e14af9e" />

I then extruded a rectangle and cut the three slots out of it.

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (3)" src="https://github.com/user-attachments/assets/5b8c0eda-3854-469d-970e-7afa56597a64" />

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (10)" src="https://github.com/user-attachments/assets/adce2a23-8af2-4f23-b1dc-d77f56037c0f" />

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (12)" src="https://github.com/user-attachments/assets/ef76741a-99be-46c6-9d72-208d0cbfd56f" />

I spent a lot of time trying to put indented text on the model to keep track of which hole what what clearance.

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (16)" src="https://github.com/user-attachments/assets/8dea4a63-8b90-40c9-a484-11e887b0440a" />

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (17)" src="https://github.com/user-attachments/assets/325fc640-fefe-4a66-8dc9-d84cfe86abce" />

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (18)" src="https://github.com/user-attachments/assets/9a9c805b-27ca-4bd0-bf8f-f43366e3fdda" />

Next, I saved the document as a .dxf file from Solidworks and imported it into Inkscape. 

<img width="430" height="418" alt="Clearance-Test-CAD-Pic (20)" src="https://github.com/user-attachments/assets/8fa66661-0dcd-4b8e-89fe-5a80cf0f292e" />

One setting I made sure to change in Inkscape was to change the bounding box from visual to geometric. This change made it so that the lines and measurements were from the middle of the strokes versus the outside. This made it so the stroke thickness didn't matter.

<img width="459" height="398" alt="InkscapeBoundingBox" src="https://github.com/user-attachments/assets/7bfafe33-8e6c-437d-bb9e-2b5ef72c321f" />

I could then load the model into the Epilog job manger and cut the part. 

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (21)" src="https://github.com/user-attachments/assets/d3a3e596-28d1-44a1-b1e2-bd7d90f6bc87" />

<img width="4000" height="3000" alt="Clearance-Test (13)" src="https://github.com/user-attachments/assets/42468b6c-fac4-4cd1-b4c1-b217916b393c" />

However, this model turned out out to be too small and I realized I could just use the square I cut to test the tolerances so I didn't need to design and cut an entirely new part.

This led to me creating a new version that I would iterate on several times to find a clearance that worked. 

For the next version, I increased the size of the slot width to the square. I mistakenly started with the ideal width of the square which made the clearance much larger than it should have been. 

<img width="780" height="503" alt="Clearance-Test-CAD-Pic (24)" src="https://github.com/user-attachments/assets/aea429b7-3846-40a3-89c7-ad3a1463da0e" />

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (26)" src="https://github.com/user-attachments/assets/b785a523-3b9b-4d1d-a955-4f890fa79478" />

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (27)" src="https://github.com/user-attachments/assets/425a2cf2-bb97-4f4b-a101-b63e8fa9ba10" />

I gave up on the individual text for each slot and just created a marker for the hole with no tolerance as a reference. I kept the order consistent with the slot with no clearance first followed by the slot with negative clearance. 

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (29)" src="https://github.com/user-attachments/assets/d482d6b8-63fe-4e48-bedb-f467756fb3f5" />

I could then save this file as a .dxf file and load it into Inkscape. 

<img width="430" height="418" alt="Clearance-Test-CAD-Pic (30)" src="https://github.com/user-attachments/assets/f88fb15c-844f-4b56-b638-c927f03fa89d" />

Every time I saved a file, Solidworks attached a watermark to it. Luckily I could remove this in Inkscape so that the laser cutter wouldn't print it. 

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (31)" src="https://github.com/user-attachments/assets/ba233ae8-6b62-415d-a30e-784c2934d6e9" />

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (32)" src="https://github.com/user-attachments/assets/81374977-46eb-4dfa-b112-7361fd5ce488" />

<img width="960" height="565" alt="Clearance-Test-CAD-Pic (33)" src="https://github.com/user-attachments/assets/3420e886-ea29-4e49-a347-ad92bb861318" />

<img width="960" height="565" alt="Clearance-Test-CAD-Pic (34)" src="https://github.com/user-attachments/assets/62ab80ff-3f9c-4dc8-9354-cec797e70607" />

<video width="100%" controls>
  <source src="ClearanceTestVid1.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

<img width="4000" height="3000" alt="Clearance-Test (14)" src="https://github.com/user-attachments/assets/5679411f-a682-484f-a2e1-929c09cf740e" />

The cut turned out well but due to my larger dimensions, the slots were too wide.

I ended up creating another three cuts before I found a clearance that worked. 

<img width="4000" height="3000" alt="Clearance-Test (19)" src="https://github.com/user-attachments/assets/7ddb56b4-8fd2-484b-9c07-287b58d19607" />

For the final design, I decided to test two tighter tolerances since I had shortened the width of the slot to be the actual width of the square with kerf accounted for and tested tolerances from -0.1 mm to -0.3 mm.

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (47)" src="https://github.com/user-attachments/assets/27b54073-9997-4a70-8ae6-5a66c090fc7b" />

<img width="780" height="503" alt="Clearance-Test-CAD-Pic (46)" src="https://github.com/user-attachments/assets/c18ac530-31a5-41f2-b662-6469aed1b791" />

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (47)" src="https://github.com/user-attachments/assets/49e1eb23-ba51-47ed-9d6d-f329386d3904" />

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (48)" src="https://github.com/user-attachments/assets/52d810e9-9461-4e77-a19a-ceee12793f24" />

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (48)" src="https://github.com/user-attachments/assets/722c78e9-c8d2-41f8-8685-62a6256885d0" />

<img width="960" height="578" alt="Clearance-Test-CAD-Pic (49)" src="https://github.com/user-attachments/assets/0da59f01-4a49-4b58-90a9-1a3cec49f201" />

<video width="100%" controls>
  <source src="ClearanceTestVid2.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

The -0.3 tolerance worked the best. It was able to hold the square and it didn't take much effort to get in. The hole with no tolerance obviously did not hold the square and the hole with -0.4 mm clearance worked but was a bit tight.

<img width="4000" height="3000" alt="Clearance-Test (24)" src="https://github.com/user-attachments/assets/9c0bb4f7-0425-4842-837f-d2d1ab1d6d42" />

* No tolerance

<img width="4000" height="3000" alt="Clearance-Test (24)" src="https://github.com/user-attachments/assets/c9a3dc2a-16bb-479b-8856-590241c0f5dc" />


* -0.3 mm tolerance

<img width="4000" height="3000" alt="Clearance-Test (25)" src="https://github.com/user-attachments/assets/7982d1f9-1c06-441f-9b58-34cb664e9bfe" />

<img width="4000" height="3000" alt="Clearance-Test (26)" src="https://github.com/user-attachments/assets/31b17704-e4c7-4461-b9d7-d4da884d7b06" />

<img width="4000" height="3000" alt="Clearance-Test (27)" src="https://github.com/user-attachments/assets/b44342c2-1703-4599-ad99-8549576efcc1" />

* -0.4 mm tolerance

<img width="4000" height="3000" alt="Clearance-Test (29)" src="https://github.com/user-attachments/assets/ee444e96-815a-4137-af7d-bfd582619005" />

This led me to choosing -0.3 mm as the clearance for all of the slots.

#### Clearance Parameter Table

| Variable Name | Value Units (Measured or Chosen) | What it controls |
|---------------|---------------|---------------|
| Material Thickness | 2.74 mm (Measured) (Step 1) | Controls the "height" of fit slots |
| Kerf | 0.2 mm (Measured) (Step 2) | Controls how much larger the model needs to be to achieve the desired size |
| Clearance | -0.3 mm (Chosen) (Step 4) | Controls how tight or lose the fits are |
| Slot Width | mm (Calculated / Kerf = D - measured width) (Step 3) | Controls the width of the slot |
| Slot Height | Material thickness + kerf = 2.74 mm + 0.20 mm = 2.94 mm (Step 3) | Controls the "height" of the fit slots. Usually is the same as material thickness (plus kerf) |


### CAD Design

For my design to cut out, since it required at least eight pieces, I wanted to make something like the laser cut wood puzzles you can purchase. I wanted to make something geometric to keep the design simple. I decided to revisit something I had previously tried to 3D model. For my design, I decided to create a [Penrose Triangle](https://en.wikipedia.org/wiki/Penrose_triangle).

<img width="250" height="227" alt="Penrose-Triangle" src="https://github.com/user-attachments/assets/d582e83b-76b2-4b77-8f95-5829d51b6363" />

This time, I actually wanted to make it 3D. I started by drawing the Penrose triangle and trying to determine how many faces I would need to make. 

<img width="1275" height="1616" alt="Lab-09-Penrose_page-0001" src="https://github.com/user-attachments/assets/e8fe888c-b922-43e4-8d6f-9a5821213a37" />

I then created a simple mockup to get an idea of how it would fit together.

To start, I put in the equations for all the different parameters so I could make it parametric. 

<img width="780" height="503" alt="PenroseCadImg (1)" src="https://github.com/user-attachments/assets/b71b4230-aec9-4a09-85af-d6f258292058" />

I then simply modeled each connection without any sort of fit.

<img width="960" height="564" alt="PenroseCadImg (3)" src="https://github.com/user-attachments/assets/03910284-a883-4c00-9b7f-ab9614490cd2" />

<img width="960" height="564" alt="PenroseCadImg (4)" src="https://github.com/user-attachments/assets/9444ef04-28f2-4d1b-b881-dd2ea5fe4027" />

<img width="960" height="564" alt="PenroseCadImg (7)" src="https://github.com/user-attachments/assets/87f386fd-1521-46e0-8968-1ec8b42715f6" />

* This is the base and left side.

<img width="960" height="564" alt="PenroseCadImg (8)" src="https://github.com/user-attachments/assets/0d412e3b-5d20-43a4-b926-386685c606bd" />

<img width="960" height="564" alt="PenroseCadImg (9)" src="https://github.com/user-attachments/assets/6d6b739c-ff2a-484a-a526-6763c1b6cd28" />

* These are the end pieces.

Next, I started putting the parts together in an assembly to get an idea for how things would fit together.

<img width="960" height="564" alt="PenroseCadImg (10)" src="https://github.com/user-attachments/assets/54d0e80b-8ec4-44dd-9ec5-7f96f9238113" />

<img width="960" height="564" alt="PenroseCadImg (11)" src="https://github.com/user-attachments/assets/dc5b6308-d142-428a-8962-3c770a1efcda" />

<img width="960" height="564" alt="PenroseCadImg (12)" src="https://github.com/user-attachments/assets/8836e736-bc37-473a-9026-709f3e02a773" />

* I quickly realized I would need to account for the thickness of overlapping parts if I wanted the cross section to be square.

<img width="960" height="564" alt="PenroseCadImg (13)" src="https://github.com/user-attachments/assets/17ef3788-ed49-48e3-9d99-5e7f4454aba8" />

<img width="960" height="564" alt="PenroseCadImg (14)" src="https://github.com/user-attachments/assets/3a673a15-72c9-48f6-85bd-a3f5258501a9" />

<img width="960" height="564" alt="PenroseCadImg (15)" src="https://github.com/user-attachments/assets/aba9411d-63d6-49d8-a375-fb591ae40dda" />

<img width="960" height="564" alt="PenroseCadImg (16)" src="https://github.com/user-attachments/assets/68a98231-f7af-4459-8570-00b714d4c654" />

<img width="960" height="564" alt="PenroseCadImg (17)" src="https://github.com/user-attachments/assets/58733f3d-080e-4839-b426-60b3814e426f" />

<img width="960" height="564" alt="PenroseCadImg (18)" src="https://github.com/user-attachments/assets/14178a60-2869-41de-955c-b47e08176112" />

* This was the top and inside L face, shortened on one end since it can't go all the way through.

<img width="960" height="564" alt="PenroseCadImg (19)" src="https://github.com/user-attachments/assets/1adefd20-4ad6-4d7d-a7fb-0d5aec9786db" />

<img width="960" height="564" alt="PenroseCadImg (20)" src="https://github.com/user-attachments/assets/018723c2-dfe2-43d3-b002-944a32ff56f8" />

<img width="960" height="564" alt="PenroseCadImg (21)" src="https://github.com/user-attachments/assets/34b3defd-3dc9-4c7c-86bc-af79da5f2c24" />

<img width="960" height="564" alt="PenroseCadImg (22)" src="https://github.com/user-attachments/assets/a9576473-4705-47ef-b4dd-81bd8202c42d" />

<img width="960" height="564" alt="PenroseCadImg (23)" src="https://github.com/user-attachments/assets/17b51b91-8f0f-42ee-a4bf-9dc65cac640e" />

* I created the last rectangular faces to cover up the gaps.

Once I had a basic 3D model, I could see what I was doing and what faces I needed. So, I started designing the faces with the slots and notches that would slide into each other. I decided to go with a slot design that was open on one side so the parts would fit together seamlessly and there would be no overlapping.

* I Started with the base again. The method I went for was to have a slot in the middle of each edge of the base. This would give me a reference for how the other parts would need to look. I tried to design as few parts as possible. However, all the L sections fit together weird and I needed to design a new one each time.

<img width="960" height="564" alt="PenroseCadImg (26)" src="https://github.com/user-attachments/assets/ae8984cb-068c-4726-8c3e-e6166243d97d" />

<img width="960" height="564" alt="PenroseCadImg (27)" src="https://github.com/user-attachments/assets/f4dff634-7061-4ab4-b81c-c926507e5256" />

<img width="960" height="564" alt="PenroseCadImg (28)" src="https://github.com/user-attachments/assets/284f10dd-d336-439f-87fe-4db1113fc438" />

* With the base in place, I decided to mess with the equations and sizing a bit. I made the total length longer and a function of the width, making sure to account for kerf and the thickness of the other parts.

* I defined new equations for the width of parts that would be in between two others. 

<img width="780" height="503" alt="PenroseCadImg (30)" src="https://github.com/user-attachments/assets/2449304a-5196-4b1d-9ac8-858073162f76" />

* Another important factor with the equations was the fact that I was importing the same equations into each separate Solidworks file. This made every file have the same equations and these equations were dependant on the text file from the original export. This would turn out to be very helpful later.

* The second part I modeled was that left side L piece that would fit into the base. Since it was going to be sandwiched between two parts, it needed to have the thinner thickness that accounted for the material thickness. 

<img width="960" height="564" alt="PenroseCadImg (32)" src="https://github.com/user-attachments/assets/84b5031c-b01e-418e-9947-8a0d8e3c0790" />

<img width="960" height="564" alt="PenroseCadImg (33)" src="https://github.com/user-attachments/assets/293c8ca6-69fc-4a3a-a6e2-c7b7c85f7098" />

<img width="960" height="564" alt="PenroseCadImg (34)" src="https://github.com/user-attachments/assets/368f4982-f12c-416f-992a-37d7c3309951" />

<img width="960" height="564" alt="PenroseCadImg (35)" src="https://github.com/user-attachments/assets/c31e5994-1ef8-4ca7-ac06-dbd3428e3fc8" />

* With the piece designed, I could then put the pieces together in an assembly to see how it fit together.

<img width="960" height="564" alt="PenroseCadImg (36)" src="https://github.com/user-attachments/assets/25258566-5233-4a5e-846a-236bb0a274e2" />

Having the assembly made the whole project significantly easier since it was very easy to see how things were going to fit together. 

* Next I designed one of the basic wall pieces that I was able to use twice, saving me some time.

<img width="960" height="564" alt="PenroseCadImg (37)" src="https://github.com/user-attachments/assets/c532d16c-4bd9-4e51-b6fc-fb873d0fe8a7" />

<img width="960" height="564" alt="PenroseCadImg (38)" src="https://github.com/user-attachments/assets/8e0e1d45-f47f-48c2-b9ce-3b6f95ba6b4e" />

<img width="960" height="564" alt="PenroseCadImg (39)" src="https://github.com/user-attachments/assets/df022c66-6706-4aea-97b1-c69c735b6a32" />

I did have to adjust the measurements slightly in order to get the piece to fit. Another reason the assembly was incredibly helpful. 

<img width="960" height="564" alt="PenroseCadImg (40)" src="https://github.com/user-attachments/assets/7695e42d-7e67-46fa-a4c8-cfc47268fbbc" />

* I needed to adjust the length so that the total length from the end of the slots would be the total length.

<img width="960" height="564" alt="PenroseCadImg (41)" src="https://github.com/user-attachments/assets/88405793-3ecd-4504-900b-efab7588af16" />

<img width="960" height="564" alt="PenroseCadImg (42)" src="https://github.com/user-attachments/assets/612fd021-626b-42c8-9bff-a57c0252c87f" />

* I could then use one to fill in the back as well.

* The next piece I made was a shortened version for the other spaces.

<img width="960" height="564" alt="PenroseCadImg (43)" src="https://github.com/user-attachments/assets/d7017937-91dd-4d65-acfc-dbec863cf027" />

<img width="960" height="564" alt="PenroseCadImg (44)" src="https://github.com/user-attachments/assets/25ef97e1-756e-492f-953e-c4bd3b42e73a" />

<img width="960" height="564" alt="PenroseCadImg (45)" src="https://github.com/user-attachments/assets/682e5426-c50a-4c9b-a261-19332dcdba7e" />

I again had to play around with the length of the part to make the slots line up properly. 

<img width="960" height="564" alt="PenroseCadImg (46)" src="https://github.com/user-attachments/assets/a454c0c4-eee4-430a-826b-694d0cd4d0b4" />

<img width="960" height="564" alt="PenroseCadImg (47)" src="https://github.com/user-attachments/assets/747b6b97-b3db-42d4-9974-de4be85e3fb2" />

<img width="960" height="564" alt="PenroseCadImg (48)" src="https://github.com/user-attachments/assets/c2f2d2d6-3d43-4c7d-a293-92d58ae67fa1" />

<img width="960" height="564" alt="PenroseCadImg (50)" src="https://github.com/user-attachments/assets/8069b565-5b54-4b13-aa6f-29bb4b338559" />

* I used the part again for the front of the vertical piece.

* The next part was the top L piece to cover the top.

<img width="960" height="564" alt="PenroseCadImg (55)" src="https://github.com/user-attachments/assets/be4893ed-a2a7-427c-9447-350068ef9c50" />

<img width="960" height="564" alt="PenroseCadImg (56)" src="https://github.com/user-attachments/assets/17b5ea02-5644-4b36-a789-2ef6cde47db2" />

<img width="960" height="564" alt="PenroseCadImg (57)" src="https://github.com/user-attachments/assets/3c07962f-2090-4b7c-ab5b-6421ccb7aa68" />

<img width="960" height="564" alt="PenroseCadImg (59)" src="https://github.com/user-attachments/assets/355092e9-06f3-49f8-a128-beb915536ee1" />

* I would need to do some more modifications to the part to make it fit in, but I did that later and instead made the next side L piece by creating a copy of the top piece I had just made and filling in some of the gaps and changing the thickness.

<img width="960" height="564" alt="PenroseCadImg (60)" src="https://github.com/user-attachments/assets/5f4d4038-085c-4aab-a21a-79961b13daa5" />

<img width="960" height="564" alt="PenroseCadImg (61)" src="https://github.com/user-attachments/assets/eb7a9fcc-48dc-4f99-8ccd-c2001441f15b" />

<img width="960" height="564" alt="PenroseCadImg (63)" src="https://github.com/user-attachments/assets/19b6f701-2125-4a8e-b14c-bceaed4a515b" />

* I had to extend the end because it was fitting inside the the corner.

<img width="960" height="564" alt="PenroseCadImg (64)" src="https://github.com/user-attachments/assets/8a72b212-95cc-41ac-87e5-2801d0c5e550" />

<img width="960" height="564" alt="PenroseCadImg (65)" src="https://github.com/user-attachments/assets/d9081335-a29b-4b43-8600-0f3b2239f203" />

* I then switched and made the changes to the top part to make it fit in better.

<img width="960" height="564" alt="PenroseCadImg (66)" src="https://github.com/user-attachments/assets/d393d920-cc81-43e6-abf1-f6fcb5ca32d4" />

<img width="960" height="564" alt="PenroseCadImg (67)" src="https://github.com/user-attachments/assets/6a6e7435-d70a-464b-bfeb-302ddbe31813" />

<img width="960" height="564" alt="PenroseCadImg (68)" src="https://github.com/user-attachments/assets/d4ad5c8c-4bb3-44bd-95b7-3d8f5bdf04db" />

<img width="960" height="564" alt="PenroseCadImg (69)" src="https://github.com/user-attachments/assets/defd23b0-bf7d-49bf-86a5-061177ec8e4e" />

<img width="960" height="564" alt="PenroseCadImg (70)" src="https://github.com/user-attachments/assets/52b76138-87da-43c9-b6a5-735c5089b19b" />

* Here are the two piece added to the assembly.

* The final part to model was the ends.

<img width="960" height="564" alt="PenroseCadImg (70)" src="https://github.com/user-attachments/assets/e60df238-aba0-41f7-9ea8-b528b07dd611" />

<img width="960" height="564" alt="PenroseCadImg (71)" src="https://github.com/user-attachments/assets/a46f377c-cacf-4f5d-98e1-89332a7b1739" />

<img width="960" height="564" alt="PenroseCadImg (72)" src="https://github.com/user-attachments/assets/195743e3-5721-4cd5-ae97-5888b6d83f5b" />

* This part was too large to fit in properly so I had to remove the ends.

<img width="960" height="564" alt="PenroseCadImg (73)" src="https://github.com/user-attachments/assets/ec458261-65a7-4ece-aa55-6c4112e52bc8" />

<img width="960" height="564" alt="PenroseCadImg (75)" src="https://github.com/user-attachments/assets/dd2346c8-41ff-4012-971c-8fa44449b34b" />

With that finished, the modeling was done. And I had a pretty good idea of what the final product would look like. 

<img width="960" height="564" alt="PenroseCadImg (77)" src="https://github.com/user-attachments/assets/53e6bf3e-b048-402c-a2db-825117b912d4" />

<img width="960" height="564" alt="PenroseCadImg (78)" src="https://github.com/user-attachments/assets/92fc1b6e-d4e4-445b-89b6-2705796a9d1d" />

Next it was onto exporting the files into Inkscape and cutting out the pieces. 


## Manufacturing

#### Process Research

Laser cutting is a viable manufacturing process due to it's flexibility. Laser cutters are able to cut through thin materials very quickly and precisely. Laser cutters can also etch or engrave materials. Comparing laser cutting to an additive manufactiring process like FDM 3D Printing, laser cutters are really only good at cutting 2D shapes and are very geometrically limited. 3D Printers have access to all 3 axis, giving them a lot more flexibility. However, 3D FDM Printers are limited to plastic filaments. Laser cutters can cut and engrave a wider range of metals, woods and acrylic. Both are good manufacturing processes with their own strengths and weaknesses. 

### Design Cutting

The manufacturing was fairly straight forward. The only tricky part was figuring out the clearances. Since I has changed my design of the slots from a closed design to an open design, that changed the clearances needed to hold the parts together. So, to start with, I cut out a couple test parts to see where the clearances were at. 

* I inserted the first dxf files into Inkscape and print the base and two of the larger faces.

<img width="430" height="418" alt="PenroseCadImg (80)" src="https://github.com/user-attachments/assets/912fbb3a-142a-4208-be8b-b9d723ec8e2d" />

<img width="430" height="418" alt="PenroseCadImg (89)" src="https://github.com/user-attachments/assets/6124ce0b-6bb3-4663-8c25-032a779a714d" />

<img width="430" height="418" alt="PenroseCadImg (85)" src="https://github.com/user-attachments/assets/256bb2b2-66f4-497d-9ec2-afff337f6207" />

<img width="960" height="564" alt="PenroseCadImg (83)" src="https://github.com/user-attachments/assets/fe7b93ac-de5f-4611-8e6c-d5f4882b466c" />

<img width="955" height="584" alt="PenroseCadImg (84)" src="https://github.com/user-attachments/assets/74b6f6e0-492d-48d1-9237-8d3d441b8173" />

I then loaded it onto the laser cutter and let it run. 

<video width="100%" controls>
  <source src="PenroseVidFinal2.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

* _Video sped up to 1.5x Speed_

And with the initial cuts, the pieces did not hold together at all. The slots were way too large. I needed to lower them quite a bit. 

This is when I realized that I had never updated my clearence from my original equations. This meant it was left at -0.2 mm. 

<img width="593" height="551" alt="PenroseCadImg (95)" src="https://github.com/user-attachments/assets/63150981-de1b-4c05-b29b-68820f4933ea" />

This is where having all of the equations bound to the file came in very helpful. I could just change the file value and all of the equations across all of the models would update. 

I tried a couple of cuts with different clearances and decided on -0.5 mm as the ideal clearance. 

<img width="593" height="551" alt="PenroseCadImg (94)" src="https://github.com/user-attachments/assets/8d1f64f1-1d90-41ef-8f9c-c06485e03021" />

<img width="960" height="564" alt="PenroseCadImg (88)" src="https://github.com/user-attachments/assets/ed0bcf81-f5f5-4f3a-a936-dfc3d420fb67" />

This changed the width of the slots from 9.8 mm down to 9.3 mm. 

<img width="960" height="564" alt="PenroseCadImg (90)" src="https://github.com/user-attachments/assets/613a9108-d123-4c3d-a1ec-d0a69453589f" />

<img width="950" height="584" alt="PenroseCadImg (92)" src="https://github.com/user-attachments/assets/ad5dd6d4-92ec-4740-821d-2c67eb93ac36" />

I then cut the rest of the parts on one cut that took about a minute and a half. 

<video width="100%" controls>
  <source src="PenroseVidFinal3.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

* _Video sped up to 4x Speed_

Once I had all of the parts, I could start asssembling the final structure.

<img width="3000" height="4000" alt="PenrosePic (2)" src="https://github.com/user-attachments/assets/7b3041dc-6ed6-4679-bd7f-b1e8026764f2" />

<img width="3000" height="4000" alt="PenrosePic (3)" src="https://github.com/user-attachments/assets/389d1155-a831-4317-88a0-252fe77dbd4c" />

<img width="3000" height="4000" alt="PenrosePic (5)" src="https://github.com/user-attachments/assets/7b7d4b52-aa99-4a38-9a73-4d97b43a54ff" />

Once I had the tolerances good enough to hold the pieces together, everything fit together perfectly.

There generally wasn't a strict process to how I laid out my parts. I mainly prioritzed getting them as close together and using as litte space and materiala as possible. 

There were never any issues with the quality of the sides. The sides were always a little burnt but it wasn't too bad so I never tried to correct the side quality. 

And if you hold it just right, you can kind of get the illusion to work.

<img width="2668" height="2322" alt="PenrosePic (15) - copy" src="https://github.com/user-attachments/assets/76cfc3b6-61e1-4104-acc8-cb223a6d695c" />


#### Laser Process Record

| Setting | Kerf coupon | Fit Coupon | Final Cut |
|---------------|---------------|---------------|---------------|
| Laser Cutter | SFL 5 | SFL 5 | SFL 5 |
| Material Type | Wood | Wood | Wood |
| Nominal Thickness | 3 mm | 3 mm | 3 mm |
| Measured Thickness (mm) | 2.74 | 2.74 | 2.74 |
| Speed | 20% | 20% | 20% |
| Power | 100% | 100% | 100% |
| Frequency | 20% | 20% | 20% |
| Number of Passes | 1 Pass | 1 Pass | 1 Pass |
| Focus Method and how it was confirmed | Manually using the pointer piece | Manually using the pointer piece | Manually using the pointer piece |
| Air assist on? Exhaust on? | Both On | Both On | Both On |
| How the origin and alignment were set | Automatically | Automatically | Automatically |

## Lessons Learned

This assignment taught me a lot about laser cutting and the differences between additive manufacturing and subtractive manufacturing. Kerf was a very knew and different parameter to think about. It certainly altered the way I had to think about this design versus previous designs. Obviously, I learned a lot about laser cutting, such as the procedures, software, and focusing. Inkscape was a very different software to figure out. I had to learn about the geometric versus visual boundary settings in Inkscape to make sure my parts were of the correct size. I even learned more about equations in Solidworks with how altering the files can change the settings in every file that has those imported settings. Overall, this assignment was completely different from any other assignment thus far and it taught me a lot more about engineering processes. 

1: Where did your measured values differ from what you assumed (nominal thickness, expected kerf)? What would have happened if you had used the assumed value?

The primary place the expected values differed from the actual values was in the nominal thickness. The actual thickness was less then the nominal thickness. Had I used the nominal thickness, my designs would be off since they are dependent on the thickness of the sheet. Every parameter would be wrong and the cut would likely not turn out well.

2: Using Taguchi's quality loss function, describe one joint in your kit that works but is not on target. What would that loss mean if the part were made by the thousands?

A couple joints are a bit tight. While the clearance worked well for most of the parts, some of the other parts came out much tighter. If this part were to be made by the thousands, there would certainly be more struggle and time taken in the assembly portion of the manufacturing process. 

3: Name a real product that uses cut sheet parts joined by tabs and slots (for example, flat pack furniture or sheet metal enclosures). How would a kerf or thickness error show up for the customer?

Some Cabinets, bookshelves, and other furniture often uses tabs and slots to easlily join the parts together. If there was a kerf orr thickness error, the furniture would likely be more difficult to assemble or it wouldn't fit together at all. 

4: If you had one more cut, what would you change, and why?

I would probably optimize the tolerances more to try and make the pieces fit together even better. 


### Process Log

**Process Log**

| Date and Time Spent | Step | What happened | Decision or change made |
| 10/23/2026 1 Hrs | Step 1 | Designed kerf coupon | Decided on size of coupon (20 x 20 mm) |
| 10/23/2026 0.5 Hrs | Step 2 | Measured kerf coupon | Determined kerf to use for all following desings |
| 10/23/2026 2 Hrs | Step 3 - 4 | Designed and iterated fit coupon | Made iterations and changed clearances until suitable clearance was found |
| 10/26/2025 1.5 Hrs | Step 5 | Cut out final design. | Altered clearances until the parts fit together nicely. |

**Total Time Spent:** 13 Hours

**1 Sheet Used**

## Resources

[Penrose Triangle](https://en.wikipedia.org/wiki/Penrose_triangle)
