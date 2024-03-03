---
created: 2023-11-03
modified: 2023-11-03
tags:
  - framework
---
#seed 
## Description

I originally had this idea when reading about [atomic design as it pertains to web development](https://bradfrost.com/blog/post/atomic-web-design/). I think there are significant parallels that can be drawn from software development to [Mechanical Design](Mechanical%20Design.md).  Both systems would seek to use [heuristics](heuristics) and [frameworks](frameworks) to guide design decisions.

Below is a graphic that shows how this framework applies to web design. 
![Pasted image 20231103224234](ATTACHMENTS/Pasted%20image%2020231103224234.png)

The way I envisioned it, [Atomic Mechanical Design](.md) is a methodology for creating mechanical systems. There are five distinct levels in the hierarchy: 

1.  [Atoms](https://bradfrost.com/blog/post/atomic-web-design/#atoms) - Part attributes, feature geometry, materials, manufacturing methods, surface finishes, and many more. 
2.  [Molecules](https://bradfrost.com/blog/post/atomic-web-design/#molecules) - The parts themselves, these can include things such as fasteners, O-rings, machined parts, etc. 
3.  [Organisms](https://bradfrost.com/blog/post/atomic-web-design/#organisms) - Assemblies: groups of parts, or molecules, which come together to achieve a certain design intent. 
4.  [Templates](https://bradfrost.com/blog/post/atomic-web-design/#templates) - Arrangements of interchangeable assembles within a [Product Option Architecture](../../3RESOURCES/DEFINITIONS/Product%20Option%20Architecture.md) which can be mixed and matched to obtain a final product [BOM](../../../5INBOX/New/BOM.md). Brad Frost calls these "Templates"
5.  [Product](https://bradfrost.com/blog/post/atomic-web-design/#pages) - A final product after selecting from product options within the [Product Option Architecture](../../3RESOURCES/DEFINITIONS/Product%20Option%20Architecture.md). Specific instances of what Brad Frost refers to as "Templates".

These five levels make up what are called [units of design](units%20of%20design). That is, the things which make up any mechanical design at all levels.

This system cannot always be applied to everything in a given assembly, there may be [OEM](OEM) parts which do not adhere to the [Atomic Mechanical Design](.md) framework. 

## Standardization

Standardization should apply at every level of the hierarchy with distinct criteria for when the rules can be broken. Since there are no syntax rules enforcing mechanical designers to use specific units of design, great care must be taken in enforcing and living by these rules. This is part of the reason for writing out this system because I have been burned many times by the snags that come with non standard parts. 

In the future I would like to explore the idea of developing a [Mechanical Design Language](ATTACHMENTS/Mechanical%20Design%20Language.md) with built in syntax checking so that mechanical designers may develop mechanical parts in much the same way that software developers develop software. 




