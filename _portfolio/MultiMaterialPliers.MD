---
title: "Multi-Material Pliers"
excerpt: "These 3D-printed multi-material pliers are capable of picking up and moving objects as small as resistors."

header:
  image: assets/img/Plier Render 2.png
  teaser: assets/img/Plier Render 2.png
gallery1:
  - image_path: assets/img/Plier Print 1.jpg
gallery2:
  - image_path: assets/img/Plier Flexible 1.png
  - image_path: assets/img/Plier Flexible 2.png
gallery3: 
  - image_path: assets/img/Plier Print 2.jpg
gallery4: 
 - image_path: assets/img/Plier GIF.gif

   
---
<br>
## Introduction

The goal of this project was to design and print pliers that are capable of gripping and picking up through-hole resistors. Typically, this would be accomplished using the print-in-place technique. This is when multi-component models are functional immediately upon being removed from the print bed. Print-in-place requires proper clearance between the joints, but single-material models can often be more rigid than desired due to irregularities of plastic extrusion. <br><br>
To solve this problem, a second material can be printed simultaneously using a multi-material printer. One material combination that works well in this scenario is polylactic acid (PLA) and thermoplastic polyurethane (TPU). Another material combination that works well for print-in-place is PLA and polyvinyl alcohol (PVA). PVA is a dissolvable support material, making it ideal for internal supports or nested parts. Print-in-place has been used in creating medical models (using PLA for bones and TPU for tissues/muscles), interactive toys (using PLA for the casing an TPU for the buttons), robotic grippers (using PLA for the frame and TPU for expanding/contracting grippers), and beyond. <br><br>
For this project specifically, the rigid and flexible components of the pliers were printed separately and then assembled after printing due to not having access to a multi-material printer.

## Design Process

For the first design iteration, the jaws of the pliers were modeled off of slip joint pliers, where the tip is flat, and just below the tip the jaws are curved out. These pliers are often used for crimping metal or loosening/tightening nuts and bolts. The tip of the jaws was angled slightly such that they would be flush against each other when the pliers were closed. Next, the flexible section of the pliers was modeled off of previous students’ designs, with a simple grid that allowed for flexibility up to the size of the gaps in the part width. Lastly, the handles of the pliers were curved so that they were smooth and easy to hold. To connect the flexible middle to the rigid components, five interlocking finger joints were used on each edge. <br>

{% include gallery id="gallery1" %}

While the jaws and handles of the pliers seemed like they would function well, the connection between the rigid and flexible parts was not ideal. The components would not stay interlocked due to the size of and clearance between the joints. <br>

To address this, four changes were made: 
1. The number of finger joints was reduced to four and the size of the joints increased. 
2. The joint angle was changed from 60 degrees to 70 degrees so that the joints would have greater contact with each other. 
3. The clearance between parts was decreased from 0.15 mm to 0.10 mm so that the joints would have a tighter fit.
4. The grid thickness was reduced from 1 mm to 0.6 mm to help improve the flexibility of the TPU-printed part.

{% include gallery id="gallery2" caption="1) Initial Flexible Middle Design; 2) Final Flexible Middle Design" %}

### Final Design <br>
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4cd3be0f6b01248d7?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
<br><br>
With the four changes made, the final design was complete! The pliers are capable of picking up and moving resistors, and in a 30 second challenge, they were able to move 14 resistors. Of note, none of the standard PLA and TPU print settings were changed in this design.<br>

{% include gallery id="gallery3" %}

**Plier Specifications**
* Jaw length = 49.23 mm
* Maximum distance between jaws = 16.62 mm
* Flexible middle width (diagonal) = 35.36 mm
* Handle length = 88.47 mm
* Maximum distance between handles = 61.73 mm

{% include gallery id="gallery4" %}
