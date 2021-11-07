# 3D Printing Tutorial

## Content

This Tutorial is divided in three main topics:

- [Theorie]()
- [How to print]()
- [Troubleshooting]()

---

### Theorie

3D Printer are machines for an Additive Manufacturing process and add material instead of
removing it like a milling machine (CNC). There are a lot of different printing technologies
developed over time. In the following, we will look at the three most popular techniques.

![3D_Printing_01_Additive_Manufacturing](doc/3D_Printing_01_Additive_Manufacturing.png)

 > Picture of an FDM printer (Source: esa-automation.com)

##### FDM Printing (Fused Deposition Modeling)

![3D_Printing_02_FDM_Printer.png](doc/3D_Printing_02_FDM_Printer.png)

> Cetus 3D Printer, a FDM printer, at the RapLAB  (Source: raplab.arch.ethz.ch)

This is the most popular as well as the easiest and cheapest solution to an additive
manufacturing process. FDM Printing use a filament out of plastic. The most popular
filaments in the consumer market are ABS ( Acrylnitril-Butadien-Styrol) and PLA (Polylactic
Acid). The printer head heats the inserted material up distributes it in three axes. By
extruding layer by layer, it reproduces the given 3d model.
As already mentioned, it is relatively cheap and easy to print with this method. On the other
hand, this method works with a visible layer structure, and you need to print support
structure for overhangs above 45 degrees.
Both procesess will need post-process work to get a result with a smooth surface.
Possibilities include sandpaper, filler etc. The final model can also be (spray-) painted.

![3D_Printing_03_FDM_Model.png](doc/3D_Printing_03_FDM_Model.png)

> A typical result from a FDM printer. The layerstrucutre is visible and overhangs up to 45 degrees can be printed without support structure (Source: prusa3d.com)


##### SLA (Stereolithography) Printing


![3D_Printing_04_SLA_Printer.png](doc/3D_Printing_04_SLA_Printer.png)

> A SLA printer. In the bottom is a container with the resin as well as the light diode that fixes the resin to the building plate. The model is printed upside down. (Source: formlabs.com)

This is the oldest 3d printing technology. Invented in the 70s uses this printer, light that fixes
a liquid resin. Other than the FDM printer this system works upside down. The print platform
lifts out of the resin basin. The light technologies enable the highest resolution for the
additive manufacturing mentioned here. Perfect smooth surfaces without visible layers are
possible.
Disadvantages to this technology: The printers are very expensive, and the resin is toxic if it
is not fixed with UV light. A well-ventilated room and safety gear is mandatory. Support
structures are also needed for SLA printing.

![3D_Printing_05_SLA_Model.png](doc/3D_Printing_05_SLA_Model.png)

> The result of an SLA printer has a much higher resolution than a fdm printer. The corners are sharper and the layerstructure is barley visible. (Source: 3dprinterbank.com)


##### SLS (Selective Laser Sintering) Printing
