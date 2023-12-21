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

[]{#TestFeatureTypevocabulary}

# **Concept scheme:** Test Feature Type vocabulary

Vocabulary last modified:  2023-12-20

subtitle: 
  Categories to specify the broad context that a sample is intended to represent.

Namespace: 
[`https://test.org/vocabulary/sampledfeature/1.0/testfeaturevocabulary`](https://test.org/vocabulary/sampledfeature/1.0/testfeaturevocabulary)

**History**

* derived from isamples sampled feature type vocabulasry for testing 

- [Any sampled feature](#anysampledfeature)
    - [Anthropogenic environment](#anthropogenicenvironment)
        - [Active human occupation site](#activehumanoccupationsite)
            - [Experiment setting](#experimentsetting)
            - [Laboratory or curatorial environment](#laboratorycuratorialenvironment)
        - [Site of past human activities](#pasthumanoccupationsite)
    - [Biological entity](#biologicalentity)
    - [Earth environment](#earthenvironment)
        - [Atmosphere](#atmosphere)
        - [Earth interior](#earthinterior)
        - [Earth surface](#earthsurface)
            - [Lake river or stream bottom](#lakeriverstreambottom)
            - [Marine water body bottom](#marinewaterbodybottom)
            - [Subaerial surface environment](#subaerialsurfaceenvironment)
        - [Glacier environment](#glacierenvironment)
        - [Subsurface fluid reservoir](#subsurfacefluidreservoir)
        - [Water body](#waterbody)
            - [Marine environment](#marinewaterbody)
            - [Terrestrial water body](#terrestrialwaterbody)
    - [Extraterrestrial environment](#extraterrestrialenvironment)

**Concepts**

[]{#anysampledfeature}

##  Any sampled feature


- Any thing that can be sampled. Top concept in sampled feature type
vocabulary.
- Concept URI token: anysampledfeature


[]{#anthropogenicenvironment}

###  Anthropogenic environment


- Child of:
 [`anysampledfeature`](#anysampledfeature)

- Sampled feature is produced by or related to human activity past or
present.
- Concept URI token: anthropogenicenvironment


[]{#activehumanoccupationsite}

####  Active human occupation site


- Child of:
 [`anthropogenicenvironment`](#anthropogenicenvironment)

- Specimen samples materials or objects produced by current or ongoing
human activity
- Concept URI token: activehumanoccupationsite


[]{#experimentsetting}

#####  Experiment setting


- Child of:
 [`activehumanoccupationsite`](#activehumanoccupationsite)

- Sampled feature is the experimental set up that produced the sample.
- Concept URI token: experimentsetting


[]{#laboratorycuratorialenvironment}

#####  Laboratory or curatorial environment


- Child of:
 [`activehumanoccupationsite`](#activehumanoccupationsite)

- Specimen samples environment in a laboratory; e.g. lab blank
measurements.
- Concept URI token: laboratorycuratorialenvironment


[]{#pasthumanoccupationsite}

####  Site of past human activities


- Child of:
 [`anthropogenicenvironment`](#anthropogenicenvironment)

- specimen samples a place where humans have been and left evidence of
their activity. Includes prehistoric and paleo hominid sites
- Concept URI token: pasthumanoccupationsite


[]{#biologicalentity}

###  Biological entity


- Child of:
 [`anysampledfeature`](#anysampledfeature)

- Sampled feature is an organism. Use for samples that represent some
species of organism as the proximate sampled feature for which the
focus is not the environment that the organism inhabits.
- Concept URI token: biologicalentity


[]{#earthenvironment}

###  Earth environment


- Child of:
 [`anysampledfeature`](#anysampledfeature)

- specimen samples the natural Earth environment

- See Also:
* [<http://purl.bioontology.org/ontology/MESH/D004777>](http://purl.bioontology.org/ontology/MESH/D004777)
* [<http://semanticscience.org/resource/SIO_000955>](http://semanticscience.org/resource/SIO_000955)
- Concept URI token: earthenvironment


[]{#atmosphere}

####  Atmosphere


- Child of:
 [`earthenvironment`](#earthenvironment)

- specimen samples the Earth's atmosphere

- See Also:
* [<http://purl.obolibrary.org/obo/ENVO_01000267>](http://purl.obolibrary.org/obo/ENVO_01000267)
* [<http://purl.obolibrary.org/obo/RBO_00000018>](http://purl.obolibrary.org/obo/RBO_00000018)
- Concept URI token: atmosphere


[]{#earthinterior}

####  Earth interior


- Child of:
 [`earthenvironment`](#earthenvironment)

- Specimen samples solid material within the earth
- Concept URI token: earthinterior


[]{#earthsurface}

####  Earth surface


- Child of:
 [`earthenvironment`](#earthenvironment)

- Specimen samples the interface between solid earth and hydrosphere
or atmosphere. Includes samples representing things collected on the
surface, or in the uppermost part of the material below the surface.
Not including recently deposited sediment that has not been modified
by interaction with the surface environment.
- Concept URI token: earthsurface


[]{#lakeriverstreambottom}

#####  Lake river or stream bottom


- Child of:
 [`earthsurface`](#earthsurface)

- Specimen samples the solid Earth interface with a lake or flowing
water body
- Concept URI token: lakeriverstreambottom


[]{#marinewaterbodybottom}

#####  Marine water body bottom


- Child of:
 [`earthsurface`](#earthsurface)

- Specimen samples the solid Earth interface with marine or brackish
water body. Includes benthic boundary layer:  the bottom layer of
water and the uppermost layer of sediment directly influenced by the
overlying water
- Concept URI token: marinewaterbodybottom


[]{#subaerialsurfaceenvironment}

#####  Subaerial surface environment


- Child of:
 [`earthsurface`](#earthsurface)

- Specimen samples the interface between solid Earth and atmosphere.
Sample is collected on the surface, or immediately below surface (zone
of bioturbation). Include soil and recently deposited subaerial
sediment at the surface.
- Concept URI token: subaerialsurfaceenvironment


[]{#glacierenvironment}

####  Glacier environment


- Child of:
 [`earthenvironment`](#earthenvironment)

- Sample of ice, water, or other thing from a glacier, ice sheet, ice
shelf, iceberg. Does not include various environments adjacent to
glacier.
- Concept URI token: glacierenvironment


[]{#subsurfacefluidreservoir}

####  Subsurface fluid reservoir


- Child of:
 [`earthenvironment`](#earthenvironment)

- Specimen samples fluid that resides in fractures or intergranular
porosity in the solid earth.
- Concept URI token: subsurfacefluidreservoir


[]{#waterbody}

####  Water body


- Child of:
 [`earthenvironment`](#earthenvironment)

- Specimen samples the hydrosphere
- Concept URI token: waterbody


[]{#marinewaterbody}

#####  Marine environment


- Child of:
 [`waterbody`](#waterbody)

- specimen samples marine hydrosphere

- See Also:
* [<http://purl.obolibrary.org/obo/ENVO_01000686>](http://purl.obolibrary.org/obo/ENVO_01000686)
- Concept URI token: marinewaterbody


[]{#terrestrialwaterbody}

#####  Terrestrial water body


- Child of:
 [`waterbody`](#waterbody)

- Specimen samples terrestrial hydrosphere-- lake, other standing
water, or a flowing water body (river, stream..) Include saline water
in terrestrial evaporite environments.
- Concept URI token: terrestrialwaterbody


[]{#extraterrestrialenvironment}

###  Extraterrestrial environment


- Child of:
 [`anysampledfeature`](#anysampledfeature)

- specimen samples environment outside of solid earth, hydrosphere, or
atmosphere.
- Concept URI token: extraterrestrialenvironment



