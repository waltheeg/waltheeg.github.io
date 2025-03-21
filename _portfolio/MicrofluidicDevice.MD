---
title: "Microfluidic Device"
excerpt: "This resin printed microfluidic device is capable of sorting particles (125 – 150 μm and 425 – 500 μm) with pinch flow fractionation."

header:
  image: assets/img/uFluidic Model Render.jpg
  teaser: assets/img/uFluidic Model Render.jpg
gallerym:
  - image_path: assets/img/uFluidic Mold.jpg
galleryc:
  - image_path: assets/img/uFluidic Casted Device.jpg

   
---
<br>
## Introduction
### Microfluidic Devices
Microfluidic devices are systems that manipulate very small volumes of liquids through channels to perform a variety of chemical and biological analyses. They are widely used for biomedical diagnoses, drug delivery, and chemical synthesis. Using a microfluidic device allows for reduced reagent consumption and rapid processing times.

### Pinch Flow Fractination
Pinch flow fractionation (PFF) is a microfluidic technique used for sorting particles based on size. As the flow enters the pinched region, the particles align to the walls due to hydrodynamic forces. The position of the particles in the pinched region depends on their size, and when the pinched region transitions to the broad region, the particles follow along their streamline and are sorted into the various outlet channels. One specific application of PFF is in cancer detection. Based on a 2009 article by Xu et al., PFF was used to sort multiple types of cancer cells from a complex sample, allowing for early cancer detection in patients ([Aptamer-Based Microfluidic Device for Enrichment, Sorting, and Detection of Multiple Cancer Cells](https://pubs.acs.org/doi/10.1021/ac9012072)).


## Design Instructions

**1. CAD Model**<br>

The first step in fabricating the microfluidic device was creating the CAD model. The device, when molded, is precisely 25 mm wide and 75 mm long, allowing it to sit flush on a common microscope slide. Some design constraints included maintaining an aspect ratio less than 4:1, keeping inlets and outlets a minimum of 11 mm away from each other so that the barbs don't intersect, and maintaining a 3 mm buffer region around the edge of the device to allow for sufficient bonding to the glass slide.<br>

For the channel design, the inlets intersect at 45 degree angles from the horizontal to allow for even mixing, the pinched region is 1.5 times the diameter of the largest particle (0.75 mm), and the broad region is wide enough (16 mm) to allow for four equally wide channels (3.067 mm each). This channel size was based on the size of the streamline for the smallest particles from the equation Y=(wP-(D/2))*(wB/wP).<br>

The design allows for optimal particle sorting because it maintains proper separation between the particle sizes and doesn't disrupt the streamline in the gaps (a pointed triangle was used to split the streamlines). Four channels were used to accommodate small particles, large particles, and excess buffer fluid. It was impossible to ensure each outlet received the same flow rate since the channels are different lengths (to accommodate the barb diameters), but by having two channels dedicated to removing buffer fluid, the streamlines including particles shouldn't be affected.<br>

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a498a7e80bce8385f9?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

<br>

**2. Print and Cure Mold**<br>

This CAD model was then SLA printed with high temperature resin. A 0.05 mm layer height was configured, and the bottom of the mold was placed parallel with the resin vat to allow for a perfectly flat bottom layer. Once printed, the device was rinsed in the FormWash for 5 minutes on the print bed and an additional 5 minutes off of the print bed. Then, the device was air dried for 30 minutes before undergoing a 60 second surface cure at room temperature. Once cured, the supports from the device were removed.
<br>

{% include gallery id="gallerym" caption="Microfluidic Device Mold" %}


**3. Parylene Coating**<br>

Next, the microfluidic device was coated in a thin layer of parylene, which is a biocompatible and chemically resistant polymer. The coating process occurs through chemical vapor deposition. The coating process is necessary to create a smooth, non-stick, and chemically inert, surface. Coating enhances the durability of the device and makes it easier to peel off the cured PDMS without damaging the mold or microstructures.
<br><br>


**4. Cast PDMS**<br>

Then, polydimethylsiloxane (PDMS) was mixed with a curing agent, placed into a vacuum chamber to remove bubbles, and poured into the SLA printed mold. The PDMS was cured at an elevated temperature for a few hours until it solidified, at which point it was carefully peeled from the mold. 
<br>

{% include gallery id="galleryc" caption="Casted Microfluidic Device" %}


**5. Plasma Bond Glass Slide**<br>

Lastly, the PDMS and glass slide were treated with oxygen plasma and immediately pressed together to form a strong, irreversible bond. Once bonded, the device was ready for testing. 



## Discussion

This microfluidic device is applicable in a wide range of fields. In the biomedical field, the device could be used to separate different sized blood components. More specifically, it could separate immune cells from smaller red blood cells for disease diagnostics. In the environmental field, the device could be used to categorize microplastics in the water. In the industrial field, the device could be used to remove unwanted particle contaminants in liquids.<br><br>

While my specific device was not tested, one problem that was noted with other similar devices was a backflow effect when the collection tubing wasn't held vertically. A solution to this would be creating a stand to hold the tubes up while the device is being tested. A second issue that was noticed was uneven flow rates between the channels. This caused particles to be sorted incorrectly since the streamlines were disrupted. One solution to this would be to curve some of the channels to ensure they are the same length while also leaving space for all of the barbs. Another solution would be to use collection barbs and tubing of equal resistance. Since there were not four barbs, one of the collection wells was left to leak out, and this uneven resistance led to disrupted streamlines.

