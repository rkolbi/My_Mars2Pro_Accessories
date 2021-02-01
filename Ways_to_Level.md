**:wrench:Ways to Level the Build PLate**  

**Remember** that as you tighten the front and side securing screws, it can move the plate by a tiny fraction - when tightening the bolts, always keep a hand gently pressing the build plate down and level.  
**I set Z=0, but when I press Home, the position is different?**  
Home is not Z=0! Home is fixed; it is the hardware Z endstop. Unless you change it physically, it will always be in the same position. Z=0 is the offset distance between Home and your LCD screen; you define during the leveling process when you set Z=0, that's why you have to Home first, then move the platform, then set Z=0.   When a new Z=0 is specified, pressing Home will NOT move the platform to the position you set; it will be the start position when a print is initiated. You can check it by removing the vat and starting an air-print.  


**:wrench:Preferred Method - Step by step follows:**  
- [ ] If the build plate is not at least halfway up, raise it by selecting the 'Tool' Button, 'Manual' Button, '10mm' Button, then Up Bottom. Each time you press this, it will raise only 10mm, so you may have to press this multiple times.  
- [ ] Remove the build plate by turning the top black rotary knob (on the Z-axis) in a counter-clockwise direction, enabling the build plate to be slid towards you. Do not remove the rotary knob; only rotate it enough to slide the plate off.  
- [ ] Optional but recommended: Test the UV light source by selecting the 'Tool' button, 'Exposure'  button, adjust for a few seconds, and select the 'Next' button to begin.  You should see a complete rectangular image on the top LCD; the front touchscreen should display the same.  
- [ ] Ensure the build plate surface is clean and free of any resin or gunk; gently scrape if needed. Clean the build plate surface with alcohol and lint-free cloth.  
- [ ] Loosen the two bright hex-head bolts on the build plate head using the large hex wrench - one is on the front, the other on the side. Do not unscrew completely, just enough to allow the build plate to rotate freely as well as up and down.  
- [ ] Remove the resin vat and place it on its side, in an area where you won't knock it. Check the top LCD free and clean. If dust or residue is present, remove using a clean microfiber cloth - apply alcohol if needed. !Only use microfiber cloth!  
- [ ] Get a standard sheet of printer paper, cut it in half, and place it over the top LCD screen.  
- [ ] Slide the build plate back onto the printer's Z-axis and tighten the rotary knob.  
- [ ] Home the Z-axis by selecting the 'Tool' button, 'Manual' button, and Home button (looks like an upside-down T).  
- [ ] The build plate will go down to the paper, slightly rise, and then down again. Check the build plate's alignment and rotate as needed to ensure it is square with the printer.  
- [ ] While gently pressing down on the build plate, ensuring it is completely flat and square, tighten the forward-facing hex-head bolt first, followed by the side facing.  
- [ ] Gently try to pull the paper out, not all the way but just only by a few millimeters or so. Try the pull test from the left and then the right edges. If the paper is unable to move, raise the build plate 0.1mm by first selecting the '0.1mm' button, followed by the Up button - this is not always required, only if you feel the paper will tear when pulling. !If one side was easier than the other, loosen the screws, press home, go up two steps.  
- [ ] Select the 'Z=0' button, and select confirm.  
- [ ] After setting Z=0, verify that it is set correctly by starting a dry-run print, leaving the piece of paper on the screen, and checking that the build plate starts the first layer at the correct Z=0 position have set. !Remember that Z=0 is not the same as Home.  
- [ ] Raise the build plate by pressing the 10mm button, followed by the up button, at least seven times. Remove the paper.  
- [ ] Grab the resin vat. Check it free and clean - both sides. And again, check the top LCD free and clean. If dust or residue is present, remove using a clean microfiber cloth - apply alcohol if needed. !Only use microfiber cloth!  
- [ ] Gently slide the resin vat into position, taking care to glide it in with a slight upward force against the securing towers and not the LCD screen (the vat film and LCD screen scratch quickly). Ensure the vat is in place before screwing in the two-tower side bolts by feeling a small detent position where it sits securely without wobble. The max resin fill indication should be visible from the front, and the resin pour-out groove should be furthest from you on the left.


**:wrench:Alternate Method 1 - Step by step follows (With Clean & Empty VAT in place):**  
- [ ] If the build plate is not at least halfway up, raise it by selecting the 'Tool' Button, 'Manual' Button, '10mm' Button, then Up Bottom. Each time you press this, it will raise only 10mm, so you may have to press this multiple times.  
- [ ] Remove the build plate by turning the top black rotary knob (on the Z-axis) in a counter-clockwise direction, enabling the build plate to be slid towards you. Do not remove the rotary knob; only rotate it enough to slide the plate off.  
- [ ] Ensure the build plate surface is clean and free of any resin or gunk; gently scrape if needed. Clean the build plate surface with alcohol and lint-free cloth.  
- [ ] Loosen the two bright hex-head bolts on the build plate head using the large hex wrench - one is on the front, the other on the side. Do not unscrew completely, just enough to allow the build plate to rotate freely as well as up and down.  
- [ ] Check the FEP free and clean. If dust or residue is present, remove using a clean microfiber cloth - apply alcohol if needed. !Only use microfiber cloth!  
- [ ] Slide the build plate back onto the printer's Z-axis and tighten the rotary knob.  
- [ ] Home the Z-axis by selecting the 'Tool' button, 'Manual' button, and Home button (looks like an upside-down T).  
- [ ] The build plate will go down to the FEP, slightly rise, and then down again. Check the build plate's alignment and very gently rotate as needed to ensure it is square with the printer.  
- [ ] While gently pressing down on the build plate, ensuring it is completely flat and square, tighten the forward-facing hex-head bolt first, followed by the side facing.  
- [ ] Select the 'Z=0' button, and select confirm.  


**:wrench:Alternate Method 2 - Step by step follows (With Resin Filled VAT in place):**  
- [ ] If the build plate is not at least halfway up, raise it by selecting the 'Tool' Button, 'Manual' Button, '10mm' Button, then Up Bottom. Each time you press this, it will raise only 10mm, so you may have to press this multiple times.  
- [ ] Remove the build plate by turning the top black rotary knob (on the Z-axis) in a counter-clockwise direction, enabling the build plate to be slid towards you. Do not remove the rotary knob; only rotate it enough to slide the plate off.  
- [ ] Ensure the build plate surface is clean and free of any resin or gunk; gently scrape if needed. Clean the build plate surface with alcohol and lint-free cloth.  
- [ ] Loosen the two bright hex-head bolts on the build plate head using the large hex wrench - one is on the front, the other on the side. Do not unscrew completely, just enough to allow the build plate to rotate freely as well as up and down.  
- [ ] Ensure there are no solidified/hardened pieces of resin present in the VAT. Ensure the FEP surface is smooth by gently raking a soft silicone spatula across all of its surface area. :warning: If roughness exists; stop the leveling process, filter the VAT's contents back into the resin bottle, clean the VAT, and then restart leveling :warning: Damage to the FEP and LCD screen is possible when debris exists between the FEP and build plate.   
- [ ] Slide the build plate back onto the printer's Z-axis and tighten the rotary knob.  
- [ ] Home the Z-axis by selecting the 'Tool' button, 'Manual' button, and Home button (looks like an upside-down T).  
- [ ] The build plate will go down to the FEP, slightly rise, and then down again. Check the build plate's alignment and very gently rotate as needed to ensure it is square with the printer.  
- [ ] While gently pressing down on the build plate, ensuring it is completely flat and square, tighten the forward-facing hex-head bolt first, followed by the side facing.  
- [ ] Select the 'Z=0' button, and select confirm.
