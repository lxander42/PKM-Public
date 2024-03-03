---
created: 2024-01-12
modified: 2024-01-12
tags:
  - standard
---
## Problem
I have too many disparate ways of tracking BOMs and changes for projects with each project having it's own system. I need to standardize this. 

[Link to BOM tracking sheet](https://lamresearch-my.sharepoint.com/:x:/r/personal/logan_alexander_lamresearch_com/Documents/2.%20Areas/Mechanical%20Engineering/Tools/ProjectBOMTracker.xlsx?d=w5f7c21cc415645ff81ff109aa797309f&csf=1&web=1&e=SdaNmG)

## Scope
- Keep track of latest BOMs 
	- In work 
	- Released 
	- Past BOMs and reasons they are no longer used
- Keep track of important PNs (non-assemblies)
- Keep track of BOM changes requested and the affected assemblies, associated PRs, QB issues, reason for change, etc...
- Keep track of reference BOMs and why they are referenced
- Have an instruction tab for how to use the tool with revision notes

## Instructions
0. Enter project information into the appropriate fields to the right
1. When beginning a project, you will likely have some reference assemblies and parts, go ahead and add these to the reference BOMs and important PNs tab.
2. Enter BOM and Part information in the appropriate tabs listed below. 
	1. **In work**: used for BOMs which are currently in work and **should not** be ordered
	2. **Released**: Released BOMs and their purpose within the project
	3. **Past BOMs**: BOMs which have been used in the past and are superseded by other BOMs (either past or currently released), BOMs should not be put in the Past BOMs sheet until the superseding BOM is released to N status. An effort should be Made to OB these BOMs at a regular frequency
	4. **Important PNs**: This tab is only for parts (not assemblies) which have some relevance to the project, their relevance should be explained in the notes section. When they are superseded by another part they should be kept up to date. 
	5. **BOM Changes**: Changes requested by stakeholders of the project, this can be due to PRs, QB issues, general requests, or other circumstances. They should be captured here and rolled out in a timely manner, with BOMs moving from the BOM Changes tab to the In work tab as the changes are starting to be made. 
	6. **Reference BOMs**: Any BOMs which have some relation to the project or are used as reference by the responsible engineer. 
	7. Fields in the tables under each tab (sheet) have been limited in column number to reduce friction when adding parts and assemblies. There is a notes column in each table for any ad-hoc information 
4. For any feature requests or change requests, contact logan.alexander@lamresearch.com