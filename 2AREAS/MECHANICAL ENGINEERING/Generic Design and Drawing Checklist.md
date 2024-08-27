---
created: 2023-10-27
modified: 2023-10-27
tags:
  - checklist
---

## Description 
This is intended as a general checklist for checking mechanical part drawings, more specific checklists should be made for specific use cases and companies. Checklist items are listed in subjective order of importance. 

This is a combination of all part types, remove requirements as needed for different part types.

## Design

- [ ] Fit check in next higher assembly with no interferences, fully constrained.
- [ ] Dimensions match tolerance calculations
- [ ] O-ring grooves are sized appropriately
- [ ] O-ring grooves have inner surface relief to avoid rubbing
- [ ] O-ring grooves have tool entry features and locations identified
- [ ] Sealing surfaces have appropriate surface finish/coating
- [ ] Standard tubing sizes used, however, tubing diameter should match welded component diameter
	- .125" - .028" wall 
	- .25" - .035" wall\
	- .375" - .035" wall
	- .5" - .049" wall
- [ ] Glands of opposing parts to be assembled in CAD with a distance of .02" to fit VCR gasket. Assess distance if using other gasketing material
- [ ] Minimum .25" distance between orbitally welded components
- [ ] Locating features are present and look correct in CAD.
- [ ] Mounting hardware to next higher assembly and surrounding components is present and appropriately dimensioned
- [ ] Standard PNs used for OTS parts
- [ ] MBR of 8x diameter when possible. If not, assess actual MBR.
- [ ] Label is modeled with dummy text in CAD
- [ ] Poke yoke features used where available/applicable (i.e. alternating male/female ends)
- [ ] Features to dodge existing hardware are present and properly dimensioned
- [ ] Embedded hardware uses standard parts where applicable
- [ ] Correct size and length for inserts (Helicoils, Pems, etc.), both for assembly hole and the intended hardware
- [ ] Part is fully released and PLM system matches CAD

## Drawing

- [ ] Title/Description match PLM system
- [ ] Tolerances adhere to [Block Tolerance Standards](../../5INBOX/Block%20Tolerance%20Standards.md)
	- ![Block Tolerance Standards](Block%20Tolerance%20Standards.md#^cc7d53)
- [ ] Non-critical features are defined with +/- or block tolerances
- [ ] Critical features are defined per [GD&T Guidelines](../../PKM-Public/2AREAS/MECHANICAL%20ENGINEERING/GD&T%20Guidelines.md) which convey design intent
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
