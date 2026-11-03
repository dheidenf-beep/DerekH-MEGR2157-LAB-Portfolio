# A10 – SLA RC2 Fit

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

### RC2 Fit Applications

RC 2 sliding and running fits are the second tightest running sliding fits after RC 1 fits. RC 2 fits, from the description in the Machinery's Handbook, are meant to be for parts that allow movement but are not meant to run freely. This applies mainly to applications that need some movement but aren't spinning fast or need precision and friction to hold in place. Mechanisms that are manually adjusted benefit from RC 2 fits. RC 2 fits can be found in switches for a sliding fit that only moves occasionally, telescoping mechanisms which need precision and don't move a lot, and pulleys or gears that are for manually adjusting systems. The RC 2 fit provides a good middle ground between not allowing parts to move at all and not allowing parts to move too much for more precise or manual applications.


## CAD Design



## Preprocessing


## Printing


## Lessons Learned



