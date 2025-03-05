---
title: "Microfluidic Device"
excerpt: "This resin printed microfluidic device is capable of sorting particles (125 – 150 μm and 425 – 500 μm) with pinch flow fractionation."

header:
  image: assets/img/uFluidic Model Render.jpg
  teaser: assets/img/uFluidic Model Render.jpg
gallerym:
  - image_path: assets/img/uFluidic Model Render.jpg
galleryc:
  - image_path: assets/img/uFluidic Model Render.jpg

   
---
<br>
## Introduction
### Microfluidic Devices
Microfluidic devices are systems that manipulate very small volumes of liquids through channels to perform a variety of chemical and biological analyses. They are widely used for biomedical diagnoses, drug delivery, and chemical synthesis. Using a microfluidic device allows for reduced reagent consumption and rapid processing times.

### Pinch Flow Fractination
Pinch flow fractination (PFF) is a microfluidic technique used for sorting particles based on size. As the flow enters the pinched region, the particles align to the walls due to hydrodynamic forces. The position of the particles in the pinched region depends on their size, and when the pinched region transitions to the broad region, the particles follow along their streamline and are sorted into the various outlet channels. One specific application of PFF is in cancer detection. Based on a 2009 article by Xu et al., PFF was used to sort multiple types of cancer cells from a complex sample, allowing for early cancer detection in patients ([Aptamer-Based Microfluidic Device for Enrichment, Sorting, and Detection of Multiple Cancer Cells](https://pubs.acs.org/doi/10.1021/ac9012072)).


## Design Instructions

**1. CAD Model**<br>

The first step in fabricating the microfluidic device was creating the CAD model. The device, when molded, is precisely 25 mm wide and 75 mm long, allowing it to sit flush on a common microscope slide. Some design constraints included maintaining an aspect ratio less than 4:1, keeping inlets and outlets a minimum of 11 mm away from each other so that the barbs don't intersect, and maintaining a 3 mm buffer region around the edge of the device to allow for sufficient bonding to the glass slide. For the channel design, the inlets intersect at 45 degree angles from the horizontal, the pinched region is 1.5 times the diameter of the largest particle, and the broad region is wide enough to allow for four equally wide channels. 

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a498a7e80bce8385f9?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

<br>

**2. Print and Cure Mold**<br>

This CAD model was then SLA printed with high temperature resin. A 0.05 mm layer height was configured, and the bottom of the mold was placed parallel with the resin vat to allow for a perfectly flat bottom layer. Once printed, the device was rinsed in the FormWash for 5 minutes on the print bed and an additional 5 minutes off of the print bed. Then, the device was air dried for 30 minutes before undergoing a 60 second surface cure at room temperature. Once cured, the supports from the device were removed.

<br>

PICTURE OF MOLD
{% include gallery id="gallerym" caption="Microfluidic Device Mold" %}


**3. Parylene Coating**<br>

Next, the microfluidic device was coated in a thin layer of parylene, which is a biocompatible and chemically resistant polymer. The coating process occurs through chemical vapor deposition, enhancing durability of the device.
<br><br>


**4. Cast PDMS**<br>

Then, polydimethylsiloxane (PDMS) was mixed with a curing agent, placed into a vacuum chamber to remove bubbles, and poured into the SLA printed mold. The PDMS was cured at an elevated temperature for a few hours until it solidfied, at which point it was carefully peeled from the mold. 
<br>

PICTURE OF CASTED DEVICE
{% include gallery id="galleryc" caption="Casted Microfluidic Device" %}


**5. Plasma Bond Glass Slide**<br>
Lastly, the PDMS and glass slide were treated with oxygen plasma and immediately pressed together to form a strong, irreversible bond. Once bonded, the device was ready for testing. 


## Final Design

EMBEDDED YOUTUBE OF DEVICE WORKING


## Discussion


* Why are resin-printed molds coated with parylene prior to casting the PDMS? 
What are 
hypothetical applications of your microfluidic mixer or sorter? 
• Why is your geometry conducive to sorting? Discuss specific dimensions (pinch width, 
outlet width, location of ports, etc.) 
• What steps or design features did you use to ensure that each outlet received the same flow rate, preventing disruptions to the streamlines and maintaining proper separation? 


* Based on the results of testing, could you implement any future changes to improve 
sorting? 

