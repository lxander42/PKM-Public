---
created: 2023-11-03
modified: 2023-11-03
tags:
  - quick-note
---
## Manufacturability recommendations 
### Material
- Aluminum: Cheap all purpose material, food safe, good corrosion resistance at low temperatures. Many anodization colors and types available for added durability and corrosion resistance. many kitchen utensils are made out of aluminum. 
- 303 Stainless Steel: Excellent corrosion resistance at all temperatures, much stronger than steel but will cost ~3x in terms of base material cost. Cannot be anodized so color must be applied via painting, which may cost more for appropriate painting. 
	- 9mm 1ft SST rod: $14.95
	- 9mm 1ft aluminum rod: $2.57
- My recommendation: go with aluminum for the first round of production, assess durability and feel, switch to stainless if necessary. 

### Design
#### Body

##### Design recommendations
- Recommend adding radius and eliminating features on legs that would require [5 axis machining](https://www.rapiddirect.com/blog/what-is-5-axis-cnc-machining/) or [forming](https://formlabs.com/blog/sheet-metal-forming/), see before and after below: 
##### Before: 
![[ATTACHMENTS/Pasted image 20231103201036.png]]
**Top down view before:** ![[ATTACHMENTS/Pasted image 20231103201218.png]]
##### After: 
![[ATTACHMENTS/Pasted image 20231103201101.png]]
**Top down view:** ![[ATTACHMENTS/Pasted image 20231103201146.png]]
**Notice how everything is cut straight down in a smooth profile:** ![[ATTACHMENTS/Pasted image 20231103201455.png]]

#### Lid
- We should try to make this out of sheet metal if possible, here are my recommendations. 

##### Corner Treatment
For the chamfered corners shown: 
![[ATTACHMENTS/Pasted image 20231103204337.png]]

I recommend going with 30 degree or 45 degree. What you have right now is 21.8 degrees, this allows them to use the following tools: 
![[ATTACHMENTS/Pasted image 20231103204151.png]]

or 
![[ATTACHMENTS/Pasted image 20231103204217.png]]

**30 degrees**
![[ATTACHMENTS/Pasted image 20231103204827.png]]

**45 degrees**
![[ATTACHMENTS/Pasted image 20231103204855.png]]

##### Bend relief width 
In order to accommodate the corner cutter, I recommend increasing the relief width to 8mm as shown: 

![[ATTACHMENTS/Pasted image 20231103205353.png]]

**Before**
![[ATTACHMENTS/Pasted image 20231103205412.png]]

This will prevent them from having to do some complex manufacturing procedure. 

##### Pivot connection tabs (for welding on shaft collar)
I recommend extending cutter chamfer along tabs, this will allow them to machine it all in one go and bend and weld afterwards. 

**Before**
![[ATTACHMENTS/Pasted image 20231103211902.png]]

**After**
![[ATTACHMENTS/Pasted image 20231103212037.png]]

Side view to show weld prep
![[ATTACHMENTS/Pasted image 20231103212053.png]]

This will allow them to tack weld it in place and finish the weld, it will look similar to this in terms of weld quality when done: 
![[ATTACHMENTS/Pasted image 20231103212327.png]]


#### Shaft sizing
Shaft should be sized for press-fit according to [[engineersedge.com)](https://www.engineersedge.com/general_tolerances.htm|General Mechanical Tolerance Table Charts for Standard Shaft Hole Fits (engineersedge.com)]]

The shaft would be tolerance so as to "stick" to the lid part with a Class V interference fit, and rotate freely through the mating hole on the body with a Class II free fit. This would necessitate a pressing tool to get together. 

![[ATTACHMENTS/Pasted image 20231103212453.png]]

#### All other parts
All other parts look good in terms of manufacturability in my opinion. 