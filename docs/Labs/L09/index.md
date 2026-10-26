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

**_INSERT VIDEO_**

<img width="4000" height="3000" alt="Clearance-Test (14)" src="https://github.com/user-attachments/assets/5679411f-a682-484f-a2e1-929c09cf740e" />

The cut turned out well but due to my larger dimensions, the slots were too wide.

I ended up creating another three cuts before I found a clearance that worked. 

<img width="4000" height="3000" alt="Clearance-Test (19)" src="https://github.com/user-attachments/assets/7ddb56b4-8fd2-484b-9c07-287b58d19607" />

For the final design, I decided to test two tighter tolerances since I had shortened the width of the slot to be the actual width of the square with kerf accounted for<img width="960" height="564" alt="Clearance-Test-CAD-Pic (47)" src="https://github.com/user-attachments/assets/27b54073-9997-4a70-8ae6-5a66c090fc7b" />
 and tested tolerances from -0.1 mm to -0.3 mm.

<img width="780" height="503" alt="Clearance-Test-CAD-Pic (46)" src="https://github.com/user-attachments/assets/c18ac530-31a5-41f2-b662-6469aed1b791" />

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (47)" src="https://github.com/user-attachments/assets/49e1eb23-ba51-47ed-9d6d-f329386d3904" />

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (48)" src="https://github.com/user-attachments/assets/52d810e9-9461-4e77-a19a-ceee12793f24" />

<img width="960" height="564" alt="Clearance-Test-CAD-Pic (48)" src="https://github.com/user-attachments/assets/722c78e9-c8d2-41f8-8685-62a6256885d0" />

<img width="960" height="578" alt="Clearance-Test-CAD-Pic (49)" src="https://github.com/user-attachments/assets/0da59f01-4a49-4b58-90a9-1a3cec49f201" />

**_FINAL VIDEO_**

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
|---------------|---------------|---------------|
|---------------|---------------|---------------|


### CAD Design





## Manufacturing



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
| Focus Method and how it was confirmed |---------------|---------------|---------------|
| Air assist on? Exhaust on? | Both On | Both On | Both On |
| How the origin and alignment were set |---------------|---------------|---------------|

## Lessons Learned



### Process Log

**Process Log**

| Date and Time Spent | Step | What happened | Decision or change made |
| 10/23/2026 1 Hrs | Step 1 | Designed kerf coupon | Decided on size of coupon (20 x 20 mm) |
| 10/23/2026 0.5 Hrs | Step 2 | Measured kerf coupon | Determined kerf to use for all following desings |
| 10/23/2026 2 Hrs | Step 3 - 4 | Designed and iterated fit coupon | Made iterations and changed clearances until suitable clearance was found |
| 10/25/2026 3.5 Hrs | Step  |---------------|---------------|
| 10/23/2026 3.5 Hrs |---------------|---------------|---------------|

