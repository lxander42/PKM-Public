---
created: 2024-02-16
modified: 2024-02-16
tags:
  - SOP
---
## Description 
Notes on cable routing in NX.

## Procedure
- Electrical team will give you a plmxml file in the discussion column, talk to them if you don't have it. 
	- This translates information between Zuken E3 and NX
- Find the component on the [Interconnect diagram](../../../3RESOURCES/PARTS/224-A19277-710.md) for reference to figure out what assemblies you need to load
- Work on the assembly level in the configuration that will require the longest cable length
- In NX, activate the Cable PN, go to application > Electrical 
- Select Harness and Cabling under the toolbox dropdown on the ribbon 
- Go to component navigator in the side ribbon, right click the electrical component navigator and import>update the plmxml file
- Under more>qualify part, under fitting, go to new and make a port connecting to where all your connectors go.
- Place part and place your connector to the port you just made, if it is not qualified with a part, open a CEG ticket to qualify it. 
	- double arrow is where your wire connects, the other arrow is where it mates to the assembly. 
- Go into the electrical component navigator and assign the part to the part you just placed. 
	- Once you assign it there will be a checkmark next to it.
	- ![Pasted image 20240216134009](ATTACHMENTS/Pasted%20image%2020240216134009.png)
- Do this for any remaining connectors
- Add a spline on the two connector ends that are the furthes apart
	- ![Pasted image 20240216134435](ATTACHMENTS/Pasted%20image%2020240216134435.png)
- To split the cable select the spline and subdivide segments, adjust the selector for where you want to split the segments. 
- Make sure everything is in the routing reference set on the assembly. 
- Right click and auto do auto routing on the component level. 
- To send back to camelot, delete all the constraints that are not labeled "routing control point" on all your routing components.
- Right click on component area>export all, naming convention is CablePN_Rev_MCAD_EXPORT

**For Backshells**
- before routing, backshell info is not in the xml file 
- find out backshell and go to place part 
- As mechanical engineer, we get to dictate if it is right angle or straight. 
- Instead of routing to the connector, you now route to the backshell. 
- After making the spline, Display connected ports, and create another spline, connect it from the double arrow port to where it connects to the backshell, this is because E3 does not see the backshell. 