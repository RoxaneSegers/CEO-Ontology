# ESO: The Event and Implied Situation Ontology.  

This repository contains the Circumstantial Event Ontology (CEO). 
This is version 1.0 (stable)

## Resource Description
The Circumstantial Event Ontology (CEO.owl), is a manually constructed resource which formalizes 
the pre-, during-, and post-situations of *events* and the *roles* of the entities affected by an event. 
Further, it allows to infer weakly causal and implicit relations between events in natural language text.


### Prerequisites
CEO is fully mapped to [SUMO](http://www.adampease.org/OP/) on class level and to [FrameNet](https://framenet.icsi.berkeley.edu/fndrupal/) on class and role level. 
As input format, CEO can work on unannotated and unprocessed data. In this case, the model will infer circumstantial relations only based on surface forms of event mentions. 
To get you started, we provide a vocabulary with event surface forms mapped to CEO classes.
However, in order to employ the full inference power of the model, we advise to use processed documents with FrameNet based Semantic Role Labeling. 
 


### Contents CEO




## Repository Description

* `CEO-2.owl` This is ESO version 2 (stable)
* `Documentation.pdf` This is the documentation of the ESO Ontology
* `CEO-HumanReadable.pdf` This file contains a transcription of ESO classes and provides examples of the instantiation of the assertions.
* `CEO-Poster.pdf` This file presents a largely visual and concise overview of the ontology and its application on natural language texts.
* `CEO-Vocabulary` This folder contains the manual mappings between FrameNet, WordNet and ESO. It includes a readme.
* `EvaluationCorpus` This folder contains the MeanTime corpus, annotated with ESO classes and roles.



## Resource Reference
If you use this resource, please cite:



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

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Event and Implied Situation Ontology (ESO)</span> by <span xmlns:cc="http://creativecommons.org/ns#" property="cc:attributionName">Roxane Segers and Marco Rospocher</span> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/RoxaneSegers/ESO-Ontology" rel="dct:source">https://github.com/RoxaneSegers/ESO-Ontology</a>.


