# Alpenmeister Meisterbox S 

![A leverless controller with a shell printed in black and white. The controller has a lid with a white logo on black background and a white groove. To the side of the shell lid a two closure tabs. The controller itself has 14 black or white buttons with low profile keycaps.](pictures/knochen_overview.jpeg "Overview of the Meisterbox S")

The goal here was to build a controller that is pocket sized, great for travelling (to locals) and that is, as the name suggests, an actual box. You can just wrap your USB cable around it and put it in your pocket, because it's barely larger than a large smartphone and weighs just below 200g.

It comes with an acrylic cover so you can put in your favorite artwork. Passthrough port on the side. Switches are Kailh choc v1. Button caps are 1U and 1.5U MBK. The layout is the Meisterlayout with two thumb buttons, two pinky buttons and a center button. It's designed as ergonomic as possible and sized down to the smallest footprint possible.

P.S. Why Knochen? Knochen means bone in German and the initial idea was to wrap the USB cable vertically, which would make it sort of shaped like a stylized dog bone.

## Case files

The repository contains five STLs in the `stls_to_print` folder which you'll need to print to make the Meisterbox S:

* 1x knochen-bottom.stl: the bottom of the shell
* 1x knochen-top.stl: the top of the shell
* 2x knochen-hinge_pin.stl: the pin used for the hinges
* 2x knochen-hinge_cap.stl: the cap to put on the hinge pin. This should be a press-fit which will be more or less tight depending on materials and print settings. You might need some force to put it on the pin or it might be loose. You can always glue this to the hinge with a little CA glue if you want
* 2x knochen-hinge_closure.stl: the closure tabs to make sure the top of the controller doesn't fall off

You might need to orient the items on your print bed. We managed to print everything together on the 180mmx180mmx180mm print bed of a Bambu Lab A1 mini. This build has been tested in PLA and PETG. Our recommendation is using PETG if you can since that would make sure your controller won't warp when exposed to heat or become brittle because of sun exposure. If you use this controller to travel, those might be some conditions it might get exposed to.

If you want to change anything about the design, check out `project_files/knochen.FCStd`. You can open the file using FreeCAD and change anything you'd like.

You will also find optional files for the acrylic cover `optional/meisterboxs-acrylic.step` and a cutout file for artwork `optional/meisterboxs-acrylic.dxf`.

## Additional Hardware

You'll need some other hardware to assemble the whole controller:
* 1x Meisterbox S PCB
* 14x Choc V1 switches
* 9x 1U Choc V1 keycaps (you could print these if you'd like)
* 5x 1.5U Choc V1 keycaps (you could print these if you'd like)
* 4x 10x10mm Chicago screws (e.g. https://de.aliexpress.com/item/1005004649666564.html)
* 1x acrylic top plate (see `optional` files. Can also be printed)
* 1x USB-C cable (we recommend right-angled, braided)



