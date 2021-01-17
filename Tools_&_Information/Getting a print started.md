**Powering on the Printer.**
1. Check the power adapter, ensure it's firmly plugged into the wall outlet - you should see a blue LED (on the transformer brick) to indicate that it has mains power.
2. Plug the DC end of the power adapter into the receptacle at the rear of the printer. Check the power switch is in the "ON" position.
3. The front LCD touch panel should greet you with a graphical display.

**Leveling the build plate, checking the UV light, and readying the resin.**
1. If the build plate is not at least half-way up, raise it by selecting the 'Tool' Button, 'Manual' Button, '10mm' Button, then Up Bottom. Each time you press this, it will raise only 10mm, so you may have to press this multiple times.
2. Remove the build plate by turning the top black rotary knob (on the Z-axis) in a counter-clockwise direction, enabling the build plate to be slid towards you. Do not remove the rotary knob; only rotate it enough to slide the plate off.
3. Ensure the build plate is clean and free of any resin or gunk; gently scrape if needed.
4. Grab the desired resin, check the recommended printing temperature, and ensure you sliced your model using the correct resin profile. Shake the resin bottle well (vigorously) for about 5 minutes. Wrap the resin bottle and build the plate in a heating pad and warm until it is at the proper temp.
5. As you are warming the resin bottle and build plate, ensure your sliced model is on the printer's network share drive.
6. Once warmed and at the proper temp, clean the build plate surface with alcohol and lint-free cloth. Slide the build plate back onto the printer's Z-axis and tighten the rotary knob.
7. Remove the resin vat and place it on its side, in an area where you won't knock it. Check the top LCD free and clean. If dust or residue is present, remove using a clean microfiber cloth - apply alcohol if needed. !Only use microfiber cloth!
8. Test the UV light source by selecting the 'Tool' button, 'Exposure' button, adjust for a few seconds and select the 'Next' button to begin. You should see a complete rectangular image on the top LCD; the front touchscreen should display the same.
9. Get a standard sheet of printer paper, cut it in half, and place it over the top LCD screen.
10. Loosen the two bright hex-head bolts on the build plate head using the large hex wrench - one is on the front, the other on the side. Do not unscrew completely, just enough to allow the build plate to rotate freely as well as up and down.
11. Home the Z-axis by selecting the 'Tool' button, 'Manual' button, and Home button (looks like an upside-down T).
12. The build plate will go down to the paper, slightly rise, and then down again. Check the build plate's alignment and rotate as needed to ensure it is square with the printer. Gently tighten the forward-facing hex-head bolt first, followed by the side facing.
13. Gently try to pull the paper out, not all the way but just only by a few millimeters or so. If the paper is unable to move, raise the build plate 0.1mm by first selecting the '0.1mm' button, followed by the Up button - this is not always required, only if you feel the paper will tear when pulling.
14. Select the 'Z=0' button, and select confirm. Raise the build plate by pressing the 10mm button, followed by the up button, at least seven times. Remove the paper.
15. Grab the resin vat. Check it free and clean - both sides. And again, check the top LCD free and clean. If dust or residue is present, remove using a clean microfiber cloth - apply alcohol if needed. !Only use microfiber cloth!
16. Gently slide the resin vat into position, taking care to glide it in with a slight upward force against the securing towers and not the LCD screen (the vat film and LCD screen scratch easily). Ensure the vat is in place before screwing in the two-tower side bolts by feeling a small detent position where it sits securely without wobble. The max resin fill indication should be visible from the front, and the resin pour-out groove should be closest to you on the tank's bottom right.
17. Grab the now warmed resin, shake it gently for an additional minute or so, then slowly and carefully fill the vat to just below the max line.
18. Let the resin in the vat sit for a few minutes to let any air bubbles escape.
19. Begin printing your sliced model's CTB file from the front touch screen or the webpage interface.

-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-

**A note on Homing, Leveling, Z=0, Step 14:**

-The 'Home' button brings to build plate down until the endstop is triggered. This is 'mechanical' Z0, homed position.
-The 'Z=0' button adds, or subtracts, to this value based on where you have positioned Z after, it was homed, and pressed 'Z=0'. This is your Z offset.
-If you're having issues with the build plate homing fine but then trying to bury itself into the LCD once a print is initiated - relevel the build plate and ensure you use Z=0.

