# 3d Printable High-Traction Silicone Wheels: (re-engineered for D-Shaft)

This project provides a comprehensive, open-source hardware solution for manufacturing high-grip robot wheels using Platinum Cure Silicone. While inspired by the original DrumBotics design, this iteration has been fundamentally re-engineered to support the needs of builders who may not have the luxury of pausing 3D prints to insert hardware or the ability to source specific tiny nuts and bolts. 

By utilizing a precision-engineered direct-fit D-bore, these wheels mount securely to N20 micro-gear motors without the need for any external set-screws or bolt tightening. This makes the design ideal for those who choose to outsource their 3D prints, as the final product requires no mid-print manual intervention. Both **STL files** (for immediate printing) and **STEP files** (for easy editing and customization) are included for the mold and the rim.

---

###  Design Philosophy and Technical Specs
The core of this design focuses on mechanical reliability and weight optimization. The wheel rim features a specialized 8-spoke "T-hook" geometry which creates a permanent mechanical bond with the silicone tire, ensuring the tread cannot slip off during high-torque maneuvers. To maintain a low weight for agile robots like line-followers and large-size micromice, the rim includes cylindrical cut-outs. The mold itself is a lid-free, dual-cavity design crafted to minimize material usage and print time.

| Component | Dimensions / Stats | Notes |
| :--- | :--- | :--- |
| **Total Wheel Diameter** | 42 mm | Includes 1 mm internal traction grooves |
| **Wheel Thickness** | 20 mm | Optimized for maximum surface contact |
| **Rim Radius** | 13.67 mm | 8-spoke "T-hook" mechanical anchors |
| **Shaft Interface** | 3 mm D-Bore | Direct-fit design; no screws or bolts |
| **D-Bore Tolerance** | ± 0.3 mm | Refined for a press-fit, slip-resistant finish |
| **Predicted Rim Mass** | ~9.12 g | Calculated for PLA at 100% infill |
| **Predicted Mold Mass** | ~92.6 g | Calculated at 100% infill for reference |
| **Mold Dimensions** | 105 x 56 x 26.5 mm | Material-efficient, lid-free construction |

---

###  Fabrication & Material Guidelines

**3D Printing Strategy**
* **Rims:** Should be printed at **maximum infill** (100%) to ensure the D-bore remains rigid and resistant to wear over time. 
* **Molds:** Designed to be material-efficient; printing at a **low infill (approximately 20%)** provides sufficient strength while reducing filament consumption. 
* **Tested Material:** The primary documentation and tolerances are based on **PLA** for both the rim and mold.

**Tolerance Testing**
Because every 3D printer and material handles tolerances differently, a dedicated `D_Bore_Test.stl` is provided. This is especially critical for anyone who chooses to use materials other than PLA, as different plastics may change the tolerance and cause a misfit. It is highly recommended to print this small test piece first to verify your motor shaft fit before committing to a full print. 

**Silicone Selection and Handling**
This design was validated using [Bluebird Platinum Silicone](https://bluebirdarts.pk/products/bluebird-platinum-silicone-liquid-rubber-set-of-1-kg-epoxy-mold-making), which is a bubble-free mixture ideal for high-quality DIY molding without a vacuum chamber.
* **Mixing Ratio:** 1A : 1B by weight.
* **Color:** Translucent (A), Translucent (B), and Translucent after curing.
* **Volume:** Approximately 17 ml of silicone mixture is used per wheel (measured by syringe).

**Casting Tips**
* **Release Agent:** You can use mold release wax or petroleum jelly (Vaseline) spread perfectly without leaving any bulged residue.
* **Syringe Discipline:** Keep track of which syringe you use for each liquid (A or B). A mistaken swap can cure the silicone inside the syringe or the bottle, ruining your entire kit.

> [!IMPORTANT]
> **Thermal Curing Warning:** If you are printing your mold in **PLA**, you must avoid thermal curing. PLA has a low glass transition temperature (~60°C). Attempting to cure silicone at high heat (such as 100°C) will warp the mold and ruin your precision tolerances.

---

###  Assembly and Casting Process

To achieve perfect concentricity and avoid misplacement or off-centering, do not use 3D-printed alignment shafts, as they will be rough and create complexity. Instead, utilize the actual steel D-shafts from an old N20 motor. 

1. **Shaft Extraction:** Open the gearbox of an old N20 motor with screws and tear it down using pliers to remove the D-shaft.
2. **Mold Setup:** Insert these steel shafts through the bottom of the mold cavity from beneath to center-align the wheel rims before pouring the silicone. 
3. **Symmetry:** This setup ensures the wheel remains perfectly centered and symmetrical during the curing process.

---

###  Design Reference

![Hub Geometry - 8 Spoke Design](Screenshot_2.jpg)
*Figure 1: Isometric view of the 8-spoke "T-hook" anchors and weight-reduction cuts.*

![Mold Cavity Section](Screenshot_4.jpg)
*Figure 2: Section view of the dual-cavity mold showing the integrated traction teeth.*

---

### ⚖️ Attribution & Support
Original inspiration by **DrumBotics**. This project provides a hardware-free alternative for the robotics community, specifically targeted at those who need a reliable D-shaft fit without complex assembly.

**Original Inspiration:** [DrumBotics - Silicone Wheels Tutorial]([https://youtu.be/wSwuph2TElI?si=L_Lbu_0M20XGUKMt])
