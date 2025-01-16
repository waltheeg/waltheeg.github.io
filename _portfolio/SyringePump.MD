---
title: "Syringe Pump"
excerpt: "This 3D printed, motorized syringe pump is programmed to accurately deliver liquid from 5mL - 20mL syringes."
header:
  image: /assets/img/Syringe Pump Feature.png
  teaser: /assets/img/Syringe Pump Feature.png
gallery:
  - image_path: assets/img/Syringe Pump Rendering 1.png
  - image_path: assets/img/Syringe Pump Rendering 2.png
  - image_path: assets/img/Syringe Pump Wiring.png
   
---

Syringe pumps are commonly used in laboratories (for microfluidic devices) and medical institutions (for administering medicine and vital nutrients). It is imperative that a syringe pump be calibrated correctly to prevent any mistakes, especially ones that can cost a life. However, commercial programmable syringe pumps are extremely expensive, even for the most basic models. As a result, DIY syringe pumps can be a cost-effective, yet functionally acceptable, alternative.

# Features

* **Linear Actuator -** The syringe pump converts the rotary motion of the stepper motor to linear movement of a syringe's plunger by using a coupler and a lead screw.
* **Suitable for Various Syringes -** Syringes of multiple diameters can be easily installed onto the syringe pump by aligning the plunger flange and barrel flange to the corresponding slits on the carriage and modified end support.
* **External Electrical Components -** There are four external electrical components attached to the enclosure shell: the LED, the ON/OFF button, the potentiometer, and the LCD screen. The ON/OFF button starts the motor. The LED shows the working condition of the syringe pump (green when the pump is running, yellow when the pump is paused, and red when all liquid is dispensed). The potentiometer has a turning knob that controls the flow rate of the pump. The LCD screen displays the flow rate of the pump and the time remaining until all liquid is dispensed.

# How to Operate

1) Fill the syringe with liquid and insert into the holders.

2) Make sure the ON/OFF button next to the LED light is pressed in, indicating an OFF stage. Plug in the power cord. The LED should turn yellow. 

3) If a preset flow rate is desired, adjust the potentiometer such that it outputs “Flow Rate: 0” (completely turned to the left) or “Flow Rate: 100” (completely turned to the right). The desired flow rate can be set in the Arduino code, which will calculate the necessary steps per second to output through the motor. Then, press the ON/OFF button to start the device at a consistent preset speed. 

4) Alternatively, if the potentiometer is required for operation, start with the knob turned completely to the left or the right (0 or 100 Flow Rate), press the ON/OFF button to start the device, and then adjust the knob to the desired flow rate. 

5) The LCD displays the flow rate and the time countdown. 

6) The LED turns green when the device is running,  yellow when the flow rate is 0 and there’s liquid remaining in the syringe, and red when the device reaches the end of its stroke.


# Bill of Materials 

## Off-the-Shelf Parts

| Part # | Part Name | # Required |
|:---------:|:----------:|:-------------:|
| 1 | V Slot | 1 |
| 2 | NEMA 17 motor | 1 |
| 3 | M3 x 10 mm bolt | 4 |
| 4 | Flexible coupler | 1 |
| 5 | M5 x 8 mm bolt | 8 |
| 6 | M5 tee nut | 8 |
| 7 | 8 x 8 x 250 mm lead screw | 1 |
| 8 | Lead screw lock collar | 2 |
| 9 | 8 mm x 200 mm linear rod | 1 |
| 10 | Linear rod lock collar | 2 |
| 11 | Flanged ball bearing | 2 |
| 12 | Through nut 8x8-4 | 1 |
| 13 | M3 x 8 mm thread forming screw | 4 |
| 14 | LM8UU linear bearing | 1 |
| 15 | 9.5 mm push button | 1 |
| 16 | 5 mm LED | 1 |
| 17 | Potentiometer | 1 |
| 18 | LCD Screen | 1 |
| 19 | 20 mL syringe | 1 |

## 3D Printed Parts

| Part # | Part Name | # Required |
|:---------:|:----------:|:-------------:|
| 20 | Motor Mounting Plate | 1 |
| 21 | Carriage | 1 |
| 22 | Syringe Support | 1 |
| 23 | Plunger Support | 1 |
| 24 | End Support | 1 |
| 25 | Enclosure Shell | 1 |
| 26 | Enclosure Drawer | 1 |
| 27 | Cord Hole Filler | 1 |
| 28 | Button Gap Filler | 1 |


# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e1faab3ee761fd268?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

{% include gallery caption="Syringe Pump Gallery" %}

# Arduino Code

[Click Here!](/assets/Code_for_Motor.ino)
