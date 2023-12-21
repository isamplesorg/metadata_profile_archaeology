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

[]{#TestSampleTypeVocabulary}

# **Concept scheme:** Test Sample Type Vocabulary

Vocabulary last modified:  2023-12-20

subtitle: 
  Broad categories to specify the kind of physical thing identified as the 'sample'.

Namespace: 
[`https://test.org/vocabulary/specimentype/1.0/testvocabulary`](https://test.org/vocabulary/specimentype/1.0/testvocabulary)

**History**

* test vocabulary derived from iSamples Material Sample type vocabulary

- [Physical specimen](#physicalspecimen)
    - [Any aggregation specimen](#anyaggregation)
        - [Anthropogenic aggregation](#anthropogenicaggregation)
        - [Biome aggregation sample](#biomeaggregation)
            - [Bundle biome aggregation](#bundlebiomeaggregation)
            - [Slurry biome aggregation](#slurrybiomeaggregation)
        - [Aggregation](#genericaggregation)
    - [Any biological specimen](#biologicalspecimen)
        - [Biome aggregation sample](#biomeaggregation)
            - [Bundle biome aggregation](#bundlebiomeaggregation)
            - [Slurry biome aggregation](#slurrybiomeaggregation)
        - [Organism part](#organismpart)
        - [Organism product](#organismproduct)
        - [Whole organism specimen](#wholeorganism)
    - [Fluid in container](#fluidincontainer)
    - [Non biologic solid object](#nonbiologicsolidobject)
        - [Artifact](#artifact)
        - [Fossil](#fossil)
        - [Other solid object](#othersolidobject)
    - [Research product](#researchproduct)
        - [Analytical preparation](#analyticalpreparation)
        - [Experiment product](#experimentalproduct)

**Concepts**

[]{#physicalspecimen}

##  Physical specimen


- A material entity that represents an entity of interest in whole or
in part (http://rs.tdwg.org/dwc/terms/MaterialSample) . Top concept in
material sample type type hierarchy.  Represents any physical specimen
(matrial sample).

- **Alternate labels:**
material sample

- Concept URI token: physicalspecimen


[]{#anyaggregation}

###  Any aggregation specimen


- Child of:
 [`physicalspecimen`](#physicalspecimen)

- Sample consists of a bunch of material fragments, not related to the
same object (e.g. not a bunch of broken pot sherds that might be
reassembled), but taken together representative of the sampled
feature. Examples: loose soil, sediment, crushed rock,  particulate,
bunches of unrelated pot sherd, human production waste, filtrates and
residues. The sample requires some kind of container to keep it
together. Cores of loosely consolidated material are considered 'Solid
material specimen' because the internal parts have spatial
relationships (e.g. upper part, lower part, sedimentary structures).
- Concept URI token: anyaggregation


[]{#anthropogenicaggregation}

####  Anthropogenic aggregation


- Child of:
 [`anyaggregation`](#anyaggregation)

- Aggregation consists of fragments of material produced by human
activity,  not described individually, and generally not all
originating from the same object.  Includes pottery in an excavation
unit that gets an aggregate description, production waste, production
raw-materials, or other residues (broken bits of plaster from a
destroyed wall), synthetic powders.
- Concept URI token: anthropogenicaggregation


[]{#biomeaggregation}

####  Biome aggregation sample


- Child of:
 [`anyaggregation`](#anyaggregation)
 [`biologicalspecimen`](#biologicalspecimen)

- Specimen is an aggregation of whole or fragmentary parts of multiple
organisms, microscopic or megascopic, representative of some site.
- Concept URI token: biomeaggregation


[]{#bundlebiomeaggregation}

#####  Bundle biome aggregation


- Child of:
 [`biomeaggregation`](#biomeaggregation)

- An aggregation of whole organisms representative of some biome
- Concept URI token: bundlebiomeaggregation


[]{#slurrybiomeaggregation}

#####  Slurry biome aggregation


- Child of:
 [`biomeaggregation`](#biomeaggregation)

- specimen consists of mixed organic and inorganic material, including
whole organisms and organism fragments.
- Concept URI token: slurrybiomeaggregation


[]{#genericaggregation}

####  Aggregation


- Child of:
 [`anyaggregation`](#anyaggregation)

- An aggregate specimen that is not biogenic or composed of
anthropogenic material fragments.  Examples: loose soil or sediment
(e.g. in a bag), rock chips, particulate filtrate or precipitate; rock
powders.
- Concept URI token: genericaggregation


[]{#biologicalspecimen}

###  Any biological specimen


- Child of:
 [`physicalspecimen`](#physicalspecimen)

- Specimen for which the sampled feature is one or more living
organisms from a particular biome context, megascopic or microscopic
- Concept URI token: biologicalspecimen


[]{#biomeaggregation}

####  Biome aggregation sample


- Child of:
 [`anyaggregation`](#anyaggregation)
 [`biologicalspecimen`](#biologicalspecimen)

- Specimen is an aggregation of whole or fragmentary parts of multiple
organisms, microscopic or megascopic, representative of some site.
- Concept URI token: biomeaggregation


[]{#bundlebiomeaggregation}

#####  Bundle biome aggregation


- Child of:
 [`biomeaggregation`](#biomeaggregation)

- An aggregation of whole organisms representative of some biome
- Concept URI token: bundlebiomeaggregation


[]{#slurrybiomeaggregation}

#####  Slurry biome aggregation


- Child of:
 [`biomeaggregation`](#biomeaggregation)

- specimen consists of mixed organic and inorganic material, including
whole organisms and organism fragments.
- Concept URI token: slurrybiomeaggregation


[]{#organismpart}

####  Organism part


- Child of:
 [`biologicalspecimen`](#biologicalspecimen)

- Part of an organism, e.g. a tissue sample, plant leaf, flower, bird
feather. Include internal parts not composed of organic material (e.g.
teeth, bone), and hard body parts that are not shed (hoof, horn, tusk,
claw).  Hair is tricky, include here for now.  Does not necessarily
imply existance of parent sample. Not fossilized; generally includes
organism parts native to deposits of Holocene to Recent age.
- Concept URI token: organismpart


[]{#organismproduct}

####  Organism product


- Child of:
 [`biologicalspecimen`](#biologicalspecimen)

- Specimen is a thing produced by some organism, generally not
composed of organic material or including biological tissue, e.g.
Shell, antler, egg shell, coral skeleton (organic tissue not
included), fecal matter, cocoon, web.  Consider internal parts not
composed of organic material (e.g. teeth, bone) and hard body parts
that are not shed (hoof, horn, tusk) to be organism parts.
- Concept URI token: organismproduct


[]{#wholeorganism}

####  Whole organism specimen


- Child of:
 [`biologicalspecimen`](#biologicalspecimen)

- Specimen consists of the bodies of one or more entire organisms of
the same species, from any kingdom. Note that these are also
inherently 'solid object'
- Concept URI token: wholeorganism


[]{#fluidincontainer}

###  Fluid in container


- Child of:
 [`physicalspecimen`](#physicalspecimen)

- Specimen is a container whose contents are liquid, gas, or mixed
dominantly fluid phases that is the actual sample material. Fluid
might include minor solid particles. Container typically human made,
but also includes natural fluid container, e.g. fluid inclusion in a
mineral grain.  Includes colloids, foams, gels, suspensions. The
sample is the fluid substance; fluid samples collected to analyze the
contained biome should be considered 'Biome Aggregation'
- Concept URI token: fluidincontainer


[]{#nonbiologicsolidobject}

###  Non biologic solid object


- Child of:
 [`physicalspecimen`](#physicalspecimen)

- Individual solid object, not formed directly by or part of a living
organism
- Concept URI token: nonbiologicsolidobject


[]{#artifact}

####  Artifact


- Child of:
 [`nonbiologicsolidobject`](#nonbiologicsolidobject)

- An object made (manufactured, shaped, modified) by a human being, or
precursor hominid. Include a set of pieces belonging originally to a
single object and treated as a single specimen.
- Concept URI token: artifact


[]{#fossil}

####  Fossil


- Child of:
 [`nonbiologicsolidobject`](#nonbiologicsolidobject)

- Specimen is the remains of one or more organisms preserved in rock;
includes whole body, body parts (usually bone or shell), and trace
fossils. An organism or organism part becomes a fossil when it has
undergone some fossilization process that generally entails physical
and chemical changes akin to diagenesis in a sedimentary rock.
Includes trace fossils, which are manifestations of biologic activity
preserved in a rock body (typically sedimentary), without included
preserved body parts.
- Concept URI token: fossil


[]{#othersolidobject}

####  Other solid object


- Child of:
 [`nonbiologicsolidobject`](#nonbiologicsolidobject)

- Single piece of material not one of the other types.
- Concept URI token: othersolidobject


[]{#researchproduct}

###  Research product


- Child of:
 [`physicalspecimen`](#physicalspecimen)

- Specimen is a product of some research workflow, e.g. a thin
section, an XRF pellet, a grain mount, SEM stub, synthetic rock or
mineral ...  In general there should be a link to a parent specimen
from which this was derived.  Might be aggregation (e.g. a synthetic
material powder) or a solid object.
- Concept URI token: researchproduct


[]{#analyticalpreparation}

####  Analytical preparation


- Child of:
 [`researchproduct`](#researchproduct)

- Specimen is a product of processing required for some observation
procedure, e.g. thin section, XRF bead, SEM stub, rock powder. If
identified separately, this should have a ‘parent’ link to the
original sample
- Concept URI token: analyticalpreparation


[]{#experimentalproduct}

####  Experiment product


- Child of:
 [`researchproduct`](#researchproduct)

- Specimen is product of an experimental procedure (e.g. synthetic
material)
- Concept URI token: experimentalproduct



