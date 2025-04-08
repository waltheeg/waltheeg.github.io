---
title: "Bike Phone Holder"
excerpt: "This 3D-printed bike mount securely holds a phone and allows it to rotate as desired."

header:
  image: assets/img/Bike Full Render.png
  teaser: assets/img/Bike Full Render.png
gallery1:
  - image_path: assets/img/Bike Detent Section.png
gallery2:
  - image_path: assets/img/Bike Clamp Part.png
  - image_path: assets/img/Bike Detent Part.png
  - image_path: assets/img/Bike TPU Part.png
gallery3: 
  - image_path: assets/img/Bike Full Render.png
gallery4: 
  - image_path: assets/img/Bike Real 1.jpg
  - image_path: assets/img/Bike Real 2.jpg
gallery5: 
 - image_path: assets/img/Bike GIF.gif

   
---
<br>
## Introduction

The goal of this project was to design and 3D print a phone holder for a bike. A phone needed to attach quickly to the holder without the use of tools, and the holder needed to allow the phone to rotate between portrait and landscape orientations. Furthermore, the holder needed to lock at the desired positions so that device could resist road vibrations. <br><br>

This project was designed through top-down modeling. Top-down modeling is a process by which individual components are constructed within an assembly. This is in contrast to bottom-up modeling, where parts are designed separately and later assembled. <br><br> 

Top-down modeling was leveraged too allow better component alignment. Since every component is created in the context of existing components (and more specifically, using projected geometry), it is much easier to ensure parts fit perfectly. Additionally, with joints added between the components, the desired motion of the design can be visualized on Fusion 360.


## Design

### Clamp Part

The clamp mechanism on the component is modeled after the clamp mechanism on many traditional bike bells, using just one bolt to tighten the device to the handlebars. To accommodate the potential for part growth, the clearance hole diameter on the clamp was increased to allow an M5 bolt to slide through with ease. <br><br>

The main body of this component includes a chamfered cut-out for a heat set insert to easily attach the detent gear. It also includes a spring box, giving supportive sidings to hold the spring and ball bearing in place. The edges of the main body were smoothed in case the user were to inadvertently hit the device while riding the bike. <br><br>


This entire part was SLS printed out of nylon powder to eliminate the concern of the part breaking along the layer lines in a traditional FFF PLA print when the clamp is tightened. 


### Rotational Mechanism

To rotate the phone, a simple detent mechanism was used. This mechanism uses a small spring-loaded ball bearing that engages with notches in a gear to hold a phone at specified angles. The detent mechanism provides tactile feedback when the phone locks in place while also allowing for easy rotation when enough force is applied. <br><br>

The detent mechanism created for this project works very well, especially when harnessing the added weight from a phone. However, one limitation is that it required the phone to be pushed in the direction of the spring before rotating. This could have been solved with a lighter spring or two symmetrical springs. <br><br>

The detent gear was SLS printed from nylon powder for ultimate durability. The only modification that was made to the part due to the potential of part growth with SLS printing was increasing the diameter of the hole to allow the M5 bolt to rotate with ease. <br><br>


{% include gallery id="gallery1" %}

### Phone Holder

The goal with the phone holder was to secure a phone at its corners such that the securement mechanism wouldn’t interfere with what is being displayed on the phone. To accomplish this, existing Amazon products were researched, and one [promising design]( Amazon.com: BONE Bike Tie Connect Kit 2, Bike Cell Phone Mount for Stem, Detachable & 360° Rotatable Silicone Holder with Shock-Absorbing Design, Cycling Phone Holder for Most Smartphones (Stem - Connection Kit) : Automotive) was selected and traced in Fusion 360. Once extruded, the component was scaled to fit an iPhone 16 Pro.<br><br>

When printing this component, an FFF printer was used. 90 TPU was selected as the filament rather than 95 TPU as it allows for increased flexibility, allowing the phone to be gripped more securely. 


### CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a499a8c2dbb0b748e5?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


## Assembly Instructions

1.	Embed a heat set insert into the center (chamfered) hole of the Clamp Part.
2.	Place a 15 mm long, 5 mm diameter compression spring into the spring box in the Clamp Part. Balance a 7 mm ball bearing on top of this spring.
3.	Place the Detent Gear in the Clamp Part, slightly compressing the spring to allow the holes to align. Secure with a 12 mm M5 bolt, leaving some space for the Detent Gear to rotate freely.
4.	Stretch the center of the TPU part over the lip of the Detent Gear.
5.	Use a 16 mm M5 bolt and M5 nut to secure the clamp to the handlebars. 
6.	Stretch the corners of the TPU Part around a phone to secure it in the clamp.<br>
To rotate the phone, simply push down into the spring and spin the phone to the desired orientation.


{% include gallery id="gallery2" caption="1) Clamp Part; 2) Detent Gear; 3) TPU Part" %}

## Final Model

xx
{% include gallery id="gallery3" %}

{% include gallery id="gallery4" %}

{% include gallery id="gallery5" %}
