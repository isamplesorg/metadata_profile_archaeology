---
comment: | 
  WARNING: This file is generated. Any edits will be lost!
format:
  html:
    ascii: true
    toc: true
    toc-depth: 4
    number-sections: true
    anchor-sections: false
    number-depth: 8
execute:
  echo: false
---

[]{#OpenContextvocabularyextensionformaterialsampleobjecttype}

# **Concept scheme:** Open Context vocabulary extension for material sample object type

no modified date

subtitle: 
  categories for kinds of sample objects specific to archaeological studies
  Vocabulary created based on summary of 'type' values found in OpenContext sample descriptions. This is a bottom-up vocabulary intended as a first draft and demonstration of a material sample type extension for the Open Context community in the iSamples context. Most of the categories are subclasses of msot:Artifact, except for 'bone object' which is a msot:OrganismPart.

Namespace: 
[`https://w3id.org/isample/opencontext/materialsampleobjecttype/oc_msotvocab`](https://w3id.org/isample/opencontext/materialsampleobjecttype/oc_msotvocab)

**History**


- [Artifact](#artifact)
    - [Architectural element](#architecturalelement)
    - [Clothing](#clothing)
    - [Coin](#coin)
    - [Container object](#containerobject)
    - [Domestic item](#domesticitem)
    - [Ornament](#ornament)
    - [Photograph](#photograph)
    - [Pot sherd](#sherd)
    - [Tile](#tile)
    - [Utility item](#utilityitem)
    - [Weapon](#weapon)

- [Organism part](#organismpart)
    - [Bone object](#peiceofbone)

**Concepts**

[]{#artifact}

##  Artifact


- An object made (manufactured, shaped, modified) by a human being, or
precursor hominid. Include a set of pieces belonging originally to a
single object and treated as a single specimen.
- Concept URI token: artifact


[]{#architecturalelement}

###  Architectural element


- Child of:
 [`artifact`](#artifact)

- Artifact that was part of a building.
- Concept URI token: architecturalelement


[]{#clothing}

###  Clothing


- Child of:
 [`artifact`](#artifact)

- Item intended to be worn to cover the (human) body
- Concept URI token: clothing


[]{#coin}

###  Coin


- Child of:
 [`artifact`](#artifact)

- peice of metal issued by some authority and recognized as money.
- Concept URI token: coin


[]{#containerobject}

###  Container object


- Child of:
 [`artifact`](#artifact)

- Item designed to contain some fluid, granular material, or other
items for preservation, transportation or display.
- Concept URI token: containerobject


[]{#domesticitem}

###  Domestic item


- Child of:
 [`artifact`](#artifact)

- item intended for household use.
- Concept URI token: domesticitem


[]{#ornament}

###  Ornament


- Child of:
 [`artifact`](#artifact)

- item intended for decoration.
- Concept URI token: ornament


[]{#photograph}

###  Photograph


- Child of:
 [`artifact`](#artifact)

- image produced by the action of light on a chemically sensitive
surface, preserved on paper, glass or other physical substrate.
- Concept URI token: photograph


[]{#sherd}

###  Pot sherd


- Child of:
 [`artifact`](#artifact)

- fragment of pottery
- Concept URI token: sherd


[]{#tile}

###  Tile


- Child of:
 [`artifact`](#artifact)

- flat or curved piece of fired clay, stone, or concrete used
especially for roofs, floors, or walls and often for ornamental work
- Concept URI token: tile


[]{#utilityitem}

###  Utility item


- Child of:
 [`artifact`](#artifact)

- Item intended for use in manufacture, construction, agriculture or
other work activity.
- Concept URI token: utilityitem


[]{#weapon}

###  Weapon


- Child of:
 [`artifact`](#artifact)

- Item for use in combat, hunting, or self defense
- Concept URI token: weapon



[]{#organismpart}

##  Organism part


- Part of an organism, e.g. a tissue sample, plant leaf, flower, bird
feather. Include internal parts not composed of organic material (e.g.
teeth, bone), and hard body parts that are not shed (hoof, horn, tusk,
claw).  Hair is tricky, include here for now.  Does not necessarily
imply existance of parent sample. Not fossilized; generally includes
organism parts native to deposits of Holocene to Recent age.
- Concept URI token: organismpart


[]{#peiceofbone}

###  Bone object


- Child of:
 [`organismpart`](#organismpart)

- Sample is an individual bone or part of a bone from an animal.
- Concept URI token: peiceofbone



