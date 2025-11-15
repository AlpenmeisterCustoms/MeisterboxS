# Alpenmeister's Meisterbox S v1   

![A leverless controller with a shell printed in black and white. The controller has a lid with a white logo on black background and a white groove. To the side of the shell lid a two closure tabs. The controller itself has 14 black or white buttons with low profile keycaps.](pictures/knochen_overview.jpeg "Overview of the Meisterbox S")

Meisterbox S © 2024 by Alpenmeister is licensed under [Creative Commons Attribution-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/)

# ATTENTION: THIS IS PAGE AND CONTROLLER IS NOW DEPRECATED.  
# [PLEASE CONTINUE HERE TO VERSION 2](https://github.com/AlpenmeisterCustoms/AlpenmeisterS-v2).

The goal here was to build a controller that is pocket sized, great for travelling (to locals) and that is, as the name suggests, an actual box. You can just wrap your USB cable around it and put it in your pocket, because it's barely larger than a large smartphone and weighs just below 200g.

It comes with an acrylic cover so you can put in your favorite artwork. Passthrough port on the side. Switches are Kailh choc v1. Button caps are 1U and 1.5U MBK. The layout is the Meisterlayout with two thumb buttons, two pinky buttons and a center button. It's designed as ergonomic as possible and sized down to the smallest footprint possible.

P.S. Why "Knochen"? Knochen means bone in German and the initial idea was to wrap the USB cable vertically, which would make it sort of shaped like a stylized dog bone.

## Case Files

The repository contains five STLs in the `stls_to_print` folder which you'll need to print to make the Meisterbox S:

* 1x `knochen-bottom.stl`: the bottom of the shell
* 1x `knochen-top.stl`: the top of the shell
* 2x `knochen-hinge_pin.stl`: the pin used for the hinges
* 2x `knochen-hinge_cap.stl`: the cap to put on the hinge pin. This should be a press-fit which will be more or less tight depending on materials and print settings. You might need some force to put it on the pin or it might be loose. You can always glue this to the hinge with a little CA glue if you want
* 2x `knochen-hinge_closure.stl`: the closure tabs to make sure the top of the controller doesn't fall off

You might need to orient the items on your print bed. We managed to print everything together on the 180mmx180mmx180mm print bed of a Bambu Lab A1 mini. This build has been tested in PLA and PETG. Our recommendation is using PETG if you can since that would make sure your controller won't warp when exposed to heat or become brittle because of sun exposure. If you use this controller to travel, those might be some conditions it might get exposed to.

If you want to change anything about the design, check out `project_files/knochen.FCStd`. You can open the file using FreeCAD and change anything you'd like.

You will also find optional files for the acrylic cover `optional/meisterboxs-acrylic.step` and a cutout file for artwork `optional/meisterboxs-acrylic.dxf`.

## PCB Files

You can find the files necessary to order the PCB in `pcb/`. Ordering the PCBs will need some caution. If you want to order the boards please closely follow the instructions.

### How to Order the PCBs
1. Go to JLCPCB.com
2. Click on "Order now"
3. Click on "Add gerber file" and choose "MeisterboxS_gerber.zip"
4. Use the following options, mostly  defaults, those that need changes are highlighted:
    - Base Material: FR-4
    - Layers: 2
    - Dimensions: do not touch
    - PCB Qty: 5 is minimum
    - Product Type: Industrial/Consumer electronics
    - Different Design: 1
    - Delivery Format: Single PCB
    - PCB Thickness: 1.6mm
    - **PCB Color: choose your color, we would recommend black**
    - Silkscreen: White
    - Surface Finish: HASL, choose with lead or LeadFree
    - Outer Copper Weight: 1oz
    - Via Covering: Tented
    - Min via hole size/diameter 0.3mm
    - Board Outline Tolerance: +/-0.2mm
    - **Confirm Production file: Yes**
    - **Mark on PCB: Remove Mark**
    - Electrical Test: Flying Probe Fully Test
    - Gold Fingers. No
    - Castellated Holes: No
    - Edge Plating: No
5. Use the switch next to "PCB Assembly"
6. Use the following options for PCB Assembly, mostly defaults, those that need changes are highlighted:
    - PCBA Type: Economic
    - Assembly Side: Top Side
    - PCBA Qty: Choose the same amount as PCB Qty
    - Tooling holes: Added by JLCPCB
    - **Confirm Parts Placement: Yes THIS IS VERY IMPORTANT, JLCPCB will make a production file to match the files we provide, please check if all components are where they should be**
    - Parts Selection: By Customer
    - Advanced Options don't touch and leave as defaults
7. Click "Next"
8. Click "Next"
9. Click "Add BOM" File and choose "MeisterboxS_bom.csv", then click "Add CPL File" and choose "MeisterboxS_CPL.csv". Then click "Process BOM & CPL"
10. You will then be presented with the components that are used on the board, they should be in stock and selected. Only then click "Next". Do not proceed if some are missing and you don't know what they do.
11. You will then see a prompt saying "The system detects components that may be offset from the PCB, does it try to automatically align it?" (sic). Click "Cancel". You will then see that the USB ports and top switches are misaligned. Select the USB ports and move them a bit inwards. Then select the top switches and rotate them 180°. Try to align them with the holes in the board. You do not have to be precise, this is just an indication of how you want the parts to be placed, the final placement in the production file will be done by a JLCPCB employee. Click "Next" when finished.
12. You will then see the costs of production. Choose a "Product Description" on the right side "Research/Eduction/DIY/Entertainment" > "DIY - HS Code 902300". This is for the customs declaration. "Click "Save to cart".
13. You'll be in your cart. Select the PCB we just configured and then go through the "Secure Checkout"

Please bear in mind: Do this at your own risk. It is your own responsibility to do the ordering process. We are not responsible for any mistakes in this instruction, as the actual ordering process might change at any time.



## Additional Hardware

You'll need some other hardware to assemble the whole controller:
* 14x Choc V1 switches
* 9x 1U Choc V1 keycaps (you could print these if you'd like)
* 5x 1.5U Choc V1 keycaps (you could print these if you'd like)
* 4x 10x10mm Chicago screws (e.g. https://de.aliexpress.com/item/1005004649666564.html)
* 1x acrylic top plate (see `optional/` files. Can also be printed)
* 1x USB-C cable (we recommend right-angled, braided)



