# :milky_way:Elegoo Mars Printer Guide

## TABLE OF CONTENTS

·  [SAFETY](#point_upSAFETY)

·  [GETTING STARTED](#keyGETTING-STARTED)

·  [OPERATING ENVIRONMENT](#partly_sunnyOPERATING-ENVIRONMENT)

·  [POWERING ON THE PRINTER](#electric_plugPOWERING-ON-THE-PRINTER)

·  [BUILD-PLATE LEVELING](#roller_coasterBUILD-PLATE-AND-LEVELING)

·  [MODEL SETUP & SETTINGS](#microscopeMODEL-SETUP-AND-SETTINGS)

·  [STARTING A PRINT](#rocketPRINTING)

·  [CLEANING THE PRINT](#star2CLEANING)

·  [POST PROCESSING THE PRINT](#hammerPOST-PROCESSING)

·  [FEP MAINTENANCE](#oceanFEP-MAINTENANCE)

·  [PRINTER MAINTENANCE](#nut_and_boltPRINTER-MAINTENANCE)

·  [CONSUMABLE ITEMS](#heavy_check_markCONSUMABLE-ITEMS)

·  [ACKNOWLEDGMENTS](#thumbsupACKNOWLEDGMENTS)



## :question:How does this printer work?

**Your Elegoo is a <u>M</u>asked <u>S</u>tereo<u>L</u>ithography <u>A</u>pparatus resin printer or MSLA for short.** The word stereolithography comes from the Greek word stereo, meaning solid, and (photo)lithography, a form of 'writing' with light. Stereolithography with your 3D printer does precisely that, drawing solids with light one layer at a time. Masked Stereolithography Apparatus(MSLA) utilizes a 405nm wavelength LED array as its light source and an LCD photomask to shape the LED array's light image. The LCD photomask is digitally displayed and composed of square pixels. Then individual pixels are deactivated on the LCD to allow the LED light to pass through to form the resulting layer.

The printing process starts as the build-plate descends into a resin vat, leaving space equal to the layer height between the build platform, or the last completed layer, and the bottom of the vat. The LCD mask then selectively allows UV light to pass through it, shining the light upward through the vat's bottom and curing a layer of resin. 

The cured layer then gets peeled from the bottom of the vat as the build platform moves up, pulling the layer off the FEP(fluorinated ethylene propylene) film. In essence, this is a tug of war between the build-plate surface and the FEP film. The build-plate usually wins this challenge as it remains flat, not allowing any edges to start peeling. The FEP film however is non-stick, highly flexible, and purposely loose. When the cured layer gets pulled upwards by the build-plate, the FEP film curves, letting the cured layer's edges begin to break free as the build-plate rises - breaking the surface suction force and yielding a peel. Once the layer is detached and raised, the fresh resin flows beneath, and the process repeats until the print is complete.

:bulb:To allow the tug of war to work in favor of yielding a successful print, the FEP has to remain non-stick and flexible, the resin has to stay viscous, and the build-plate needs to bond to the resin. Assuming the item to be printed has been orientated and sliced correctly, the easiest way to ensure success is to keep the build-plate and FEP clean, operate the printer at a room temperature of 21'C and above, and have a leveled build-plate. Regarding temperature, always check the resin manufacturer's data as some require it to be a bit higher.



## :point_up:SAFETY

#### Before you start printing, remember safety first and read the owner's manual!

Always handle resins as though they are toxic unless you have specific documentation that states otherwise. Unless otherwise stated, resins are not approved for use with food, drink, or medical application on the human body. Never ingest resin in liquid or solid form. If swallowed, immediately call a poison center or medical professional.

· Ensure you're working in a well-ventilated area. Do not eat, drink, or smoke in the printing work area. Remove jewelry (rings, watches, bracelets) before handling uncured UV curable materials. 

· Always wear proper eye protection and a mask when exposed to any uncured resin, whether during print preparation, printing, or post-processing. Ensure you are wearing chemical-resistant gloves, butyl, nitrile, or neoprene. Avoid using latex gloves.

· Ensure your body is adequately protected by clothing in case of spills and splashes. In case of spillage, if resin makes contact with skin or eyes, wash thoroughly with hand soap and water and seek medical advice - do NOT use solvents to wash - do NOT wash with hot or warm water - this will open your pores and may allow the resin to be pushed further into your skin.

· Tools that may be contaminated with the material should be cleaned before reuse with window cleaner or plenty of denatured or isopropyl alcohol, followed by thorough washing with soap and water.

· Do note that photopolymer resins exothermically react with light, especially UV, and can produce very high heat.



## :partly_sunny:OPERATING ENVIRONMENT 

·  Your printer should be placed in a well-ventilated room, on a level surface, that is away from direct sunlight with an ambient room temperature of at least 21'C / 70'F - 25'C / 77'F being ideal.

·  Always place the printer on a stable surface, where it cannot fall or tip over. Avoid placing the printer over carpeted areas or use a barrier to avoid the possibility of carpet damage.

·  Check the resin manufacturer's datasheet and temperature recommendations as they may have different requirements.

·  Not only does the resin have a stated operational temperature to be maintained, but also the FEP. If the FEP is too cold, it will not have the proper elasticity and increase the object's peel force - increasing the odds of a failed print 'stuck to the bottom.' Operating below the recommended temperature could also make the FEP more prone to damage. To ensure proper FEP elasticity is yielded, operate the equipment in an environment of at least 21C / 70'F.



## :key:GETTING STARTED

·  [PLACE THE PRINTER ON A STABLE, FLAT SURFACE](#partly_sunnyOPERATING-ENVIRONMENT)

·  [APPLY POWER TO THE PRINTER](#electric_plugPOWERING-ON-THE-PRINTER)

·  [LEVEL THE BUILD-PLATE](#roller_coasterBUILD-PLATE-AND-LEVELING)

·  [PREPARE AND PRINT THE TEST FILE](#rocketPRINTING)

·  [CLEAN THE PRINTED TEST FILE](#star2CLEANING)

·  [CURE THE PRINTED TEST FILE](#hammerPOST-PROCESSING)



## :electric_plug:POWERING ON THE PRINTER

·  Place the power cord so you cannot trip over it, step on it, or inadvertently unplug it.

·  Check the power adapter, ensure it's firmly plugged into the wall outlet - you should see a blue LED (on the transformer brick) to indicate that it has mains power.

·  Plug the DC end of the power adapter into the receptacle at the rear of the printer. Check the power switch is in the "ON" position.

·  The front LCD touch panel should greet you with a graphical display.



## :roller_coaster:BUILD-PLATE AND LEVELING 

As touched on in the front matter, the printing process starts with the build-plate descending into the resin vat, leaving space equal to the layer height between the build-plate and the vat's bottom FEP lining. An improperly leveled build-plate will cause this space to be too large or too small, leading to failed print will with harden resin stuck to the vat's bottom. 
Make sure you take the time to level your build-plate correctly. Do not rush this step in your hurry to start printing, take time and get it right. Once your build-plate is leveled correctly and locked down tight, you do not have to relevel it anymore unless you make other adjustments that affect the build-plate. *Do not confuse build-plate leveling with adjusting the four legs of the machine - which is leveling the machine itself.*

**How do I level my build-plate?** 

It is highly recommended that you use the official method, aka paper method, if you're using standard FEP film thickness (100~200um). Watch the Official Elegoo Leveling instructional video [here](https://youtu.be/tiHu3o72NDw), and the reset Z=0 instructional video [here](https://youtu.be/cqRBZUAEWD4).

**:wrench:Preferred Method - Step by step follows:**  
- [ ] If the build-plate is not at least halfway up, raise it by selecting the 'Tool' Button, 'Manual' Button, '10mm' Button, then Up Bottom. Each time you press this, it will raise only 10mm, so you may have to press this multiple times.  
- [ ] Remove the build-plate by turning the top black rotary knob (on the Z-axis) in a counter-clockwise direction, enabling the build-plate to be slid towards you. Do not remove the rotary knob; only rotate it enough to slide the plate off.  
- [ ] Optional but recommended: Test the UV light source by selecting the 'Tool' button, 'Exposure' button, adjust for a few seconds and select the 'Next' button to begin.  You should see a complete rectangular image on the top LCD; the front touchscreen should display the same.  
- [ ] Ensure the build-plate surface is clean and free of any resin or gunk; gently scrape if needed. Clean the build-plate surface with alcohol and lint-free cloth.  
- [ ] Loosen the two bright hex-head bolts on the build-plate head using the large hex wrench - one is on the front, the other on the side. Do not unscrew completely, just enough to allow the build-plate to rotate freely as well as up and down.  
- [ ] Remove the resin vat and place it on its side, in an area where you won't knock it. Check the top LCD free and clean. If dust or residue is present, remove using a clean microfiber cloth - apply alcohol if needed. !Only use microfiber cloth!  
- [ ] Get a standard sheet of printer paper, cut it in half, and place it over the top LCD screen.  
- [ ] Slide the build-plate back onto the printer's Z-axis and tighten the rotary knob.  
- [ ] Home the Z-axis by selecting the 'Tool' button, 'Manual' button, and Home button (looks like an upside-down T).  
- [ ] The build-plate will go down to the paper, slightly rise, and then down again. Check the build-plate's alignment and rotate as needed to ensure it is square with the printer.  
- [ ] While gently pressing down on the build-plate, ensuring it is completely flat and square, tighten the forward-facing hex-head bolt first, followed by the side facing.  
- [ ] Gently try to pull the paper out, not all the way but just only by a few millimeters or so. Try the pull test from the left and then the right edges. If the paper is unable to move, raise the build-plate 0.1mm by first selecting the '0.1mm' button, followed by the Up button - this is not always required, only if you feel the paper will tear when pulling. :warning:If one side was easier to pull the paper than the other, you will have to readjust by loosening the securing screws and go up three steps. If this is a continuing problem, see the notes following the leveling section.:warning: 
- [ ] Select the 'Z=0' button, and select confirm.  
- [ ] After setting Z=0, verify that it is set correctly by starting a dry-run print, leaving the piece of paper on the screen, and checking that the build-plate starts the first layer at the correct Z=0 position have set. !Remember that Z=0 is not the same as Home.  
- [ ] Raise the build-plate by pressing the 10mm button, followed by the up button, at least seven times. Remove the paper.  
- [ ] Grab the resin vat. Check it free and clean - both sides. And again, check the top LCD free and clean. If dust or residue is present, remove using a clean microfiber cloth - apply alcohol if needed. !Only use microfiber cloth!  
- [ ] Gently slide the resin vat into position, taking care to glide it in with a slight upward force against the securing towers and not the LCD screen (the vat film and LCD screen scratch quickly). Ensure the vat is in place before screwing in the two-tower side bolts by feeling a small detent position where it sits securely without wobble. The max resin fill indication should be visible from the front, and the resin pour-out groove should be furthest from you on the left.

**:wrench:Alternate Method 1 / Clean & Empty VAT in place - Step by step follows:**  

- [ ] If the build-plate is not at least halfway up, raise it by selecting the 'Tool' Button, 'Manual' Button, '10mm' Button, then Up Bottom. Each time you press this, it will raise only 10mm, so you may have to press this multiple times.  
- [ ] Remove the build-plate by turning the top black rotary knob (on the Z-axis) in a counter-clockwise direction, enabling the build-plate to be slid towards you. Do not remove the rotary knob; only rotate it enough to slide the plate off.  
- [ ] Ensure the build-plate surface is clean and free of any resin or gunk; gently scrape if needed. Clean the build-plate surface with alcohol and lint-free cloth.  
- [ ] Loosen the two bright hex-head bolts on the build-plate head using the large hex wrench - one is on the front, the other on the side. Do not unscrew completely, just enough to allow the build-plate to rotate freely as well as up and down.  
- [ ] Check the FEP free and clean. If dust or residue is present, remove using a clean microfiber cloth - apply alcohol if needed. !Only use microfiber cloth!  
- [ ] Slide the build-plate back onto the printer's Z-axis and tighten the rotary knob.  
- [ ] Home the Z-axis by selecting the 'Tool' button, 'Manual' button, and Home button (looks like an upside-down T).  
- [ ] The build-plate will go down to the FEP, slightly rise, and then down again. Check the build-plate's alignment and very gently rotate as needed to ensure it is square with the printer.  
- [ ] While gently pressing down on the build-plate, ensuring it is completely flat and square, tighten the forward-facing hex-head bolt first, followed by the side facing.  
- [ ] Select the 'Z=0' button, and select confirm.  

**:wrench:Alternate Method 2 / Resin Filled VAT in place - Step by step follows:**  

- [ ] If the build-plate is not at least halfway up, raise it by selecting the 'Tool' Button, 'Manual' Button, '10mm' Button, then Up Bottom. Each time you press this, it will raise only 10mm, so you may have to press this multiple times.  
- [ ] Remove the build-plate by turning the top black rotary knob (on the Z-axis) in a counter-clockwise direction, enabling the build-plate to be slid towards you. Do not remove the rotary knob; only rotate it enough to slide the plate off.  
- [ ] Ensure the build-plate surface is clean and free of any resin or gunk; gently scrape if needed. Clean the build-plate surface with alcohol and lint-free cloth.  
- [ ] Loosen the two bright hex-head bolts on the build-plate head using the large hex wrench - one is on the front, the other on the side. Do not unscrew completely, just enough to allow the build-plate to rotate freely as well as up and down.  
- [ ] Ensure there are no solidified/hardened pieces of resin present in the VAT. Ensure the FEP surface is smooth by gently raking a soft silicone spatula across all of its surface areas. :warning: If roughness exists, stop the leveling process, filter the VAT's contents back into the resin bottle, clean the VAT, and then restart leveling :warning: Damage to the FEP and LCD screen is possible when debris exists between the FEP and build-plate.   
- [ ] Slide the build-plate back onto the printer's Z-axis and tighten the rotary knob.  
- [ ] Home the Z-axis by selecting the 'Tool' button, 'Manual' button, and Home button (looks like an upside-down T).  
- [ ] The build-plate will go down to the FEP, slightly rise, and then down again. Check the build-plate's alignment and very gently rotate as needed to ensure it is square with the printer.  
- [ ] While gently pressing down on the build-plate, ensuring it is completely flat and square, tighten the forward-facing hex-head bolt first, followed by the side facing.  
- [ ] Select the 'Z=0' button, and select confirm.


**How tight to the paper should I level the build-plate?**

When using the recommended paper method, the paper should be tight enough to pull out with even resistance but not push back in. Remember that the build-plate must grip the paper evenly. 

**Remember** that as you tighten the front and side securing screws, it can move the plate by a tiny fraction - when tightening the bolts, always keep a hand gently pressing the build-plate down and level. When done, if you will find that you cannot pull the paper without tearing, you should raise / backoff the build-plate level by 0.1mm (100um) until the plate is gripping the paper with even resistance and that you can pull but not push it back. This usually requires just one raising of 0.1mm. Lastly, whether you had to raise the plate or not, set Z=0.

**What type of paper should I use to level the build-plate?** 

Just regular photocopy paper, they're generally around 80gsm, but any paper 70 ~ 120gsm (average thickness ranging from 0.05 to 0.10mm) should work too. Just ensure that the paper is clean and not creased or folded. 

**I tried to level the build-plate, but one side is tighter than the other?** 

Using your fingers, push the opposite side of the plate when tightening the set bolts. Alternatively, if you're using the paper method, you can slip another strip of paper to the side, which is too tight, and then tighten the screw. You may need to try this a few times to get the perfect level. 

**I set Z=0, but when I press Home, the position is different?**

**Home is not Z=0!** Home is fixed; it is the hardware Z endstop. Unless you change it physically, it will always be in the same position. Z=0 is the offset distance between Home and your LCD screen; you define during the leveling process when you set Z=0, that's why you have to Home first, then move the platform, then set Z=0. 

When a new Z=0 is specified, pressing Home will NOT move the platform to the position you set; it will be the start position when a print is initiated. You can check it by removing the vat and starting a print.

As said, improper leveling contributes to a lot of frustration, mostly because of its mechanics' poor documentation. In this example, let's say you are leveling the printer, loosened the screws, and press home. You tug on the paper, it feels tight, so you raise by .1mm, then hit 'Z=0' because you raised Z. With this, once you home again, the build-plate will still stop at mechanical zero because of homing stops at the endstop trigger. If you looked at the electrical position of Z, it would read Z:-0.1. Now we know that when we initiate a print, it will home and then go to Z offset (raise .1mm), and then start printing.

Flash forward several prints later, and you level the machine again. You place your piece of paper on the LCD, loosen the screws, and press home. This time you tighten the screws and then remove the paper with no significant tension/friction and think that you don't have to press 'Z=0' because you didn't move Z to take out the paper... WRONG - This is what gives people issues - IF you don't press Z=0, the printer will still have an offset of 0.1mm from the previous leveling, and you may run into problems due to incorrect leveling - because it's 0.1mm off. Remember, homing goes to mechanical zero when the endstop is triggered and doesn't care about the offset!

*Try this for fun: Home and then raise Z by 10mm, press Z=0, and then home again to see where it stops - it will stop when the endstop is triggered, and it will seem as if the Z=0 did nothing. Then, with vat out and no resin, start a print - it will home and then begin to print 10mm above the LCD. So, long story short, when leveling and you're happy with the paper pull test - whether you bumped Z height or not, press 'Z=0'.*

**Do I have to relevel my build-plate after every print?**

No, this should not be required. If you have correctly leveled, securely tightened, and locked down the build-plate tight, it will remain in place and correctly leveled for a very long time. You only need to relevel your build-plate if it has slipped, been knocked, or you made changes that affect the Z=0 position. 

**Should I sand my build-plate?**

Sanding is the last resort you should attempt, and only when you have verified that the build-plate surface is not flat.



## :microscope:MODEL SETUP AND SETTINGS

**How do I use Chitubox slicer?**

CHITUBOX has an excellent article repository [here](https://www.chitubox.com/en/support/indepth/technology), this should be your first stop. In addition, lots of video tutorials exist on YouTube - 3DPrintingPro has an excellent set [here](https://www.youtube.com/watch?v=TTZpvhfaNWY&list=PLC4QzbTxrEF-fA1OC_-zE_4f6n1K-w2SS).

**What settings do I need for the test (rook) file?** 

The test file that came on the included USB stick has been pre-sliced and settings configured for generic resin. Please see the [Printing](#PRINTING) portion of the guide for directions on how to obtain the best results with this file. 

**How should I orientate my part?**

By orientating the part in different directions, there can be a significant difference in the print quality. Sudden changes in the layer's cross-section, small to large or vice versa, will lead to a drastic volumetric change of exposed resin, affecting each layer's shrinkage. In severe instances, this can affect inter-layer adhesion but almost always will result in visible surface lines. CHITBOX has a good article on this topic [here](https://www.chitubox.com/en/article/support/howto/chitubox-free/editing/25). 3DPrintingPro's related video is [here](https://www.youtube.com/watch?v=8xolVj0izVo&t=19s). 

Lastly, vary the placement of your part on the build-plate. If you consistently place your objects in the build-plate's center, your FEP will prematurely wear out in the center yet be absolutely fine in the surrounding, unused, wasted areas.

**What angle should I use to minimize layer lines?**

There isn't one best angle for printing everything. It really depends on your layer height and the type of model you're printing. Don't forget that model orientation also plays a big part in determining the best angles. You could actually be losing details printing at the wrong angle for the layer height. See a detailed explanation [here](https://www.youtube.com/watch?v=Qs2Rb0ExnIM). 

**I bought x resin; what are the best settings for it?** 

Every resin behaves differently; there are no best settings that will work for every resin and every machine. For a quick start, you can refer to the [community resin exposure settings](https://www.elegoo.com/pages/3d-printing-user-suupport). Those settings should enable you to get a print going quickly, but you will need to test and adjust from there to find the best settings applicable for your machine. 

Casting resins can have a difficult time bonding to the build-plate, and subsequently ruining your print. There are multiple ways to increase adhesion during printing. You may apply a thin layer of primer (can be the very resin you are using) on the plate to improve adhesion. Apply to the build-plate and keep under UV light for 10 to 15 minutes. Another way would be to change the profile settings, increase the number of bottom layers, and simultaneously increase the bottom curing time, increasing adhesion. If build-plate bonding persists, you can apply resin on the build-plate surface and leave for 3 mins before printing. Your last resort would be to rough up the build-plate by scrubbing it with a clean 'cooking pan' abrasive pad, using a circular motion, covering the entire plate while it is flat on the working surface. A good video applying primer [here](https://www.youtube.com/watch?v=eDl3vzZy0qQ).

**How do I find the optimal settings for my resin and machine?** 

It's usually best to start with the community resin exposure settings and then dial them in with a few test prints. These test prints will allow you to obtain the optimum settings for your resin, in your environment, matched to your machine. A good instructional video can be found [here](https://www.youtube.com/watch?v=r9GwPEJ8Lq8).

**Resin storage**

Store resins at room temperature in a tightly-closed container away from direct sunlight, preferably in a leak-proof bag. When choosing a storage location, remember that although your room temperature may be adequate, locations at floor level and against exterior walls can expose the resin to varying temperature fluctuations. Inspect the bottles for leakage every couple of weeks, ensure that the caps are on tightly, and give a quick shake to ensure the resin components stay uniformly mixed.

**My resin is expired, can I still use it?** 

Generally, most resin manufacturers advise using the product within one year. These are basically "use by" dates, not expiry per se. In practice, if it was stored at room temperature, in a tightly-closed container, and had no contamination from any cleaning products - It should be acceptable for use. Start by giving the resin a good shake mixing. When pouring it from the bottle to the vat, use a paint filter to catch any particulates that may be present, pay attention to how it flows out of the bottle; it should have a smooth uniform flow as you'd expect with no lumps, chunks, or crystals. Lastly, do a small/quick test print so you can avoid wasting time down the road.

**What do the print settings mean?**

This is assuming you're using the Chitubox slicer that is included on the USB stick. Other slicers may use different terminology, but they're functionally the same. If you're just starting, it's highly recommended you use the Chitubox slicer. It's basic, won't overwhelm you with bells and whistles, and just works. 

**·  Layer Height:** As the name implies, layer height is the exact height of each cured layer. Layer thickness affects not only the speed (printing time) and the quality of each print. The number of layers required to create an object determines the printing speed and the printing time required. The thinner the layer thickness, the longer it takes to make a 3D printed object of a given height. While relatively, with a slimmer layer height, you will increase the quality of the print, leading to a smoother surface and more detail visible in the Z-direction (height) of the model.
Generally, the printers' minimum functional layer height is 25 µm (0.025mm) layer height, and the maximum is 100 µm (0.1mm) layer height. You can adjust this setting based on your printer's actual situation, given the object and resin. If you have no idea how to choose the right one, the tried-and-true technique is to start with a layer height of 50 μm (0.05mm).

**·  Bottom Layer Count:** Simple, this one it's about how many of those super hard base layers to lay down on the base of your print usually this is 5-8 layers.

**·  Exposure Time:** The print quality for each 3D resin is also affected by the light power and the curing or exposure time. Exposure Time is the amount of time that the light source will expose each layer during printing. Different Mars printers have different cure times for various resins, with the mono LCD equipped units requiring about two-thirds less time. 

**·  Bottom Exposure Time:**  Same as *Exposure Time* but only applies to the bottom layers, as set in the *Bottom Layer Count*.

**·  Light-off Delay:** This is the amount of time that the UV light is turned off between the end of one exposure cycle and the beginning of the next. After exposure, the UV light turns off, the build-plate lifts and peels, and then descends; ready for the next cycle and will wait at the bottom (resting at the set layer height over the FEP sheet, at the bottom of your vat) before the UV light comes on again for the next exposure cycle. Longer off-times leave more time for the resin to settle out and form a new layer with fresh resin. This is especially useful for more viscous resins to mitigate issues of poor definition of surfaces facing the build-plate.

**·  Bottom Light-off Delay:** Same as *Light-off Delay* but only applies to the bottom layers, as set in the *Bottom Layer Count*.

**·  Lifting Distance:** This is how far the Z-Axis will pull up upon completion of the exposure cycle.

**·  Bottom Lift Distance:** Same as *Lifting Distance* but only applies to the bottom layers, as set in the *Bottom Layer Count*.

**·  Lifting Speed:** Lift speed refers to the rate at which the build-plate is lifted from the resin vat between layers. When lift speed is too fast, the model and supports can be broken or damaged due to the tug of war between the build-plate and the FEP film. But if reduced too much, the printing time will be unnecessarily increased. When modifying this setting, you should take both print quality and print time into account. 

**·  Bottom Lift Speed:** Same as *Lifting Speed* but only applies to the bottom layers, as set in the *Bottom Layer Count*.

**·  Retract Speed:** This is how quick the Z-axis will plunge back into the vat, after it has completed it's lift cycle. This setting applies to both normal and bottom settings.

**·  Anti-aliasing:** Aliasing is the staircase effect that occurs when diagonal or curved lines or borders are drawn on raster displays consisting of square or rectangular pixels. Anti-aliasing is to smooth object edges by reducing the number of lines and vertical artifacts you see on your 3D printed model.
CHITUBOX provides an anti-aliasing function with a 2/4/8 level. After special algorithm processing, it makes the model more smooth and effectively reduces edge aliasing.

**·  Transition Layer Count:** This is the number of layers where the bottom and normal exposure times will gradually decrease rather than an abrupt drop, aiding the adhesion between them.   At present, this is only available for the ELEGOO SATURN, and the transition type is linear only.

**What is cupping / suction warping, and how do I combat it? Should I add a vent hole?**

Vent holes are often improperly called "drain" holes; they are not for draining resin. Imagine a glass full of water upside down in a bucket of water. When you pull the glass up out of the bucket, it stays full until the lip of the glass breaks the surface of the water in the bucket. 

In the vat, the lowest point of the print, the new layer does not generally rise above the vat's liquid resin level. Therefore, the liquid resin inside the "bowl" or "cup" cannot evacuate unless you add a vent hole. This is a significant cause of failures. You have to reduce the work that the stepper motor has to do to lift the platform.

Initially, in the printer's vat, the inside volume of resin will be pulled up. Eventually, depending on the volume of the inside space and the volume of resin in the vat, the new layer will rise above the fluid level because the surface of the fluid will be moving down at ever-increasing rates with each layer. That is, the level of the fluid inside the space and in the vat are actually moving in opposite directions. When that happens, all of the fluid inside will be released, but now you have a trapped volume of air, so you will alternate between struggling with lifting up and struggling with pushing down. 

Without vent holes, it's a recipe for bad prints. The result is that you can get multiple failures at various heights, depending on where these extremes occur. 

**How do I hollow my model?**

It depends on the software. Two popular free programs that make it easy to hollow your models are Chitubox and Meshmixer. Look [here.](https://www.youtube.com/watch?v=wAW-rqrr8nc)

**Can I just use auto supports for all my models?** 

Not the best idea. For simple models, auto supports should generally work, but as with anything automatic, it will never be perfect. For a start, you can use auto supports and supplement with manual supports on parts that the software missed. But it will be best to [learn to place your supports manually](https://www.youtube.com/channel/UCbv2mDrRqXovPdahRyoCFhA/search?query=supports) and precisely; you will find that you will need less supports and produce better prints in the long run. 



## :rocket:PRINTING

:exclamation:*Ensure you are operating your printer with an ambient room temperature of at least 21'C / 70'F, 25'C / 77'F being ideal. This is critical for success as it greatly affects the resin and FEP film properties.*

**My first print, do I have to print the rook?** 

:wrench:It is recommended that you print it, but before you print the rook file from the USB stick, there are some steps you need to take to ensure success.

- [ ] Check your resin's bottom & normal exposure times, for your printer model, [here](https://docs.google.com/spreadsheets/d/1pXFnb8nZNR-jC5h0_t28NJ3jpmWeOPu6bmYNY05lysU/edit#gid=0).
- [ ] Plug the USB stick in your computer and open the __Rook.ctb file in Chitubox slicer, you should just have to double-click on the file to open it. 
- [ ] Once it opens the file, you will see two columns of numerical data in the lower portion of the screen. Check that 'Exposure Time(s):' and 'Bottom Exposure Time(s):' match the numbers corresponding to your printer/resin in the excel spreadsheet above. 
- [ ] If the numbers in Chitubox differ from the spreadsheet, double-click the number to change and type the value obtained from the spreadsheet.
- [ ] Click the 'Save' button and call the file '__My-Rook.ctb'. Safely eject the USB stick from your computer.
- [ ] Inspect the build-plate surface and ensure it is free of any debris. Give it a good wipe down with IPA and a lint-free cloth. Ensure the build-plate a firmly secured by snugging the black rotary knob.
- [ ] Inspect the FEP film on the bottom of the resin vat. Make sure it is clean and clear, free of any holes, deep dents, and deep scratches. Ensure the resin vat is secured by snugging the two vat screws.
- [ ] Identify the max file line in the resin vat. Pour your prepared resin into the vat, filling it halfway - to a level between the FEP film and the max fill line. If any air bubbles exist, wait a few minutes for them to dissipate.
- [ ] Plug the USB stick in to your printer, select the '__My-Rook.ctb', and commence the print.

A successful test print with a known-good model will confirm that your printer works as it should and that you have precisely leveled your build-plate and your FEP tension is correct. It is also inevitable that sooner or later, a print will fail. A failed print will often leave small, partially cured resin pieces floating in the vat or hard cured resin stuck to the FEP. For subsequent prints to have the highest success rate, the resin vat must be cleaned and cleared of debris.  Although it is not required, it is good practice to inspect and clean the vat after every print.

**I'm about to start a print, but the touchscreen shows a filename highlighted in red?** 

That's normal; it's showing the last file you selected or printed. 

**How long do I have to shake the resin up or heat it?**

·  It is always best to read the resin's manufacturer's datasheet/instructions since every resin is particular and requires different mixing and operating temperature.

·  In most cases, resins don't like to be used below 21'C/70'F.

·  A non-pigmented resin getting a good shake for 30 seconds is enough, while a heavy pigmented one for a minute or two. If the resin is thicker due to low temp, add some extra time to that.

**How much resin should I pour into the vat?** 

To start, fill the VAT about halfway between the FEP surface and max fill line. Do not exceed the max fill line; if there is too much resin, it will rise from displacement and cause a spill. Once you pour resin into the VAT, let it sit for a few minutes to allow any air bubbles to escape before printing. 

**Can I add resin halfway through a print?**

·  Yes, no problem. You do not have to pause the print; just slowly and gently pour the resin into the vat. Make sure to not bump or touch the build-plate while pouring. Be mindful of displacement when adding resin. 

·  Make sure to mix the fresh resin well before adding. Try to ensure the resin temperature is the same.

**Can I pause halfway through a print?** 

Yes, you can pause at any time during your print. Resume as quickly as you can to ensure that your print will continue safely. However, it is generally not recommended as it will most likely leave a line at the layer where you paused. If you time your pause after a peel move, the chances of resuming without a line is better. 

**My print turned out OK but there resin 'skin' on the FEP?**

This is typical resin over-exposing during the printing process. Double-check your machine/resin exposure settings. It is very common to mistake resin exposure settings for the Mars vice Mars 2; this could differ from 10 seconds to 3 seconds.

**My print is stuck to the FEP! How should I remove it?**

· Unscrew the resin vat retaining screws and remove the vat.

· Empty the resin vat. The vat has one corner recessed to aid in pouring. Use the recessed corner in combination with a funnel and screen to pour the resin into the bottle. 

· Wipe the remaining resin into the funnel with a soft silicone squeegee and then with a soft paper cloth. The layer of hardened/stuck resin should now be discernible. 

· While the vat is in a normal upright position, grasp it with both hands, with fingers on the bottom side of the FEP and palms against the sides of it. Use your fingertips (not your fingernails) to detach the solidified resin from the FEP by gently applying pressing up. Start from the edges and use a circular motion to separate it evenly. You may be able to hear the layer detaching.

· You should now be able to remove the large pieces by using the plastic scraper to very gently slide across the FEP with the blade at a low shallow angle. 

· Once removed, proceed with normal after print cleanup, but pay particular attention to the FEP. Inspect the surface for any scratches, dents, or holes. If the FEP is damaged, replace it immediately.

**My prints are not dimensionally accurate!?!?**

First, ensure that your exposure settings are optimal for the resin used. Underexposure causes thinner parts, while overexposure will swell. Many of the basic resins swell when printed. There could also be slight shrinkage. It all depends on your settings and the brand of resin and formulations that manufacturers use. It usually isn't noticeable on organic prints. 

**How can I make them true to scale?**

Here is a process to determine a correction factor to use in your slicer.

- [ ] Log room temp.
- [ ] Do resin calibration prints, get it nailed. Write the temp and exposure seconds on the bottle.
- [ ] Make a cube or download one if lazy. 20mm cubes are typical, but the correction factor will be more accurate when you make it larger. If you typically print a standard sized object in the X & Y planes, then use a block outline of the shape you will print as the resin shrinkage may not be a true linear correction.
- [ ] Slice the .stl file as usual, at 100% scale.
- [ ] Print, wash and cure the object.
- [ ] Calculate the scaling factor:  
  Use the following formulas to determine the required scaling factor:  
  X Scaling Factor = (XCAD - XPART)/ XCAD * 100% (answer will be as a percentage)  
  EXAMPLE:  
  X measurement of CAD model = 20mm  
  X measurement of printed part = 18.5mm  
  X Scaling Factor = (20.0 – 18.5)/20.0 *100 = 7.5%  
  Slicer X scaling factor should be 100% + 7.5% = 107.5%      
- [ ] Go into your slicer, change X & Y scaling to the calculated correction factor and then slice the .stl file.
- [ ] Print, wash and cure the object.
- [ ] Measure the corrected print. If an error still exists, go back to the 'Calculate the scaling factor' step, but you will then subtract or add to the previously obtained scaling factor and then repeat the verification process.
- [ ] The last step, write the correction factor on the bottle.  


**Lines or Layer Shifting on the printed model?**

See Elegoo's support guide [here](https://www.elegoo.com/blogs/3d-printer-user-guide/lines-or-layer-shifting-on-the-printed-model).

**Holes in the 3D printed model?**

See Elegoo's support guide [here](https://www.elegoo.com/blogs/3d-printer-user-guide/holes-in-the-3d-printed-model).

**I hear a rumbling / loud humming noise once I start a print?** 

If you're having issues with the build-plate homing fine but then trying to bury itself into the LCD and making a rumbling/loud humming noise once a print is initiated - relevel the build-plate and ensure you use Z=0.

**I hear a strange faint knock or a suction/sticking sound every time the plate lifts. Is this normal?** 

It's completely normal. It's a good sign that your print is sticking to the build-plate and that the layers are releasing from the FEP film. It will be more audible during the first few bottom layers of the print, don't worry if you can't hear it later on as it depends on the layer section being printed. 

**How do I know that my print is sticking to the build-plate?** 

·  One easy way to tell is by listening for the sound that's made as the layer peels off the FEP. You can hear it clearly, especially for the first few bottom layers. Don't worry if you can't hear it anymore later; it varies depending on the layer's size being printed. 

·  You can also use the pause to check on your print, but note that you may get a line at the layer where you paused. 

**My prints just won't stick?** 

This is almost always a build-plate leveling issue. Make sure your leveling is 100% correct before attempting these other solutions. 

·  Clean the build-plate carefully with IPA or other solvents. Dry before use. 

·  Shake your resin in the bottle well before using it. Resin already in the vat may have settled and need to be stirred. 

·  Preheat or warm the resin, you can use a hairdryer or heating pad on most bottles to gently heat the resin to 20~30°C. 

·  Preheat the build-plate, same as the resin. 

·  The build-plate may have shifted. Try and level it again; make sure to tighten well. 

·  There may be cured resin in your vat, in which case you should drain and clean. 

·  Did you remember to set, or reset, Z=0?

·  The FEP film may be too tight or too loose. 

·  You may be using resin formulated for SLA laser or DLP printers. Check the resin manufacturer's recommendations. 

·  Are you using a specialty monomer-free resin such as Blue cast? You may need a primer coat. Check the resin manufacturer's recommendations. 

·  If all else fails, check your plate level once again and use Z=0! 

**The bottom layers stick, but my prints didn't form/fell off at the supports?**

See Elegoo's support guide [here](https://www.elegoo.com/blogs/3d-printer-user-guide/model-sticking-to-the-fep-rather-than-sticking-to-the-build-platform) and [here](https://www.elegoo.com/blogs/3d-printer-user-guide/print-falls-from-the-support-or-part-of-the-print-is-missing).

If your prints have good bottom adhesion but fail at the supports, this is generally due to your normal layers' incorrect exposure settings. As a first step, try increasing exposure. 

·  Try increasing normal exposures by a second or two. 

·  You may need to increase support tip size and depth in your slicer settings. 

·  A mix of medium and heavy supports will help and/or increase support density. 

·  It can also be due to the orientation of your model. Try to angle your model and minimize large surface sections. 

·  Is your model a large solid? Hollowing the model is recommended. 

**The top of my prints are sharp and detailed, but the bottoms seem soft and less defined?** 

During the printing process, resin components form covalent bonds, but layer to layer, the part remains in a semi-reacted or semi-cured state. While in this semi-reacted state, the resin retains polymerizable groups that can still form bonds across layers. Polymerization only stops when the resin is fully cured via post-processing in a UV station or sunlight. 

Simply put, during printing, the layers of the model facing the FEP film are always sharply defined as the layer is exposed perfectly against it. Whereas the layers facing the build-plate, previously exposed, still receive UV light from diffusion/diffraction/scattering from the current exposed layer and thus will still cure slightly. This is akin to overexposure and thus details will be lost. Coupled with this, some resin always remains around the bottom parts (facing the build-plate) and will also bond and cure to the details. 

This is a limitation of the technology but can be largely mitigated and overcome by the following:

·  Ensure that exposure settings are optimal for your resin. Overexposure will magnify this issue. 

·  Ensure that the model is well orientated and angled to minimize resin pooling and that important details are presented facing the FEP film. 

·  Allow enough clearance for the supports so that resin does not get trapped between the bottom of the print and the build-plate.

·  Set longer UV off-times so that more viscous resins can drain during lift. It will also help to heat the resin during colder temperatures. 



## :star2:CLEANING

**How do I clean my prints?** 

The recommended method is the two tub system. Fill both containers with 91% Isopropyl Alcohol (IPA) or other solvents such as 95% Ethanol. Although not necessary, heating the first tub to around 45°C helps dissolve the resin faster. 

Drop the print into the first tub and swirl for several seconds. Use a soft brush on hard to reach parts, crevices, etc. Then dunk the part in the second tub of solvent and rinse clean. Do not leave your prints soaking too long in the tubs - only enough time to remove the excess resin. 

Lastly, remove the part and dry thoroughly before UV curing; pat-drying with a lint-free cloth followed by blow-drying with compressed air or a hairdryer works well. Whichever way you choose - ensure the part is dried thoroughly before UV curing; failure to do so can result in loss of definition, white powdery remains on the part, and flaking/scaling on surfaces. 

**What solvents should I use to clean my prints?** 

Resin manufacturers universally recommend 91% Isopropyl Alcohol (IPA) or 95% Ethanol. Other solvents may be used but generally not recommended. Do not pay for overpriced cleaning solutions marketed for 3D resin printers. When in doubt, check the resin manufacturer's datasheet/recommendations. 

**How long do I clean my parts in solvents?** 

For as little time as possible to get your prints cleaned of uncured resin. Do not leave your prints to soak. Some manufacturers advise no longer than 30 seconds. Usually no more than 3 minutes. When in doubt, check the resin manufacturer's datasheet/recommendations. 

**How do I clean the LCD?**

Use a microfiber cloth and a small spray of IPA to remove any dust and stains. If there is dried resin on the glass, you can carefully scrape it off with a razor. Finally, buff the glass with a microfiber cloth.

**The FEP tore, and there's cured resin on the LCD. How do I clean that?** 

Damp a piece of a microfiber cloth with IPA, then lay it on the cured resin. Wait a few minutes, then with a fingernail, gently try to prise the layer of cured resin off the LCD glass. If you can't easily prise it off, use a razor or glass scraper, but be careful with that. Be prepared to purchase a replacement LCD.

**How do I clean the FEP Film?**

Once you have drained the vat of resin, spray down with IPA and gently wipe it off with a microfiber cloth. Spray again and use the microfiber cloth to soak off the remaining residue from the FEP. You may need to repeat this several times. Finally, buff the FEP with the microfiber cloth. Be careful of dried resin on the cloth that could scratch or puncture the FEP. 

**What else can I use to clean my prints and tools from uncured resin?**

·  Manufacturers universally advise using a solvent like 91% IPA (Isopropyl Alcohol) or 95% Ethanol. Proprietary cleaning solutions or other solvents may also be used, such as Mineral spirits (aka White spirits, Turpentine), etc. 

·  If you have bought a water-washable resin, you can simply use water and some mild soap. 

·  A small brush helps get into and clean the fine grooves or details in your prints.

·  Alcohol and other flammable solvents should not be used directly with ultrasonic cleaners because of the fire hazard.

**How long can I keep the resin in the vat?**

It depends on environmental factors and type/brand of resin. Typically if the resin is kept out of light and spared any moisture/dirt, it may sit in the vat for a few weeks. Clear resins tend to sit better; opaque resins will need more stirring before use to mix the pigments back. When in doubt, check the resin manufacturer's datasheet/recommendations. 

·  Check for loose cured resin or stuck resin; you will need to clean that out. 

·  Cover the vat. You can cut a piece of cardboard that fits over the vat or print one out on an FDM printer.

·  Before printing, carefully stir the resin for 1 - 2 minutes with a soft silicone spatula, be careful not to scratch the FEP screen.

·  Do not leave the build-plate hanging with uncured resin. Take it out and clean with IPA - leave it out until you are ready to print. This will lessen the weight on the single lead screw prevent deformation and potential Z wobble. 

**Can I put excess resin that didn't get used during a print back into the original bottle?**

Yes, but always strain out any debris using a filter! The resin vat has one corner recessed to aid in pouring. Use the recessed corner in combination with a funnel (screen placed inside the funnel) to pour the resin back into the bottle. Inspect the FEP's surface for any scratches, dents, or holes. If the FEP is damaged, replace it immediately.

**Water washable resin, how to dispose of the dirty water after washing the print? Wash it down the drain?** 

**Do not pour it down the drain!** Water washable resin works because it uses water-soluble monomers. Water isn't an acrylate. Water can not cure. When you dilute resin into anything that's not capable of curing, it won't be inert again. 
The only proper way to dispose of the wash is to reduce the solution by evaporation, and then collect and UV cure the resin residuals and dispose of them properly. 



## :hammer:POST PROCESSING

**My print stuck so well to the build-plate that I can't remove it?** 

When prints adhere so well that removal is difficult, use the provided sharpened steel scraper to fracture the model off the plate. Place the build-plate/print on your working surface, in a position where the model is facing left and adjustable head facing right or vice-versa. While using a very low, near-parallel to the build-plate angle, position the steel scraper on the edge where the model and build-plate interface and then give a quick, gentle downwards knock to the handle. Running hot water over the print/build-plate for several seconds may provide additional assistance.

**When should I remove supports?** 

It is generally best to first clean the entire print before removing any supports - this will reduce your and the work area's resin exposure. Following the cleaning process, remove the supports before UV curing as they are softer, and in many cases, you can easily pull or rub them off. In some cases, you may want to remove them after curing, especially when working with thin and delicate parts that may warp during the curing process if not supported.

**What is post-curing?**

Post-curing enables your printed parts to reach the highest possible strength and become more stable. Many post-curing methods exist using light and heat, from curing only with natural sunlight, using salon type UV fingernail curing stations, to DIY UV curing stations. Heat accelerates the process and enables even more complete bond formation, resulting in increased material properties impossible to achieve with light alone. For small prints, a low-cost UV nail salon might be an effective post-curing tool. But to maximize mechanical properties, consider purchasing an enclosure around a powerful 405 nm light.

**How long should I cure my print?**

The proper light, heat, and time will optimize your prints' mechanical properties. Post-cure time depends on your equipment, resin choice, and part geometry. An ideal post-cure setting achieves the properties you need in the shortest amount of time. For standard resins, this amount may be as short as 10 minutes, going up 30 minutes. Where strength, rigidity, and temperature resistance are needed, engineering grade resins improve with post-cure up to 60 minutes. Always check the resin manufacturer's datasheet/recommendations as each different brand and kind of resin will differ. 

**What will happen with over-curing?**

The material will degrade due to UV irradiation. With extreme UV exposure levels, the part will degrade and cause brittleness. Placing a part outside is generally not nearly enough to cause any notable amount of degradation. But curing a part overnight in a high-intensity UV chamber might be enough to damage the material. This is not unique to resin and would occur in most organic materials.

**Will curing prints underwater speed up the curing time?**

Yes. Underwater heat dissipation and UV diffuse scattering effect will be better. The water does absorb UV light, but the absorption is not significant at the wavelengths used to cure UV resin. So you don't have to add much exposure time if you cure your parts in a shallow tank of water. There are really no "cons" to curing in a water bath, other than getting your parts wet and require drying.

**Is post-curing with sunlight useful?** 

If you don't have a UV chamber, you can submerge the print in a clear container filled with water, as said above. Then place the container under direct sunlight. Of course, the exposure time will be much longer than under a direct UV lamp. If the print still feels uncured or sticky, leave the print and the container in the sun for some more time.

**How durable are the prints? Will they break if I drop them?** 

It depends on the resin used. Unlike PLA or ABS, regular hobby-grade resin prints are quite brittle and can easily break when dropped. There are specially formulated resins for prototyping or even functional usage, which have different properties such as flexibility, hardness, and UV resistance. 

**Why do I get white chalky residue on my prints after curing?** 

The white residue appears if there's moisture, water, or uncured resin on your prints when UV cured. Always clean your prints well and make sure they are completely dry before the UV curing. 



## :ocean:FEP MAINTENANCE

When you receive your new printer, it will come with an aluminum or plastic vat frame with FEP film already installed. Check that the film is tight by lightly tapping with your finger. If it is tensioned correctly, it should sound just like a snare drum. 

Sometimes the screws may seem loose, but they may be tensioned correctly from the factory. Do not merely tighten the screws, as you may over tension the FEP. 

**How tight exactly should the FEP be tensioned?** 

If it sounds like a snare drum when you lightly tap with a finger, it should be good enough. But since hearing is subjective, to be precise, you should use an audio analyzer to check; factory tensioned FEP film is around 350Hz, but anything between 250Hz to 375Hz is fine. [This](https://youtu.be/Yr_wtZqBfbQ) video shows how to tune/tension your FEP.

**Why do I have to go through all this trouble to get the correct FEP tension?** 

When your print peels from the FEP film, there are a lot of suction forces involved. Unlike more expensive machines, it does not have a tilt peel mechanism; therefore, it relies on the FEP film's flexibility to provide a clean and successful peel. 

*If the film is too tightly tensioned, your prints won't peel off properly and may stick to the build-plate, too loosely tensioned, and it'll have layer lines or other unwanted artifacts.*

A correctly tensioned FEP at a normal room temperature will give the best print results and avoid print failures or delamination problems. 

**Should I coat my FEP film?**

Not needed in most cases, FEP (fluorinated ethylene propylene, invented by DuPont, sold under the brand name Teflon FEP) is already one of the most slippery materials known to science. With that being said, many users report increased success rates with different coatings but caution must be taken as applications and compounds vary from case to case.

**Why is my FEP film so cloudy or hazy?** 

When new, the film is clear. But it is easily scratched by handling or cleaning. Use a soft tissue to soak resin when cleaning up the vat, do not aggressively wipe the film as even tissue will scratch it. These micro scratches cause the film to go cloudy. Buffing the film with a microfiber cloth will restore some clarity. The film must be kept clear to ensure sharp and detailed prints. 

**When should I replace my FEP film?** 

If you take care of it, it will not need to be replaced for months. You should only need to replace the FEP film when it becomes scratched up or cloudy. If it is not correctly maintained, your print quality will deteriorate. Replace it immediately if it is punctured or torn. If you notice cured resin on your LCD glass, it means the film may have a micro tear.

**How do I replace the FEP film?** 

Watch the video by Elegoo detailed step by step [here](https://youtu.be/tsokPTRLXss). It is important to note one significant neglect in that video: there is no mention of tightness! Watch the below video for that. It is also much easier to trim the excess FEP before placing the retaining assembly into the VAT frame. 
FEP replacement video using Gatorade bottle cap [here](https://youtu.be/Yr_wtZqBfbQ). 

**How do I test if my FEP film has protective plastic on it?** 

It's difficult to see if there's a protective plastic film on your FEP. An easy way to test is by dripping a few drops of resin on your FEP film, then hold the film vertically. If the resin slides downward easily without sticking and leaves the FEP clear, it's good. If the resin sticks where you dripped it and moves slowly or smears, you have protective plastic that needs to be removed. 

**Why do I need to use a bottle cap or foam when replacing the FEP film?** 

The bottle cap, or foam, will allow some slack to the film so that when you tighten the frame down, you will get approximate tension. If you don't do that, you may over tension the film and it may tear. If it didn't tear, later on you'll be wondering why all your prints fail. 



## :nut_and_bolt:PRINTER MAINTENANCE

**What maintenance do I need to do to keep my printer running well?** 

·  Keep your printer clean! Keep everything clean by wiping down with a microfiber cloth slightly dampened with IPA. Wipe resin drops and spills off immediately with IPA and tissue.

·  Keep your vat and FEP clean. Empty the resin vat after each print failure. The vat has one corner recessed to aid in pouring. Use the recessed corner in combination with a funnel and screen to pour the resin into the bottle. Inspect the FEP's surface for any scratches, dents, or holes. If the FEP is damaged, replace it immediately.

·  Keep the LCD screen clean. Use a microfiber cloth dampened with IPA or LCD cleaning spray to clean to surface. Do not use paper towels; otherwise, you may scratch the LCD surface. 

·  Dust off and keep the printer's cover clean. Clean the lid with IPA, but do not use ethanol or acetone. 

·  Clean and Grease Z-Screw. Depending on usage frequency, every two months or earlier, clean and replace the grease on the lead screw. If it squeaks, do this immediately. 

Peter Grande has a good video on general maintenance; you can find it [here](https://youtu.be/2178v1iMSqo). 

**What grease should I use for the lead screw (Z rod)?**

Use a PTFE based such as Super Lube or white lithium viscous grease. It should be a thick, creamy, toothpaste consistency type. You can use a generic machine grease, cosmoline, gel grease, gear grease, or similar but make sure the lubricant is not thin and runny, and Do NOT use WD-40!
Watch the Official Elegoo instructional video [here](https://youtu.be/OWXlZSi15cE).

**How do I replace the grease on the lead screw?** 

Wipe all the old dirty grey grease off with a cloth rag or kitchen towels. Then really get it clean by wiping again with solvent and use a toothbrush to get between the threads. IPA works great. Make sure solvent doesn't drip down into the stepper motor beneath. When it's clean and dry, re-grease with good quality grease, apply by dabbing onto the entire length of the screw, then switch on the printer and run the slide block up and down. 

**How do I replace the LCD screen?**

Watch the Official Elegoo instructional video [here](https://youtu.be/JYxKFs2lY8w).

**How do I replace the Z limit switch?**

Watch the Official Elegoo instructional video [here](https://www.youtube.com/watch?v=tBmwPHZfxI8).

**How do I replace the front touch screen?**

Watch the Official Elegoo instructional video [here](https://youtu.be/45wycTFA9E0).

**Where can I buy replacement parts?**

From Elegoo's website [here](https://www.elegoo.com/collections/parts-accessories), or Chitu Systems [here](https://chitusystems.com/).

**Where can I find firmware updates, original manual, original USB drive files, and resin settings?**

From Elegoo's website [here](https://www.elegoo.com/pages/3d-printing-user-suupport).



## :heavy_check_mark:CONSUMABLE ITEMS

There are many consumables available for resin printing, and this is just a brief list to give you some ideas. In addition to this consumables list, you will need resin. There are several kinds of resins; standard, high-definition, flexible, castable, high-temperature, and more. Each resin presents its unique strengths and weaknesses, but the standard type is usually best to start while getting comfortable with the resin printing process. With that, when selecting a resin, make sure that it is compatible with your machine - which is an MSLA LED/LCD unit with a 405nm light source. Please pay attention to the resin manufacturer's recommended operating temperature to ensure that it will be usable in your environment.   

**Tier 1 - Critical Items. These are the typical use items that you should have on hand.**  
*Metal Scraper  
*Plastic Scraper  
Plastic Razor Blades  
Nitrile Gloves  
Safety Glasses  
Mask / Respirator   
Paint Filters  
Small Funnel for Paint Filters  
Small Soft Silicone Squeegee  
Paper Towels  
Microfiber Cloth Pack  
Isopropyl Alcohol  
Small Paint Brush (or toothbrush)  
Windex Foaming Spray  

**Tier 2 - Recommended Items. Items that you will eventually need or will make the machine's operation safer & more manageable.**  
Replacement FEP Film  
Craft Apron  
Quality USB Stick  
Silicone or Boot Mud Mat  
or Cafe Serving Tray  
Super Lube PTFE Grease  
Exacto Knives  
Pickles Bucket w/ Basket  

**Tier 3 - Helpful Items. These are items that you don't need per se, but they will be helpful.**  
Clean & Wash Station  
or Ultrasonic Cleaner  
Replacement LCD Screen  
Printer Enclosure  
Small/Micro file set  
UV Flashlight  
Hex Driver Set  
^Resin VAT Cover  
^Top Cover Handle  
^Dual Angled Drip Attachment  

*Included with the printer.  
^Can be printed or purchased.  



## :thumbsup:ACKNOWLEDGMENTS

**Where did all this information come from?** 

Information was gathered from the [Photonsters](http://photonsters.org), [Elegoo product site](https://www.elegoo.com/), [Chitubox](https://www.chitubox.com/en/support/indepth/technology), [ElegooMars Reddit Sub](https://www.reddit.com/r/ElegooMars/), and various others.  
Photonsters.org is a wealth of information, always worth is visit, even if you don't have a Photon... 