So, let's say you are leveling the printer, loosened the screws, and press home. You tug on the paper, it feels tight, so you raise by .1mm, then hit 'Z=0' because you raised Z. With this, once you home again, the build plate will still stop at mechanical zero because homing stops at the endstop trigger. If you looked at the electrical position of Z, it would read Z:-0.1. This is all good, and now we know that when we initiate a print, it will home and then go to Z offset (raise .1mm), and then start the print.
Flash forward several prints later, and you level the machine. You place your piece of paper on the LCD, loosen the screws, and press home. This time you tighten the screws and then remove the paper with no significant tension/friction and think that you don't have to press 'Z=0' because you didn't move Z to take out the paper... WRONG - This is what gives people issues - IF you don't press Z=0, the printer will still have an offset of 0.1mm from the previous leveling, and you may run into problems due to incorrect leveling - because it's 0.1mm off.
Remember, homing goes to mechanical zero when the endstop is triggered and doesn't care about the offset! 

Try this for fun: Home and then raise Z by 10mm, press Z=0, and then home again to see where it stops - it will stop when the endstop is triggered, and it will seem as if the Z=0 did nothing. Then, with vat out and no resin, start a print for - it will home and then begin to print 10mm above the LCD.
So, long story short, when leveling and you're happy with the paper pull test - whether you bumped Z height or not, press 'Z=0'.

-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-

**A note on equipment operating temperature:**

Not only does the resin have a stated operational temperature to be maintained, but also the FEP. If the FEP is too cold, it will not have the proper elasticity and will increase the object's peel force - increasing the odds of a failed print 'stuck to the bottom'. Additionally, operating below the recommended temperature could also make the FEP more prone to damage.

Tensile Strength @ 73°F: 2100-3050psi / 14.5 to 21 MPa
Elongation @ 73°F: 240 - 300%
Yield Strength @ 73°F: 1740psi / 12 MPa

**To ensure proper FEP elasticity is yielded, operate the equipment in an environment of at least 20C, 23C and above being optimal.** 

-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-

**Question: Do you really shake the bottle for 5 minutes?**

I've always been doing it for maybe 10 sec, and everything's fine.
Answer: I'd say if 10 seconds works for your use case, then stick with it - When in any doubt, read the mfg instructions.

I usually shake the resin for 3 - 5 minutes, then warm with a heating pad until the proper temperature is obtained - 25C if the resin mfg doesn't specify, and then gently shake the bottle back and forth just a bit before pouring it into the resin vat. I have found that different brands, with varying resin types, with differing pigmentation levels, can need quite a bit of mixing to not so much. The resin's temp will also factor in how well it mixes, mostly due to viscosity, and subsequently, this dictates how fast the bubbles will escape the liquid due to reduced surface friction/tension.

-For example, from Siraya Sculpt: "To get the best results out of Sculpt, SHAKE HARD (applies to all resins with pigments) To do it correctly to shake that bottle for 20-30s before use. Stir up the resins that is already in the vat before each print. And if you just received Sculpt, before opening it up for the first time, turn it upside down for a minute (submerged in warm water is even better) and then shake for another minute or two to make sure you get a great mix. IF you want to take it to the next level, throw a small metal ball in there and shake, the object will significantly increase the efficiency of mixing pigments and resins."

-On a lesser impacting example, professional/commercial side of the house, with similar resin, is supposed to be mixed for 1 hour for a brand new bottle and 10 minutes after the first initial use – and that's using a mixer machine like the LC-3D.

Granted, the equipment here is not at the same level as those machines, but the resin is related. I think in most cases, a non-pigmented resin getting a good shake for 30 seconds is enough, while a heavy pigmented one for a couple of minutes. If the resin is thicker due to temp, add some extra time to that, and since a few minutes doesn't cost me anything, I bring it out to 3 - 5 to make it easy - 3 for clear and up to 5 for heavy pigment. In my environment, I already know the temp is not where it should be, so the resin bottle is wrapped in a heating pad and brought up to temp – this usually takes 10 minutes or more. The heating process kills two birds with one stone, first and foremost warming the resin and secondly letting the air bubbles from the mixing action escape. When it is at temp, just a gentle back and forth shake for a minute to mitigate the case of any compounds settling.

So, to bring my thought back full circle, I stand by the stated instructions to say 5 minutes. I don't know what resin they are grabbing, its state, or the temp. On the flip side, I know a 5-minute shake won't hurt it, but it will bring bubbles. I know ten plus minutes sitting and getting warmed will ensure the proper temp and let the bubbles escape. And I know the last gentle shake will provide any settled pigment or additives mixed without making more bubbles.

Apologies for the long reply, but I wanted to advocate my thought process clearly. But again, if 10 seconds works, then stick with it - all that matters is that you're getting good prints :)
