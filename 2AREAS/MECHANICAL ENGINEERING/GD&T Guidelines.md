---
created: 2024-02-15
modified: 2024-02-15
tags:
  - SOP
---
## Description 
I want a way to define GD&T features on a drawing such that the function of the part is fulfilled. Right now, that standard does not exist for me, there has likely been research done on this topic, I will just need to find it. This note will be broken up by feature type, since we usually are using them on the same features over and over. 

## Theory of Operation 
Firstly, if you are mating to any OEM components, guidelines about tolerancing of the features should be taken from said components. 

### Bolt patterns
An important concept in GD&T to be aware of when dimensioning and tolerancing bolt patterns are composite positional tolerances. 

[Understanding composite positional tolerances in GD&T | Article | FARO](https://www.faro.com/fr-FR/Resource-Library/Article/understanding-composite-positional-tolerances-in-gd-t)

Composite tolerances are used when we have relatively looser location requirements but tighter orientation tolerances. The full definition of composite tolerances can be found in section 10.5 of the ASME Y14.5-2018 standard. 

A simple example would be a set of holes (pattern) used to affix a name plate. The relative position of the holes is important (tighter tolerance), in order to match the same hole on the plate itself, but the absolute position of the entire pattern on the part may be less critical (looser tolerances) as long as the orientation is good.

The composite tolerance bolt pattern consists of:  
- Pattern-locating tolerance zone framework (PLTZF)
- Feature-relating tolerance zone framework (FRTZF)

**There are 3 main types of composite tolerances** 
All examples are reference of the part shown below:
![Pasted image 20240215162709](../../3RESOURCES/PUBLIC%20ASSETS/Pasted%20image%2020240215162709.png)

#### Composite tolerance with only primary datum in the lower segment

![Pasted image 20240215162113](../../3RESOURCES/PUBLIC%20ASSETS/Pasted%20image%2020240215162113.png)

![Pasted image 20240215161236](../../3RESOURCES/PUBLIC%20ASSETS/Pasted%20image%2020240215161236.png)

The blue zone dots (FRTZF) can translate up-down and left-right and rotate around z within the limits of PLTZF. 

#### Composite tolerance with primary and secondary datums in lower segment

![Pasted image 20240215162525](../../3RESOURCES/PUBLIC%20ASSETS/Pasted%20image%2020240215162525.png)

![Pasted image 20240215162552](../../3RESOURCES/PUBLIC%20ASSETS/Pasted%20image%2020240215162552.png)

The FRTZF can translate up-down and left-right within the limits of PLTZF. 

#### Two single-segmented position tolerancing

![Pasted image 20240216081230](../../3RESOURCES/PUBLIC%20ASSETS/Pasted%20image%2020240216081230.png)

![Pasted image 20240215162807](../../3RESOURCES/PUBLIC%20ASSETS/Pasted%20image%2020240215162807.png)

The blue tolerance zone cylinders can translate left-right within the limits of the yellow tolerance zone cylinders.

### Example
Say you are mounting a spacer ring onto a chamber, we must take into account the following tolerances: 
- Tolerance of locating feature from spacer ring to chamber
- Composite positional tolerance of chamber bolt holes 
- Composite positional tolerance of spacer ring bolt holes
- Tolerance of bolt holes in spacer ring

This will give us a full picture of our allowable tolerances for the locating feature, and positional tolerances for the chamber and spacer ring bolt patters. The threads are fixed and come from manufacturer. 

Strategy is to simulate tolerances with a [Monte-Carlo simulation](https://www.youtube.com/watch?v=HwVBi--mE4M). This will help ensure that we are not just using "min/max" method and defining a statistical limit for our tolerance calculations based on actual manufacturing data. 

See: 
[Normal distribution - Wikipedia](https://en.wikipedia.org/wiki/Normal_distribution)
[Design Decisions to Ensure Quality & Alignment of Threaded Parts (designworldonline.com)](https://www.designworldonline.com/design-decisions-to-ensure-quality-alignment-of-threaded-parts/)

**Tolerance Stackup**
Chamber: 
- Pin location
- Pin Diameter (only important for alignment of spacer ring)
- Bolt pattern relative to pin
- Bolt pattern spacing

Spacer ring
- locating hole location
- Pattern location relative to locating hole
- pattern spacing
- bolt hole clearance 

Goal is to allow perfect alignment of bolt thread major dia with mating threads in chamber. This means that if the bolt is aligned with its mating holes, there must be no intersection of the clearance holes on the spacer ring (usually counterbored bolt pattern).

#### Datum Strategy
See [Datums | McGraw-Hill Education - Access Engineering (accessengineeringlibrary.com)](https://www.accessengineeringlibrary.com/content/book/9781260453782/chapter/chapter4)

See [GD&T in precision engineering: using slots in precision location | Article | FARO](https://www.faro.com/en/Resource-Library/Article/gd-t-in-precision-engineering-using-slots-in-precision-location) as a reference

![Pasted image 20240216105052](../../3RESOURCES/PUBLIC%20ASSETS/Pasted%20image%2020240216105052.png)

**Primary datum**: sealing surface or surface which mates with a part in the next higher assembly. This datum should have a flatness tolerance of 0.003" if it is a sealing surface, and 0.005" if non-sealing. See [FEL-PRO Head gasket sealing flatness recommendations](https://www.felpro.com/technical/tecblogs/surface-finish.html) Keep the tolerance regardless of feature size until suppliers complain, then re-evaluate. 

**Secondary Datum**: The locating hole should be the secondary datum. This is because this is the hole that is aligned to the location features in the mating part, it is recommended to use a hole-slot alignment for most parts to allow for easier manufacturing and assembly. 

**Tertiary Datum**: This should be the final locating feature, usually a slotted hole for the remaining locating pin. 






