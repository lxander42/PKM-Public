---
aliases: []
created: 2023-11-03
modified: 2024-08-30
tags: [seed, system]
---

#seed 

# Description

Eventually I want to develop a mechanical design language which is human-readable but helps mechanical designers design and document mechanical parts in much the same way that a software engineer would develop software. 

The units of mechanical design (see [Atomic Mechanical Design](../Atomic%20Mechanical%20Design.md)) would be formatted in file formats similar to [JSON](../../CODING/JSON.md). 

This would help enforce standardized design rules so that mechanical systems would be more robust, interchangeable, and sustainable. 

# Examples

These [JSON](../../CODING/JSON.md) schemas are not set in stone yet, but just ideas for how this might play out

## Atom

```JSON
{
  "atom": {
    "id": "Atom001",
    "name": "Surface Finish",
    "description": "Characteristics of a part's surface",
    "attributes": {
      "type": "Mechanical",
      "properties": [
        {
          "name": "Roughness",
          "unit": "micrometers",
          "valueRange": "0.1 to 3.2"
        },
        {
          "name": "Hardness",
          "unit": "HV",
          "valueRange": "100 to 700"
        }
      ]
    },
    "applicableStandards": [
      "ISO 4287",
      "ASME B46.1"
    ],
    "notes": "Surface finish affects friction, wear, and appearance of the part."
  }
}

```

## Molecule
