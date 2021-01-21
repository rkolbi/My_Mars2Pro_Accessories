# Elegoo Mars Printer Guide

## TABLE OF CONTENTS

·  [SAFETY](#SAFETY)

·  [OPERATING ENVIRONMENT](#OPERATING-ENVIRONMENT)

·  [POWERING ON THE PRINTER](#POWERING-ON-THE-PRINTER)

·  [BUILD PLATE LEVELING](#BUILD-PLATE-LEVELING)

·  [RESIN VAT & FEP SETUP](#VAT-AND-FEP-SETUP)

·  [MODEL SETUP & SETTINGS](#MODEL-SETUP-AND-SETTINGS)

·  [STARTING A PRINT](#PRINTING)

·  [CLEANING THE PRINT](#CLEANING)

·  [POST PROCESSING THE PRINT](#POST-PROCESSING)

·  [PRINTER MAINTENANCE & TROUBLESHOOTING](#MAINTENANCE-AND-TROUBLESHOOTING)

·  [ACKNOWLEDGMENTS](#ACKNOWLEDGMENTS)


## >SAFETY

#### Before you start printing, remember safety first and read the owners manual!

·  If you have lost or misplaced the manual, you can find it [here](https://www.elegoo.com/pages/3d-printing-user-suupport). 

·  Always handle resins as though they are toxic unless you have specific documentation that states otherwise. Do note that photopolymer resins exothermically react with light, especially UV, and can produce very high heat. 

·  Ensure you're working in a well-ventilated area. Always wear proper eye protection and a mask when exposed to any uncured resin, whether during print preparation, printing, or post-processing. Ensure you are wearing chemical-resistant gloves, butyl, nitrile, or neoprene. Avoid using latex gloves. 

·  Ensure your body is adequately protected by clothing in case of spills and splashes. In case of spillage, if resin makes contact with skin or eyes, wash thoroughly with soap and water and seek medical advice - do NOT wash with hot or warm water - this will open your pores and may allow the resin to be pushed further into your skin.



## >OPERATING ENVIRONMENT 

·  Your printer should be placed on a level surface, away from direct sunlight, and somewhat dust-free.

·  An ambient room temperature of at least 21'C / 70'F is recommended - 25'C / 77'F being ideal.

·  Check the resin manufacturer's datasheet/temperature recommendations.

·  Not only does the resin have a stated operational temperature to be maintained, but also the FEP. If the FEP is too cold, it will not have the proper elasticity and increase the object's peel force - increasing the odds of a failed print 'stuck to the bottom.' Operating below the recommended temperature could also make the FEP more prone to damage. To ensure proper FEP elasticity is yielded, operate the equipment in an environment of at least 21C / 70'F.



## >POWERING ON THE PRINTER

·  Check the power adapter, ensure it's firmly plugged into the wall outlet - you should see a blue LED (on the transformer brick) to indicate that it has mains power.

·  Plug the DC end of the power adapter into the receptacle at the rear of the printer. Check the power switch is in the "ON" position.

·  The front LCD touch panel should greet you with a graphical display.



## >BUILD PLATE LEVELING 

Incorrect build plate leveling is the number one reason for print failures. It is a statistical fact, most of the issues posted invariably trace back to imperfect build plate leveling as the root cause. 

**Make sure you take the time to level your build plate correctly.** Do not rush this step in your hurry to start printing.

·  Once your build plate is leveled correctly and locked down tight, you do not have to relevel it anymore unless you make other adjustments that affect the build plate. 

·  Ensure that you lock down the build plate after leveling. 

·  Do not confuse build plate leveling with adjusting the four legs of the machine.

**How do I level my build plate?** 

It is highly recommended that you use the official method, aka paper method, if you're using standard FEP film thickness (100~200um). Watch the Official Elegoo Leveling instructional video [here](https://youtu.be/tiHu3o72NDw). Watch the Official Elegoo reset Z=0 instructional video [here](https://youtu.be/cqRBZUAEWD4).

**Detailed Step by step follows:**

- [ ] If the build plate is not at least halfway up, raise it by selecting the 'Tool' Button, 'Manual' Button, '10mm' Button, then Up Bottom. Each time you press this, it will raise only 10mm, so you may have to press this multiple times.


- [ ] Remove the build plate by turning the top black rotary knob (on the Z-axis) in a counter-clockwise direction, enabling the build plate to be slid towards you. Do not remove the rotary knob; only rotate it enough to slide the plate off.


- [ ] Ensure the build plate surface is clean and free of any resin or gunk; gently scrape if needed. Clean the build plate surface with alcohol and lint-free cloth.


- [ ] Loosen the two bright hex-head bolts on the build plate head using the large hex wrench - one is on the front, the other on the side. Do not unscrew completely, just enough to allow the build plate to rotate freely as well as up and down.


- [ ] Remove the resin vat and place it on its side, in an area where you won't knock it. Check the top LCD free and clean. If dust or residue is present, remove using a clean microfiber cloth - apply alcohol if needed. !Only use microfiber cloth!


- [ ] Get a standard sheet of printer paper, cut it in half, and place it over the top LCD screen.


- [ ] Slide the build plate back onto the printer's Z-axis and tighten the rotary knob.


- [ ] Home the Z-axis by selecting the 'Tool' button, 'Manual' button, and Home button (looks like an upside-down T).


- [ ] The build plate will go down to the paper, slightly rise, and then down again. Check the build plate's alignment and rotate as needed to ensure it is square with the printer.


- [ ] While gently pressing down on the build plate, ensuring it is completely flat and square, tighten the forward-facing hex-head bolt first, followed by the side facing.


- [ ] Gently try to pull the paper out, not all the way but just only by a few millimeters or so. If the paper is unable to move, raise the build plate 0.1mm by first selecting the '0.1mm' button, followed by the Up button - this is not always required, only if you feel the paper will tear when pulling.


- [ ] Select the 'Z=0' button, and select confirm.


- [ ] After setting Z=0, verify that it is set correctly by starting a dry-run print, leaving the piece of paper on the screen, and checking that the build plate starts the first layer at the correct Z=0 position have set. !Remember that Z=0 is not the same as Home.


- [ ] Raise the build plate by pressing the 10mm button, followed by the up button, at least seven times. Remove the paper.


- [ ] Grab the resin vat. Check it free and clean - both sides. And again, check the top LCD free and clean. If dust or residue is present, remove using a clean microfiber cloth - apply alcohol if needed. !Only use microfiber cloth!


- [ ] Gently slide the resin vat into position, taking care to glide it in with a slight upward force against the securing towers and not the LCD screen (the vat film and LCD screen scratch quickly). Ensure the vat is in place before screwing in the two-tower side bolts by feeling a small detent position where it sits securely without wobble. The max resin fill indication should be visible from the front, and the resin pour-out groove should be furthest from you on the tank's right.



**How tight to the paper should I level the build plate?**

If you are using the recommended paper method, the paper should be tight enough to pull out with even resistance but not push back in. Remember that the build plate must grip the paper evenly. 

**Remember** that as you tighten the front and side securing screws, it can move the plate by a tiny fraction - when tightening the bolts, always keep a hand gently pressing the build plate down and level. When done, if you will find that you cannot pull the paper without tearing, you should raise / backoff the build plate level by 0.1mm (100um) until the plate is gripping the paper with even resistance and that you can pull but not push it back. This usually requires just one raising of 0.1mm. Lastly, whether you had to raise the plate or not, set Z=0.

**What type of paper should I use to level the build plate?** 

Just regular photocopy paper, they're generally around 80gsm, but any paper 70 ~ 120gsm (average thickness ranging from 0.05 to 0.10mm) should work too. Just ensure that the paper is clean and not creased or folded. 

**I tried to level the build plate, but one side is tighter than the other?** 

Using your fingers, push the opposite side of the plate when tightening the set bolts. Alternatively, if you're using the paper method, you can slip another strip of paper to the side, which is too tight, and then tighten the screw. You may need to try this a few times to get the perfect level. 

**I set Z=0, but when I press Home, the position is different?**

**Home is not Z=0!** Home is fixed; it is the hardware Z endstop. Unless you change it physically, it will always be in the same position. Z=0 is the offset distance between Home and your LCD screen; you define during the leveling process when you set Z=0, that's why you have to Home first, then move the platform, then set Z=0. 

When a new Z=0 is specified, pressing Home will NOT move the platform to the position you set; it will be the start position when a print is initiated. You can check it by removing the vat and starting a print.

As said, improper leveling attributes to a lot of frustration, mostly because the manufacture of these printers poorly document the mechanics of it. In another example, let's say you are leveling the printer, loosened the screws, and press home. You tug on the paper, it feels tight, so you raise by .1mm, then hit 'Z=0' because you raised Z. With this, once you home again, the build plate will still stop at mechanical zero because of homing stops at the endstop trigger. If you looked at the electrical position of Z, it would read Z:-0.1. Now we know that when we initiate a print, it will home and then go to Z offset (raise .1mm), and then start printing.

Flash forward several prints later, and you level the machine. You place your piece of paper on the LCD, loosen the screws, and press home. This time you tighten the screws and then remove the paper with no significant tension/friction and think that you don't have to press 'Z=0' because you didn't move Z to take out the paper... WRONG - This is what gives people issues - IF you don't press Z=0, the printer will still have an offset of 0.1mm from the previous leveling, and you may run into problems due to incorrect leveling - because it's 0.1mm off. Remember, homing goes to mechanical zero when the endstop is triggered and doesn't care about the offset!

Try this for fun: Home and then raise Z by 10mm, press Z=0, and then home again to see where it stops - it will stop when the endstop is triggered, and it will seem as if the Z=0 did nothing. Then, with vat out and no resin, start a print for - it will home and then begin to print 10mm above the LCD. So, long story short, when leveling and you're happy with the paper pull test - whether you bumped Z height or not, press 'Z=0'.

**Do I have to relevel my build plate after every print?**

No, it is absolutely not necessary. If you have correctly leveled, securely tightened, and locked down the build plate tight, it will remain in place and correctly leveled for a very long time. You only need to relevel your build plate if it has slipped, been knocked, or you made changes that affect the Z=0 position. 

**Should I sand my build plate?**

Sanding is the very last resort that you should attempt, and only when you have verified that the build plate surface is not flat.

**I'm sure my build plate is level, but I still can't get a print!** 

Did you just switch resins? Did you use an unsuitable resin formulated for SLA Laser or DLP printers? Are you using specialty castable resins? Did you mix the resin properly before use? Is the resin expired? Is it too cold? Many factors may affect print adhesion. Keep testing to find the root causes for your plate adhesion issues. 

For the vast majority of standard modeling resins, ensuring a leveled build plate and increasing bottom exposures should enable plate adhesion.

Some resins such as Anycubic Maroon or Monocure Rapid are known to be notoriously tricky to obtain adhesion. This is due to their formulation. Try other resins, or increase bottom exposures by 10-second increments and keep testing. 

Castable and other specialty resins such as Blue cast (monomer-free) generally need longer bottom exposures and the help of a primer coat. Primers are just UV glue and can be found online cheaply. You can also try LOCA (Liquid Optically Clear Adhesive), 



## >VAT AND FEP SETUP

When you receive your new printer, it will come with an aluminum or plastic vat frame with FEP film already installed. Check that the film is tight by lightly tapping with your finger. If it is tensioned correctly, it should sound just like a snare drum. 

Sometimes the screws may seem loose, but it may be tensioned correctly from the factory. Do not simply tighten the screws, or you may then over tension the FEP. 

**How tight exactly should the FEP be tensioned?** 

If it sounds like a snare drum when you lightly tap with a finger, it should be good enough. But since hearing is subjective, to be precise, you should use an audio analyzer to check; factory tensioned FEP film is around 350Hz, but anything between 250Hz to 375Hz is fine. [This](https://youtu.be/Yr_wtZqBfbQ) video shows how to tune/tension your FEP.

**Why do I have to go through all this trouble to get the correct FEP tension?** 

When your print peels from the FEP film, there are a lot of suction forces involved. Unlike more expensive machines, it does not have a tilt peel mechanism; therefore, it relies on the FEP film's flexibility to provide a clean and successful peel. 

*If the film is too tightly tensioned, your prints won't peel off properly and may stick to the build plate, too loosely tensioned and it'll have layer lines or other unwanted artifacts.*

A correctly tensioned FEP at a normal room temperature will give the best print results and avoid print failures or delamination problems. 

**Should I coat my FEP film?**

Not needed in most cases, FEP (fluorinated ethylene propylene, invented by DuPont, sold under the brand name Teflon FEP) is already one of the most slippery materials known to science. Coating your FEP film with a hydrophobic substance like Rain-X may cause lousy quality prints.

**Why is my FEP film so cloudy or hazy?** 

When new, the film is clear. But it is easily scratched by handling or cleaning. Use a soft tissue to soak resin when cleaning up the vat, do not aggressively wipe the film as even tissue will scratch it. These micro scratches cause the film to go cloudy. Buffing the film with a microfibre cloth will restore some clarity. The film must be kept clear to ensure sharp and detailed prints. 

**When should I replace my FEP film?** 

If you take care of it, it will not need to be replaced for months. FEP film needs to be replaced only when it becomes too scratched up or cloudy from use. If it is not replaced, your print quality will deteriorate. Replace it immediately if it is punctured or torn. If you notice cured resin on your LCD glass, it means the film may have a micro tear.

**How do I replace the FEP film?** 

Watch the video by Elegoo detailed step by step [here](https://youtu.be/tsokPTRLXss). It is important to note one very important omission in that video: there is no mention of tightness! Watch the below video for that. Also, it is much easier to trim the excess FEP before placing the retaining assembly into the VAT frame. 
FEP replacement video using Gatorade bottle cap [here](https://youtu.be/Yr_wtZqBfbQ). 

**How do I test if my FEP film has protective plastic on it?** 

It's difficult to see if there's a protective plastic film on your FEP. An easy way to test is by dripping a few drops of resin on your FEP film, then hold the film vertically. If the resin slides downward easily without sticking and leaves the FEP clear, it's good. If the resin sticks where you dripped it and moves slowly or smears, you have protective plastic that needs to be removed. 

**Why do I need to use a bottle cap or foam when replacing the FEP film?** 

The bottle cap, or foam, will allow some slack to the film, so that when you tighten the frame down you will get approximate tension. If you don't do that, you will over tension the film and it may tear. If it didn't tear, later on you'll be wondering why all your prints fail. 



## >MODEL SETUP AND SETTINGS

**How do I use Chitubox slicer?**

Lots of video tutorials exist on youtube. 3DPrintingPro has a very good set [here](https://www.youtube.com/watch?v=TTZpvhfaNWY&list=PLC4QzbTxrEF-fA1OC_-zE_4f6n1K-w2SS).

**What settings do I need for the test (rook) file?** 

The test file that came on the included USB stick has been pre-sliced and settings configured for Elegoo generic resin. All you need to do is select the file and print. If you have a different resin, you may need to change the exposure settings. 

**I bought x resin; what are the best settings for it?** 

Every resin behaves differently; there are no best settings that will work for every resin and every machine. For a quick start, you can refer to the [community resin exposure settings](https://www.elegoo.com/pages/3d-printing-user-suupport). Those settings should enable you to get a print going quickly, but you will need to test and adjust from there to find the best settings applicable for your machine. 

**How do I find the optimal settings for my resin and machine?** 

It's usually best to start with the community resin exposure settings, and then dial them in with a few test prints. These test prints will allow you to obtain the optimum settings for your resin, in your environment, matched to your machine. A good instructional video can be found [here](https://www.youtube.com/watch?v=r9GwPEJ8Lq8).

**My resin is expired, can I still use it?** 

Generally, most resin manufacturers advise that resin be used within one year. The dates are basically "use by" dates, not expiry per se. In practice, when kept properly in a cool, dry location and unexposed to light, the resin can be stored and used without issues. 

**What do the print settings mean?**

This is assuming you're using the Chitubox slicer that is included on the USB stick. Other slicers may use different terminology, but they're functionally the same. If you're just starting out, it's highly recommended you use the Chitubox slicer. It's basic, won't overwhelm you with bells and whistles, and just works. 

**Bottom Exposures (Bottom layers):** 

This is how long the UV light will turn on to set the layer of resin that is on your build plate for the first few layers (it's extra long to give the resin the best chance to stick to your plate and form a super hard base to help keep your part from wobbling and rocking about.) For the sample green resin at 0.05mm layers, the exposure for bottom layers is 60 seconds. 

**Bottom layer (Bottom layers):**

Simple, this one it's about how many of those super hard base layers to lay down on the base of your print usually this is 5-8 layers.

**Normal exposures (Normal exposure time) :** 

After your base layers have finished, this is the time the UV will be on to cure all the rest of the layers of your print and will always be lower than your base/bottom layers setting. 

**Exposure off (Off time):**

Light off delay. This is the amount of time that the UV light is turned off between the end of one exposure cycle and the beginning of the next. After an exposure, the UV light turns off, the build plate lifts and peels, and then descends; ready for the next cycle and will wait at the bottom (resting at the set layer height over the FEP sheet, at the bottom of your vat) before the UV light comes on again for the next exposure cycle. 

Longer offtimes leave more time for the resin to settle out and form a new layer with fresh resin. This is especially useful for more viscous resins to mitigate issues of poor definition of surfaces facing the build plate.

**What is suction warping, and how do I combat it? Should I add a vent hole?**

Vent holes are often improperly called "drain" holes; they are not for draining resin. Imagine a glass full of water upside down in a bucket of water. When you pull the glass up out of the bucket, it stays full until the lip of the glass breaks the surface of the water in the bucket. 

In the vat, the lowest point of the print, the new layer does not (generally) rise above the level of the liquid resin in the vat. Therefore, the liquid resin inside the "bowl" or "cup" cannot evacuate unless you add a vent hole. This is a significant cause of failures. You have to reduce the work that the stepper motor has to do to lift the platform.

Initially, In the printer vat, the inside volume of resin will be pulled up. Eventually, depending on the volume of the inside space and the volume of resin in the vat, the new layer will rise above the fluid level because the surface of the fluid will be moving down at ever-increasing rates with each layer. That is, the level of the fluid inside the space and in the vat are actually moving in opposite directions. When that happens, all of the fluid inside will be released, but now you have a trapped volume of air, so you will alternate between struggling with lifting up and struggling with pushing down. 

Without vent holes, it's really a recipe for bad prints. The result is that you can get multiple failures at various heights, depending on where these extremes occur. Formlabs has a good article on [model orientation,venting and suction cups.](https://support.formlabs.com/hc/en-us/articles/115000018124-Model-Orientation)

**How do I hollow my model?**

It depends on the software. Two popular free programs that make it easy to hollow your models are Chitubox and Meshmixer. Give a look [here.](https://www.youtube.com/watch?v=wAW-rqrr8nc)

**Can I just use auto supports for all my models?** 

Not the best idea. For simple models, auto supports should generally work, but as with anything automatic, it will never be perfect. For a start, you can use auto supports and supplement with manual supports on parts that the software missed. But it will be best to [learn to place your supports manually](https://www.youtube.com/channel/UCbv2mDrRqXovPdahRyoCFhA/search?query=supports) and precisely; you will find that you will need less supports and produce better prints in the long run. 

**What angle should I use to minimize layer lines?**

There isn't one best angle for printing everything. It really depends on your layer height and the type of model you're printing. Don't forget that model orientation also plays a big part in determining the best angles. You could actually be losing details printing at the wrong angle for the layer height. See a detailed explanation [here](https://www.youtube.com/watch?v=Qs2Rb0ExnIM). 



## >PRINTING

**My first print, do I have to print the rook?** 

It is highly recommended that you print it. A successful test print will confirm that your printer works as it should and that you have properly leveled your build plate and your FEP tension is correct. If it did not print successfully, troubleshooting will be easier as you can rule out various other problems such as resin, settings, or slicing - additionally community assistance will be easier as it is a familiar part with easy 'reads'. 

**I'm about to start a print, but the touchscreen shows a filename highlighted in red?** 

That's normal; it's showing the last file you selected or printed. 

**How long do I have to shake the resin up or heat it?**

·  It is always best to read the resin's manufacturer's datasheet/instructions since every resin is particular and requires different mixing and operating temperature.

·  In most cases, resins don't like to be used below 21'C/70'F.

·  A non-pigmented resin getting a good shake for 30 seconds is enough, while a heavy pigmented one for a minute or two. If the resin is thicker due to low temp, add some extra time to that.

**How much resin should I pour into the vat?** 

To start, fill the VAT about half way, between the FEP surface and max fill line.. Do not exceed the max fill line; if there is too much resin, it will rise from displacement and cause a spill. Once you pour resin into the VAT, let it sit for a few minutes to let any air bubbles escape before printing. 

**Can I add resin halfway through a print?**

·  Yes, no problem. You do not have to pause the print; just slowly and gently pour the resin into the vat. Make sure to not bump or touch the build plate while pouring. Be mindful of displacement when adding resin. 

·  Make sure to mix the fresh resin well before adding. Try to ensure the resin temperature is the same.

**Can I pause halfway through a print?** 

Yes, you can pause at any time during your print. Resume as quickly as you can to ensure that your print will continue safely. However, it is generally not recommended as it will most likely leave a line at the layer where you paused. If you time your pause after a peel move, the chances of resuming without a line is better. 

**Lines or Layer Shifting on the printed model?**

See Elegoo's support guide [here](https://www.elegoo.com/blogs/3d-printer-user-guide/lines-or-layer-shifting-on-the-printed-model).

**Holes in the 3D printed model?**

See Elegoo's support guide [here](https://www.elegoo.com/blogs/3d-printer-user-guide/holes-in-the-3d-printed-model).

**I hear a rumbling / loud humming noise once I start a print?** 

If you're having issues with the build plate homing fine but then trying to bury itself into the LCD and making a rumbling/loud humming noise once a print is initiated - relevel the build plate and ensure you use Z=0.

**I hear a strange faint knock or a suction/sticking sound every time the plate lifts. Is this normal?** 

It's completely normal. It's a good sign that your print is sticking to the build plate and that the layers are releasing from the FEP film. It will be more audible during the first few bottom layers of the print, don't worry if you can't hear it later on as it depends on the layer section being printed. 

**How do I know that my print is sticking to the build plate?** 

·  One easy way to tell is by listening for the sound that's made as the layer peels off the FEP. You can hear it clearly, especially for the first few bottom layers. Don't worry if you can't hear it anymore later; it varies depending on the size of the layer being printed. 

·  You can also use the pause to check on your print, but note that you may get a line at the layer where you paused. 

**My prints are not dimensionally accurate, sometimes slightly oversized by as much as 0.3mm?**

First, ensure that your exposure settings are optimal for the resin used. Underexposure causes thinner parts, while overexposure will swell. Many of the basic resins swell when printed. There could also be slight shrinkage. It all depends on your settings and the brand of resin and formulations that manufacturers use. It usually isn't noticeable on organic prints. 

**My prints just won't stick?** 

This is almost always a build plate leveling issue. Make sure your leveling is 100% correct before attempting these other solutions. 

·  Clean the build plate carefully with IPA or other solvents. Dry before use. 

·  Shake your resin in the bottle well before using it. Resin already in the vat may have settled and need to be stirred. 

·  Preheat or warm the resin, you can use a hairdryer on most bottles to gently heat the resin to 20~30°C while swilling. 

·  Preheat the build plate, same as the resin. 

·  The build plate may have shifted. Try and level it again; make sure to tighten well. 

·  There may be cured resin in your vat. Drain and clean. 

·  Did you remember to set Z=0?

·  The FEP film may be too tight or too loose. 

·  You may be using resin formulated for SLA laser or DLP printers. Try using a known resin like the sample green. Note that some resins like maroon or yellow are very difficult to work with. 

·  Are you using a specialty monomer-free resin such as Blue cast? You may need a primer coat. Check manufacturer's recommendations. 

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

Simply put, during printing, the layers of the model facing the FEP film are always sharply defined as the layer is exposed perfectly against it. Whereas the layers facing the build plate, previously exposed, still receive UV light from diffusion/diffraction/scattering from the current exposed layer and thus will still cure slightly. This is akin to overexposure and thus details will be lost. Coupled with this, some resin always remains around the bottom parts (facing the build plate) and will also bond and cure to the details. 

This is a limitation of the technology but can be largely mitigated and overcome by the following:

·  Ensure that exposure settings are optimal for your resin. Overexposure will magnify this issue. 

·  Ensure that the model is well orientated and angled to minimize resin pooling and that important details are presented facing the FEP film. 

·  Allow enough clearance for the supports so that resin does not get trapped between the bottom of the print and the build plate.

·  Set longer UV off-times so that more viscous resins can drain during lift. It will also help to heat the resin during colder temperatures. 



## >CLEANING 

**How do I clean my prints?** 

The recommended method is the two tub system. Fill both containers with 91% Isopropyl Alcohol (IPA) or other solvents such as 95% Ethanol. Although not necessary, heating the first tub to around 45°C helps dissolve the resin faster. 

Drop the print into the first tub and swirl for several seconds. Use a soft brush on hard to reach parts, crevices, etc. Then dunk the part in the second tub of solvent and rinse clean. Do not leave your prints soaking too long in the tubs. Remove then dry thoroughly (blow-drying with compressed air works best) before UV curing. 

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

·  Manufacturers universally advise the use of a solvent like 91% IPA (Isopropyl Alcohol) or 95% Ethanol. Proprietary cleaning solutions or other solvents may also be used, such as Mineral spirits (aka White spirits, Turpentine), etc. 

·  If you have bought a water washable resin, you can simply use water and some mild soap. 

·  A small brush is very helpful to get into and clean the fine grooves or details in your prints.

·  Alcohol and other flammable solvents should not be used directly with ultrasonic cleaners because of the fire hazard.

**How long can I keep the resin in the vat?**

It depends on environmental factors and type/brand of resin. Typically if the resin is kept out of light and spared any moisture/dirt, it may sit in the vat for a few weeks. Clear resins tend to sit better; opaque resins will need more stirring before use to mix the pigments back. When in doubt, check the resin manufacturer's datasheet/recommendations. 

·  Check for loose cured resin or stuck resin, you will need to clean that out. 

·  Cover the vat, you can cut a piece of cardboard that fits over the vat, or print one out on an FDM printer.

·  Before printing, carefully stir the resin for 1 - 2 minutes with the a soft silicone spatula, be careful not to scratch the FEP screen.

·  Do not leave the build plate hanging with uncured resin, take it out and clean with IPA, leave it out until you are ready to print, this will lessen the weight on the single lead screw thus prevent deformation and potential Z wobble. 

**Can I put excess resin that doesn't get used in a print back into the original bottle?**

Yes, but always strain out any debris first using a filter.

**Water washable resin, how to dispose of the dirty water after washing the print? Wash it down the drain?** 

**Do not pour it down the drain!** Water washable resin works because it uses water-soluble monomers. Water isn't an acrylate. Water can not cure. When you dilute resin into anything that's not capable of curing, it won't be inert again. 

Even after you expose the mixture to UV, the photoinitiators in the diluted resin water will still cleave and generate free radicals. If some acrylate molecules are nearby, there will be a tiny bit of chain growth taking place. The spent photoinitiators, pigments, and the portion of the resin that actually cures will settle out, but the rest will still remain diluted in the water. 

*What this means is that resin cannot cure to completion in solution (water). It cannot cure due to a change in concentration of reactants, and there will be contaminates in the wash that are not safe down the drain.*

The only proper way to dispose of the wash is to reduce the solution by evaporation, and then collect and UV cure the resin residuals and dispose of them properly. 



## >POST PROCESSING

**My print stuck so well to the build plate that I can't remove it?** 

Congratulations on having a well-leveled plate. Sometimes prints adhere so well that removal is difficult. Try the following methods to remove recalcitrant prints, in order of recommendation:

·  Heat up the print and build plate to around 40~50°C by using a hairdryer or running them under hot water. Your print can then be easily removed. 

·  Use the provided sharpened steel scraper - place the build plate on your working surface with its edge on the working table (so the model is facing left and adjustable head facing right or vise-versa), position the steel scraper on the edge where the model and build plate interface, and then give a gentle downwards knock to the handle - fracturing the model off the plate.

·  Look at the whambam or other manufacture's removable build plate surface. 

**How long should I cure my print?**

Check the resin manufacturer's datasheet/recommendations. An easy way to find out if your print has cured enough with sunlight or a UV light set up is to find an area where you don't mind a mark and try to dent it with your fingernail. If you can, then it's not ready yet, and as soon as you can't dent it, it's ready. Do not over cure as resin may become overly brittle, and white or clear resin will turn yellow. 

**When should I remove supports?** 

It is generally best to first clean the entire print before removing any supports - this will reduce your and the work area's resin exposure. Following the cleaning process, remove the supports before UV curing as they are softer, and in many cases, you can easily pull or rub them off. In some cases, you may want to remove them after curing, especially when working with thin and delicate parts that may warp during the curing process if not supported.

**How durable are the prints? Will they break if I drop them?** 

It depends on the resin used. Unlike PLA or ABS, regular hobby-grade resin prints are quite brittle and can easily break when dropped. There are specially formulated resins for prototyping or even functional usage, which have different properties such as flexibility, hardness, and UV resistance. Once you have familiarized yourself with your printer using the sample green resin, you might want to experiment further with different resins. 

**Why do I get white chalky residue on my prints after curing?** 

The white residue appears if there's moisture or water on your prints when you UV cure. One way to avoid this is not to wash your prints in water after cleaning in solvents. Always make sure your prints are completely dry before final UV curing. 



## >MAINTENANCE AND TROUBLESHOOTING

**What maintenance do I need to do to keep my printer running well?** 

Keep everything clean by wiping down with a microfiber cloth slightly dampened with IPA. Wipe resin drops and spills off immediately with IPA and tissue. Keep your vat and FEP clean. Keep the LCD screen perfectly clean. Dust off and keep the printer's cover clean. And every two months or earlier, depending on usage frequency, clean and replace the grease for the lead screw. If it squeaks, do this immediately. 

**What grease should I use for the lead screw (Z rod)?**

Use a PTFE based or white lithium viscous grease. It should by thick, creamy, toothpaste consistency type. Can use generic machine grease, cosmoline, gel grease, gear grease, etc. Just make sure the lubricant is not thin and runny. Do NOT use WD-40!
Watch the Official Elegoo instructional video [here](https://youtu.be/OWXlZSi15cE).

**How do I replace the grease on the lead screw?** 

Wipe all the old dirty grey grease off with a cloth rag or kitchen towels. Then really get it clean by wiping again with solvent and use a toothbrush to get between the threads. IPA works great. Make sure solvent doesn't drip down into the stepper motor beneath. When it's clean and dry, regrease with good quality grease, apply by dabbing onto the entire length of the screw, then switch on the printer and run the slide block up and down. 

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



## >ACKNOWLEDGMENTS

**Where did all this information come from?** 

Most of the information, insights, tips, and tricks were gathered from the [Photonsters](http://photonsters.org) team documentation, [Elegoo product site](https://www.elegoo.com/), [Elegoo Mars reddit](https://www.reddit.com/r/ElegooMars/), and various others. Photonsters.org is a great team and has a wealth of information, always worth is visit. 
