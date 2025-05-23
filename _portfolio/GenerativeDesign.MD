---
title: "Generative Design Palm Pen Holder"
excerpt: "This SLS printed palm pen holder helps those with a variety of disabilities to be able to write independently."

header:
  image: assets/img/GD Header.jpg
  teaser: assets/img/GD Header.jpg
gallery1:
  - image_path: assets/img/GD MMC.jpg
gallery2:
  - image_path: assets/img/GD Preserve.png
gallery3: 
  - image_path: assets/img/GD Obstacle.png
gallery4: 
  - image_path: assets/img/GD I1.png
  - image_path: assets/img/GD I2.png
  - image_path: assets/img/GD I3.png
gallery5: 
  - image_path: assets/img/GD I4.png
  - image_path: assets/img/GD I5.png
  - image_path: assets/img/GD I6.png
gallery6: 
  - image_path: assets/img/GD FFM Compare.png
gallery7: 
  - image_path: assets/img/GD FFM Weight 1.jpg
  - image_path: assets/img/GD FFM Weight 2.jpg
  - image_path: assets/img/GD SLS Weight.jpg
gallery8: 
  - image_path: assets/img/GD Lightbox.jpg
  - image_path: assets/img/GD Spin.gif
gallery9: 
  - image_path: assets/img/GD Use.gif
   
---
<br>
## Device Overview

My generative design project is a lightweight palm pen holder. This adaptation is very useful for individuals who have difficulty gripping standard pencils and pens due to a variety of conditions. Potential users of a palm pen holder include those with arthritis, cerebral palsy, stroke, muscular dystrophy, spinal cord injury, or limb difference.<br><br>

This device was initially designed by Makers Making Change [(MMC Palm Pen Holder)]( https://www.makersmakingchange.com/s/product/palm-pen-holder/01tJR00000068z8YAA). One drawback of their design is that it is not lightweighted most optimally. By using generative design, the palm pen holder can be designed to be even lighter. This is especially helpful for those with neuromuscular disorders as they would be able to write for longer if they had a lighter device.

{% include gallery id="gallery1" caption="Makers Making Change's Palm Pen Holder" %}

Makers Making Change is a Canadian-based organization that makes affordable assistive technology for those with disabilities. This organization is extremely similar to Tikkun Olam Makers (TOM), which operates in over 35 countries. Vanderbilt has one of the 70+ university chapters of TOM, and I have been fortunate enough to lead the chapter for the past three semesters. Through my work with TOM, I have seen how important it is to continually improve upon existing assistive technologies to help meet the needs of those with disabilities. 


## Generative Design Set-Up

### Preserve Geometries
* Curved cuff
* Pen cylinder
* Hex nut box
* Bolt cylinder
* Bolt head cylinder

{% include gallery id="gallery2" %}

### Obstacle Geometries
* Hand (space inside cuff)
* Pen
* Hex nut
* Bolt
* Bolt head

{% include gallery id="gallery3" %}

### Structural Constraints
A fixed constraint was added to the bolt cylinder as it was an interface between my part and surrounding parts. This made it so that the cylinder was not translated or rotated at all, ensuring that the bolt would line up with the nut and hole in the pen shaft.

### Load Cases 
<br>
Table of Forces:

| **Force** | **Magnitude** | **Location** | **Rational** |
|:---------:|:----------:|:-------------:|:-------------:|
| Hand Force | 10 N | Bottom of cuff | When writing, the user’s hand will exert a force downwards on the bottom of the cuff. |
| Hand Pressure | 0.10 MPa | Front and back cuff faces | When gripping the device, the user’s hand will compress the cuff. |
| Pen Moment | 0.40 Nm | Inside of pen shaft | When inserting and tightening, or when writing, the pen will exert a moment on the pen shaft. |


<br>The direction and location of each load was determined by visual inspection on the MMC model. The magnitude of each load was influenced by AI’s suggestions. To further refine the loads, this device could be printed and used for a period of time by an individual with a disability before determining where the weakest points are.

### Design Iterations

{% include gallery id="gallery4" caption="Iterations 1-3" %}
{% include gallery id="gallery5" caption="Iterations 4-6" %}

## Final Design

### Weight Comparison
While the final model was SLS printed, a prototype was FFM printed to conduct a weight comparison. The original model weighed 29 g, and the generative design model weighed 18 g. This results in a 37.93% decrease in weight! Of note, this difference would likely be higher if the original model were printed with 100% infill as the generative design model was printed. <br><br>

{% include gallery id="gallery6" %}

When SLS printed, the final model weighed 17 g, a 41.38% reduction when compared to the original FFM model. 

{% include gallery id="gallery7" %}

### CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a448c2918c3c047465?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

### SLS Print

{% include gallery id="gallery8" %}

{% include gallery id="gallery9" %}

## Critique of Generative Design
Generative design was very useful for this project. It helped to create a lightweight, organic form that would have been difficult and time-consuming to manually design. In general, generative design can provide multiple optimized options for a given set-up that balance material use and structural performance. Generative design is especially helpful in the early prototyping stage to explore creative, unconventional solutions before diving into final part design.<br><br>

One limitation that I encountered was constraint sensitivity. Part of the reason why I had so many iterations was because the model would not generate correctly if the preserve and obstacle geometries were not perfect. Any small change would drastically alter the outcome, often ending with material where it shouldn’t be. A second limitation I encountered was manufacturability. In the assistive technology world, most devices are designed for FFM printing as that is most accessible to makers. However, generative design often requires SLS printing due to the complex geometries, meaning that the design would not be able to be used as widespread as Makers Making Change’s current design. The third limitation I encountered was long computation time. Each iteration took around an hour to solve, meaning that generative design would not be feasible if a part needed to be completely designed in a single day.<br><br>

Overall, generative design would be extremely useful in medical and assistive devices field where user-centered designs are of great importance. It would also be useful in aerospace and automotive industries where complex geometries with high strength-to-weight ratios are needed. On the other hand, generative design would likely fall short in high-volume manufacturing or highly regulated industries where organic shapes might be too difficult to produce or certify.
