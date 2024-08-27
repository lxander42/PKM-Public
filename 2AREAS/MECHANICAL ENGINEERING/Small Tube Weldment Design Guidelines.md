---
created: 2024-08-26
modified: 2024-08-26
tags:
  - SOP
---
# About
This page is an introduction to tube weldments, designed to point the user to pertinent information for tube weldment design.

# Supporting documentation
- SEMI Standards 
	- SEMI F20 – Specification for 316L stainless steel bar, forgings, extruded shapes, plate, and tubing for components used in general purpose, high purity and ultra-high purity semiconductor manufacturing applications 
	- SEMI F19 – Specification for the surface condition of the wetted surfaces of stainless steel components
	- SEMI E49.8 – Guide For High Purity And Ultrahigh Purity Gas Distribution Systems In Semiconductor Manufacturing Equipment

# Materials 
- 316L Stainless Steel per Semi F20
	- General purpose (GP) grade – for components intended for use in chemical distribution systems of semiconductor manufacturing facilities that do not have stringent cleanliness requirements. Examples are clean dry air and vacuum lines.
	- Hi purity (HP) grade – for components intended for use in high performance capability chemical distribution systems of semiconductor manufacturing facilities.
	- Ultra-high purity (UHP) grade – for components intended for use in advanced chemical distribution systems of semiconductor manufacturing facilities in which optimum resistance to corrosion and contamination in critical process chemicals are required.
- Alloy 22 (UNS NO6022)/HASTELLOY® C-22® alloy

# Fabrication/Design
- Orbital weld clearances
	- Minimum of .25" clearance between welded components

[DPG Engineering-DPG Wiki - Tube Weldment Design (sharepoint.com)](https://lamresearch.sharepoint.com/sites/DPGEngineering-DPGWiki/SitePages/Tube%20Weldment%20Design.aspx?web=1)

# Design Checklist
- [ ] Fit check in next higherassembly. Make sure no interferences and fully constrained
- [ ] Standard tubing sizes used, however, tubing diameter should match welded component diameter
	- .125" - .028" wall 
	- .25" - .035" wall\
	- .375" - .035" wall
	- .5" - .049" wall
- [ ] Glands of opposing parts to be assembled in CAD with a distance of .02" to fit VCR gasket. Assess distance if using other gasketing material
- [ ] Minimum .25" distance between orbitally welded components
- [ ] Standard PNs used for OTS parts
- [ ] MBR of 8x diameter when possible. If not, assess actual MBR.
- [ ] Label is modeled with dummy text in CAD
- [ ] Poke yoke features used where available/applicable (i.e. alternating male/female ends)
- [ ] Part is fully released and PLM system matches CAD

# Drawing Checklist
- [ ] Title/Description match PLM system
- [ ] Tolerances adhere to [Block Tolerance Standards](Block%20Tolerance%20Standards.md)
	- ![Block Tolerance Standards](Block%20Tolerance%20Standards.md#^cc7d53)
- [ ] Non-critical features are defined with +/- or block tolerances
- [ ] Critical features are defined per [GD&T Guidelines](GD&T%20Guidelines.md) which convey design intent
- [ ] Material notes are per [Standard Material Notes](Standard%20Material%20Notes.md)
- [ ] Appropriate finish callout per [[Standard Finish Notes]]
- [ ] Part marking note: SILKSCREEN/PAINT/ELECTROCHEMICAL ETCH/LASER ETCH (CHOOSE 1) PART NUMBER AND REVISION WITH .XX" HIGH CHARACTERS IN APPROXIMATE LOCATION SHOWN. 
- [ ] Clean specification if required
- [ ] Box notes match appropriate features
- [ ] All child parts are released
- [ ] Standard notes
	- [ ] ALL BEND RADII SHALL BE X.XX" MAX/MIN.
	- [ ] ALL EXTERNAL SEAMS SHALL BE CONTINUOUS WELD AND GROUND FLUSH. CORNER WELDS SHALL BE GROUND TO R X.XX"
	- [ ] INSTALL HARDWARE PER MANUFACTURING INSTRUCTIONS. PROTECT ALL HARDWARE AND THREADS AS NEEDED PRIOR TO FINISH SUCH THAT INTENDED HARDWARE FUNCTION IS NOT IMPAIRED. FLOATING HARDWARE SHALL RETAIN FULL RANGE OF MOTION AFTER FINISH. ALL THREADS SHALL PASS GO/NO GO GAUGE AFTER FINISH.
	- [ ] PRESS FIT PER MANUFACTURER’S SPECIFICATIONS.
- [ ] Mating/critical points have dimensions double check
- [ ] Bends are dimensioned to theoretical sharp with appropriate box note
- [ ] Weld callouts per [Welding](Welding.md) BKMs (AWS A2.4)