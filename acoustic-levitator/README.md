![319523205-5173c0f6-0d28-48f7-96ac-889d97e8fc29](https://github.com/user-attachments/assets/32b98478-8b15-47ca-858e-df0c27436936)# Acoustic Levitator

**Defying Gravity with Sound Waves!**

Imagine witnessing particles suspended in mid-air, as if held by invisible hands. This isn't science fiction—it's acoustic levitation in action.

![DSC02902 Kopie](https://github.com/user-attachments/assets/a9439547-914a-4b54-94ef-6a50aa655dcd)


Acoustic levitation uses ultrasonic waves to lift objects without physical contact, where materials float freely, defying gravity. The device achieves this through carefully aligned loudspeakers emitting ultrasonic waves, forming standing waves that manipulate air pressure and create zones where objects can be levitated and manipulated with sound.


## Schematics

Our guide is structured as follows to help you build your own acoustic levitator:

**The Electronics:** Detailed parts list, tools needed, electronics setup, and step-by-step construction.
**The Wood Case:** Instructions to build a supporting structure.

### The Electronics

#### 1. Parts List 

This low-cost levitator design is based by Asier Marzo's work [1]. Materials can be sourced from various suppliers or bought as a kit (https://de.aliexpress.com/item/1005001908749344.html). Here's what you'll need:

* **1x 3D-printed TinyLev** - STL files available in the **'Instructables.zip'**.
* **1x Arduino Nano with mini USB cable** - Generates the necessary square wave signals.
* **72x Air-borne ultrasound transducers (10mm 40kHz)** - Key elements for creating the levitating sound field. 
* **1x L298N Dual H-Bridge motor driver** - Amplifies the signal from the Arduino Nano, crucial for the device's efficiency and also manages the phase and frequency precisely.
* **Essentials:** 1x DC Barrel, 1x power switch, 1x DC jack, 3x buttons, jumper wires, wires of various gauges, some exposed wires, and a base sheet for the driver board.

_The **code for the Arduino Nano** is available in the **'Instructables.zip'**_.

#### 2. Needed Tools

Prepare the following tools for assembly:
* 3D printer, soldering iron, hot-glue gun, multimeter, cable peeler, screwdriver, pliers, drill, and optionally, an oscilloscope.
    
#### 3. Electronics' Setup

Here is the electronic schematics: 

![319501143-5bd645b4-7fe7-4155-9720-b677664a749d](https://github.com/user-attachments/assets/8950b872-4c36-4c1d-82bb-9b5f6d7d0a0f)

**Attention:**
* The setup came with an **unsuitable power supply** - it is important that it is **not higher than 10V, otherwise it will be overheated!** To overcome this problem, I built in **a decoy module instead of the DC Barrel**, where you can choose the voltage that goes into the electronics. To use this module you need a power supply with a range from 5V to 20V. I chose this one with 45W, but there are many that work. **I set it to 9V!**. Here are the elements use:

     * Decoy module: https://www.amazon.de/dp/B0CH37FZ9N?psc=1&ref=ppx_yo2ov_dt_b_product_details
     * Power supply: https://www.conrad.de/de/p/ansmann-home-charger-247pd-usb-ladegeraet-45-w-steckdose-ausgangsstrom-max-3-a-anzahl-ausgaenge-2-x-usb-usb-c-buchse-2227125.html?refresh=true
     * 1 long USBc cable


<p align="center">
<img src="https://github.com/user-attachments/assets/3aec0493-4902-4630-b2b2-4b9c82bcfe09" alt="Alt text" style="width:70%; height:auto; ">
</p>

 * When gluing the transducers to the 3D-printed support structure, make sure you don't use too much glue so that the shape is maintained and no transducer strays too far from the shape the support structure provides.

 * I replaced the cooling element with a larger one to make sure the levitator doesn't overheat.

<p align="center">
<img src="https://github.com/user-attachments/assets/04df3814-f20c-406e-8cb0-9183ab03bf3c" alt="Alt text" style="width:20%; height:auto;">
</p>

* I also added a small red laser in the hole in the middle of the 3D printed part, where I removed the lens so the light is not bundled. The laser has to be soldered to 5V and ground. **Be careful when soldering, the laser is temperature sensitive!**

**For electronics, here is a paper summary[1]:**
The design features a single-axis, non-resonant acoustic levitator. It's built around a series of compact ultrasonic transducers, which act as the system's emitters. This setup is engineered to control two channels, capable of generating signals up to 70 Vpp (peak-to-peak voltage), with the precision of phase adjustments down to π/12. We keep one channel at a steady phase while we can adjust the other to move levitated objects up or down with precision.

This levitator is user-friendly and designed for longevity, requiring lower operating voltages than what you'd typically see in laboratory settings. Traditional lab setups often depend on high-voltage Langevin horns to generate significant sound pressure from a single source. These horns are sensitive to temperature, difficult to tune to a specific frequency and potentially dangerous because of the high voltage. The idea of using an array of transducers is analogous to moving from a single powerful lamp to an array of light-emitting diodes (LEDs).  

![315937722-284263c8-ca0f-47e7-8845-c67f31021234](https://github.com/user-attachments/assets/087c06f7-81dc-4387-9bf1-bbdcffdc2b90)

Unlike _resonant_ configurations that use one emitter facing a reflector, our _non-resonant_ setup employs two opposing emitters. While resonant setups might be more efficient, they're also more prone to issues with temperature changes and require precise alignment. The system stands out for its versatility and stability, capable of working flawlessly within a wide temperature range (-40°C to +40°C) without the need for recalibration. This makes it a better option for diverse applications.

#### 4. Step-to-Step Construction

For assembly guidance, refer to these instructional videos:

* https://youtu.be/yVDWrWpaBho?si=ZAmCy2piCWks4kC8
* https://youtu.be/ABjRnSYw-4k?si=KRd1o-waau9IIHIh


### The Wood Case

Construct a durable case to house the electronics and ensure the levitator's stability. We used furnished panels or screen-printed panels, birch film-coated on both sides BFU 100. You can buy the wood e.g. here in https://holz-krüger.de/.  

<p align="center">
  <img  src="https://github.com/user-attachments/assets/8bbea707-89eb-40df-bcf1-d6b35b0cc2ec" alt="standing">
</p>

First, we construct the box without the support for the levitator. Then we construct the ear-shaped support, and finally we assemble it.  

**The box: the walls.**

1. Cut 4 equal pieces with the measurements H 110 mm, L 350 mm, T 12mm and a bevel cut (45°) on both edges like in the following sketch (view from the side):

<p align="center">
<img width="288" alt="Bildschirmfoto 2024-04-04 um 11 37 13" src="https://github.com/xstageproject/experiments/assets/78161180/62a93e29-fa45-40d5-9468-e49bf2a7e9cf">
</p>


2. Cut/mill on the inner side of each of the pieces a slit (with a depth of 10 mm) - or milling a groove in wood, deutsch: eine Nut fräsen - that is as thick as the wood, like this: 
<p align="center">
<img width="288" src="https://github.com/user-attachments/assets/ac33e4ef-9365-4c1e-a5e5-11d113167fc1">
</p>

The idea is that the floor panel will be glued into the slit of each side. 

3. Make a chamfer in the wood (deutsch: eine Kanten-Fase mit der Tischfräse machen), so it looks more beautiful but also that nobody cuts him/herself with the wood edges. They can be really . 

**The box: the floor panel.**
   
1. Cut a square of 360x360 mm. The bottom appears to be longer than the walls, but it is not. The measurements are chosen this way because the length of the walls (350 mm) plus the depth of the material (12 mm) gives a total length of the box of 362 mm. By having a floor panel that is 360 mm long, we can insert it into the 10 mm slit of the wall panels, giving us a visible floor of 350 mm. 
 
<p align="center">
  <img width="486" src="https://github.com/xstageproject/experiments/assets/78161180/5173c0f6-0d28-48f7-96ac-889d97e8fc29" alt="standing" style="width:40%; height:auto;">
</p>


**The ear-shaped support**

**Step-by-Step Guide to Constructing the Wood Module**

* Materials and Tools Needed:
* Stencil (ear-shaped), 4 wood pieces, Sandpaper, Drill, Bandsaw, Bench milling machine, Hand milling machine, Wood glue, Clamps, Pressure application tools, Safety gear (gloves, goggles)

Instructions:
**1. Stencil Design and Preparation:**
* Design and laser cut a stencil in the shape of the ear-shaped support.
<p align="center">
<img src="https://github.com/user-attachments/assets/1699c86b-7e36-4d87-8bf7-a6c1783e3d7b" alt="Alt text" style="width:33%; height:auto;">
</p>

**2. Cutting and Sanding:**
* Using the stencil, cut out 4 pieces of wood that match the stencil’s shape.
* Sand one side of each piece to ensure that later the inner surfaces will glue to each other.

**3. Stencil Attachment:**
* Align the stencil with the wood pieces and drill holes to secure it in place, preventing any movement.

**4. Rough Cutting with Bandsaw:**
* Use the bandsaw to perform a rough cut along the outer edges of the stencil. Focus on giving the wood pieces the initial shape of the stencil.
* Important: For 2 out of the 4 pieces, cut out the inner circle as well.

**5. Detailed Milling with Bench Milling Machine:**
* Secure the stencil to the wood pieces again.
* Use the bench milling machine to precisely cut the detailed shape, including the inner circle for 2 of the pieces.

**6. Cable Duct Cutting with Hand Milling Machine:**
* For the 2 pieces without the inner circle cutout, use the hand milling machine to create a space for fitting the levitator.
* Additionally, cut out a cable duct to accommodate any necessary wiring.

**7. Gluing and Clamping:**
* Arrange the sanded parts together as required.
* Apply wood glue to the surfaces that will be joined.
* Clamp the pieces together and apply pressure for several hours to ensure a strong bond.

**8. Finishing:**
* Once the glue is fully dried, sand the borders of the assembled module to make sure all edges are even and smooth.

**Visual Reference:**
<p align="center">
<img src="https://github.com/user-attachments/assets/69298355-9baf-4aea-903d-6badad0bc199" alt="Alt text" style="width:33%; height:auto; display:inline-block; margin-right: 10px;">
 <img src="https://github.com/user-attachments/assets/cc461930-4dad-4e5d-9387-710ae3fb3ae5" alt="Alt text" style="width:33%; height:auto; display:inline-block;">   
 <img src="https://github.com/user-attachments/assets/48186855-68b6-4b20-8b47-78c79db2ce99" alt="Alt text" style="width:33%; height:auto; display:inline-block;">   
</p>




**Assemblying the two parts**

To install the ear-shaped module to the box, follow these steps:

**1. Create a Stencil:** Design and laser cut a stencil that provides the correct distance between the two ear-shaped modules (based on the distance set by the 3D printed part) and indicates the position of the two buttons
<p align="center">
    <img src="https://github.com/user-attachments/assets/bda9e354-75a8-4030-95dc-c9b2bb311247" alt="Alt text" style="width:40%; height:auto;">  
</p>


**2. Drill Holes in Modules:** In the bottom part of each ear-shaped module, drill two centered holes.

**3. Transfer Hole Positions to Box:** Insert suitable marking tips into the drilled holes and use them to transfer the hole positions to the box. Use the stencil to ensure correct positioning. Here's a video explanation of the process: https://youtu.be/j3SrxKgMRGg

**4. Drill Holes in Box:** Drill the holes in the box at the marked positions. Also, drill holes for the buttons.

**5. Insert Threaded Sockets:** Install threaded sockets (Gewinde-Muffen) into the holes so that the parts can be re-installed as needed.

<p align="center">
   <img src="https://github.com/user-attachments/assets/c09a41f7-ef8a-4f2a-909a-1d4b18edae5d" style="width:40%; height:auto;"> 
</p>

**6. Install Levitator:** Insert the levitator into the ear-shaped module and thread the cables through the cable duct. Screw the ear-shaped module to the box and glue the electronics to the box.

<p align="center">
     <img src="https://github.com/xstageproject/experiments/assets/78161180/1322a548-34f8-4d66-82ca-1f7ba93571db" alt="Alt text" style="width:40%; height:auto; display:inline-block; margin-right: 10px;"> 
     <img src="https://github.com/xstageproject/experiments/assets/78161180/a0051c8e-602d-4b1b-9d20-bd1245c23256" alt="Alt text" style="width:40%; height:auto; display:inline-block;">  
</p>

**7. Install Buttons:** Install the buttons and solder them to the Arduino.

**8. Install the Cover:** Laser cut (Abdeckung_Levitator.dfx) and install the cover (in the bottom part of the box) to protect the cables from being ripped out during transportation. 

**9. Test:** Test that everything is working correctly. If necessary, solder any connections that need adjustment.

## Troubleshooting

## Scientific Background

### Acoustic Levitation

Acoustic levitation is a phenomenon that harnesses the power of sound waves to lift and manipulate objects in mid-air. This technique relies on the principles of acoustics, particularly the concept of standing waves and acoustic radiation pressure. In general, sound is a vibration that propagates as an acoustic wave through a transmission medium such as a gas, liquid or solid. Here is a schematic visualization of such propagation:

<p align="center">
  <img src="https://github.com/xstageproject/experiments/assets/78161180/6f1c18f8-af3b-4a0c-b435-64a09a29564e" alt="KXWd">
</p>

**Standing Waves and Nodes:**
When ultrasonic waves, emitted from transducers, intersect, they can form standing waves. A standing wave is a pattern of vibration that simulates a wave standing still. These waves are characterized by nodes (points of minimum displacement) and antinodes (points of maximum displacement). In the context of acoustic levitation, objects are trapped at the nodes, where the acoustic pressure is highest, effectively counteracting gravity.

**Acoustic Radiation Pressure:**
The core principle behind acoustic levitation is the acoustic radiation pressure exerted by the sound waves on the object. This pressure results from the momentum transfer when the sound wave interacts with an object, creating a force that can lift and suspend the object. The magnitude of this force depends on several factors, including the sound wave's amplitude, frequency, and the object's size and material.

<p align="center">
  <img width="486" src="https://github.com/xstageproject/experiments/assets/78161180/cd7b509c-d237-4d4b-b822-0b60b3653de4" alt="standing">
</p>


The arrangement of the transducers is crucial for achieving stable levitation. They are oriented and spaced to create a geometric focus, which enhances trapping forces. By modifying the excitation signal of the transducers, it is possible to control the horizontal movement of the trapped particles.

<p align="center">
<img width="286" alt="_Simulated acoustic field; each circle represents a 10 mm diameter transducer and the colour represents the emitting phase of the transducers (two driving signals are required to produce vertical movement of the traps). Image from [1]._ " src="https://github.com/xstageproject/experiments/assets/78161180/9d036c3f-8ef1-400f-abbb-ba9f02132843">
<figcaption>Simulated acoustic field; each circle represents a 10 mm diameter transducer and the colour represents the emitting phase of the transducers (two driving signals are required to produce vertical movement of the traps). Image from [1].</figcaption></p>

**Acoustic waves can trap particles of different materials and a wide range of sizes of millimetre dimensions**. 
This is a significant difference with respect to optical trapping in which the particle size range is 0.01-10 μm and the materials need to be dielectric or optically transparent. Acoustic trapping has a ratio of trapping force to input energy orders higher than optical manipulation.  Magnetic levitation can strongly hold samples in the mid-air but only supports ferromagnetic materials. Other forms of levitation such as aerodynamic levitation agitate and alter the samples in the process, and in electrostatic levitation, the required control systems are complex and the sample materials are limited.


### Ultrasound Technology
Ultrasound refers to sound waves with frequencies above the upper audible limit of human hearing, which is about 20 kHz. Children can hear some high-pitched sounds that older adults cannot hear, because in humans the upper limit pitch of hearing tends to decrease with age. In acoustic levitation, ultrasonic frequencies are typically used because they can create smaller nodes in the standing wave pattern, allowing for the manipulation of small objects with greater precision.

![850px-Ultrasound_range_diagram svg](https://github.com/xstageproject/experiments/assets/78161180/9c8a5859-201f-44a7-bc6c-05d2426bc03b)

The Acoustic Levitator's transducers are operating in the ultrasonic range, which in this case is at 40kHz.

**Perception in animals**

* Bats use a variety of ultrasonic ranging (echolocation) techniques to detect their prey. They can detect frequencies beyond 100 kHz, possibly up to 200 kHz.
  
* Dogs and cats' hearing range extends into the ultrasound; the top end of a dog's hearing range is about 45 kHz, while a cat's is 64 kHz.
  
* Many insects have good ultrasonic hearing, and most of these are nocturnal insects listening for echolocating bats. These include many groups of moths, beetles, praying mantises and lacewings. 


### Applications Beyond Levitation

While acoustic levitation is a compelling demonstration of ultrasound's capabilities, the technology has widespread applications across many fields:

**Medical Imaging:** Ultrasound is perhaps best known for its use in medical sonography, providing real-time images of the interior of the body without ionizing radiation.
**Non-Destructive Testing:** In industry, ultrasound is used to detect flaws in materials, assess thickness, and perform other inspections without damaging the object.
**Cleaning:** High-frequency ultrasonic cleaners can remove dirt and contaminants from surfaces at a microscopic level, widely used in healthcare, manufacturing, and jewelry cleaning.
**Chemistry and Pharmaceuticals:** Ultrasound can accelerate chemical reactions and is used in the production of pharmaceuticals, in a process known as sonochemistry.

Acoustic levitation itself has applications in containerless processing, materials science, and pharmacology, allowing for the study of substances without container-related contamination and the manipulation of small particles or droplets in a controlled manner.

[1] _Asier Marzo, Adrian Barnes, Bruce W. Drinkwater; TinyLev: A multi-emitter single-axis acoustic levitator. Rev. Sci. Instrum. 1 August 2017; 88 (8): 085105. https://doi.org/10.1063/1.4989995_

_Acoustic Wave Gif:_ 
https://images.app.goo.gl/GzPLr7egBPVpys7r9 
https://www.acs.psu.edu/drussell/demos/standingwaves/standingwaves.html 

_Ultrasound picture:_ https://upload.wikimedia.org/wikipedia/commons/7/74/Ultrasound_range_diagram.svg  

## Change Log / Variants


