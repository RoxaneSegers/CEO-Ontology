# CEO: The Circumstantial Event Ontology.  

This repository contains the Circumstantial Event Ontology (CEO). 
This is version 1.0 (stable).

## Resource Description
The Circumstantial Event Ontology (CEO.owl), is a manually constructed resource which formalizes 
the pre-, during-, and post-situations of events and the roles of the entities affected by an event. 
Further, it allows to infer *circumstantial relations* between events in natural language text. A circumstantial relation is defined here as an implicit and weakly causal relation.
For instance, events pertaining to class A and event B can happen independently, but if they appear in context, a circumstantial relation is inferred based on shared properties in the class assertions.

Example: "Three months ago she *arsoned* her ex-husband stables. She was *arrested* soon after; the historical buildings are currently being *restored* by an expert builder." 
For a human reader, it is clear that 'arson', 'arrest' and 'restoration' are causally related in this context. However, there are no clues in these sentences that explicitly connect them. 
Our system, based on the CEO ontology, infers exactly these implicit relations. It does not define explicitly that e.g. 'arson' causes 'restoration' as the relation is plausible but certainly not necessary; therefore the ontology is designed to infer it.
In the case of ceo:Arson we defined e.g. that after some arson there is damage. And before some restoration takes place, there must be some damage. Hence, we connect the events in this sentence with a so called circumstantial relation. We have created large sets of class assertions in order to connect events
based on shared and implicit semantics. As such, we can not only connect the events, but also explain *why* something happened. In the case of the arson and restoration example, we know that the stables were restored *because* they were damaged due to some arson.


### Prerequisites
CEO is fully mapped to [SUMO](http://www.adampease.org/OP/) on class level and to [FrameNet](https://framenet.icsi.berkeley.edu/fndrupal/) on class and role level. 
As input format, CEO can work on unannotated and unprocessed data. In this case, the model will infer circumstantial relations only based on surface forms of the event mentions. 
To get you started, we provided a vocabulary with event surface forms mapped to CEO classes.
However, in order to employ the full inference power of the model, we advise to use processed documents with FrameNet based Semantic Role Labeling. CEO will run on top of this output.
 

### Contents CEO

* 223 event classes
* 121 properties
* 79 roles
* 456 situation rule assertions
* skos mappings to SUMO (195) and FrameNet Frames (265) and Frame Elements (263)

## Repository Description

* `CEO-1.owl` This is ESO version 1 (stable)
* `CEO-HumanReadable.pdf` This file contains a transcription of all CEO classes and provides examples of the instantiation of the assertions.
* `CEO-Vocabulary` This folder contains the manual mappings between event mentions extracted from the ECB+/CEO corpus and the CEO ontology. It includes a readme. Note that a new file is in the making with proper lemmatization and manual mappings to Princeton WordNet.
* `EvaluationCorpus` This folder contains the ECB+/CEO corpus, annotated with circumstantial relations between event mentions and instances. It includes the CAT annotation task and statistics on the corpus annotation.
* `CEO-Poster.pdf` This file presents a schematic overview of the ontology metamodel.
* `CEO-LatestPaperOnCEO.pdf` This file contains the latest publication on the CEO ontology. (published in Proceedings of [LREC](http://lrec2018.lrec-conf.org/en/) 2018.


## Resource Reference
If you use this resource, please cite:
Segers, R., T.Caselli, P. Vossen (2018). “The Circumstantial Event Ontology (CEO) and ECB+/CEO; an Ontology and Corpus for Implicit Causal Relations between Events”. 
In: Proceedings of the 11th edition of the Language Resources and Evaluation Conference [LREC](http://lrec2018.lrec-conf.org/en/), Miyazaki, Japan, May 7-12, 2018.


## Contact

roxane.segers (the email symbol) gmail.com


## Acknowledgements:
This work was co-funded by:
- Netherlands Organization for Scientific Research (NWO) via the Spinoza grant, 
awarded to [Piek Vossen](http://vossen.info/) in the project [Understanding Language by Machines](http://www.understandinglanguagebymachines.org/)

## Provenance of this repository
This repository is an adapted clone of this original [repository](https://github.com/newsreader/eso-and-ceo).
Cloned an adapted in April 2018.

## License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">The Circumstantial Event Ontology(CEO)</span> by <span xmlns:cc="http://creativecommons.org/ns#" property="cc:attributionName">Roxane Segers</span> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/RoxaneSegers/CEO-Ontology" rel="dct:source">https://github.com/RoxaneSegers/CEO-Ontology</a>.


