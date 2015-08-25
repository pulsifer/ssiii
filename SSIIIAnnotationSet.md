#A draft set of required, recommended, and optional metadata elements to be used to annotate SSIII ontologies

# Dublin Core Reference Documents #

[Dublin Core Metadata Initiative Home Page](http://dublincore.org/)

[Dublin Core RDF (DC-RDF) document](http://dublincore.org/2010/10/11/dcelements.rdf#)

# RDF/OWL Reference Documents #

[RDF Schema](http://www.w3.org/TR/rdf-schema/)

[OWL](http://www.w3.org/TR/owl-ref/)

# SSIII Annotation Element Set #

These elements are required, recommended, or optional for ontologies developed by the SSIII community.

## Required ##

### Ontology Level ###

[rdfs:comment](http://www.w3.org/TR/rdf-schema/#ch_comment):  An account of the resource. An instance of rdf:Property that may be used to provide a human-readable description of a resource.

[rdfs:label](http://www.w3.org/TR/rdf-schema/#ch_label): an instance of rdf:Property that may be used to provide a human-readable version of a resource's name.

[dc:creator](http://dublincore.org/2010/10/11/dcelements.rdf#creator): An entity primarily responsible for making the resource.  In our case the creator will be the "SSIII Project Team."

[dc:rights](http://dublincore.org/2010/10/11/dcelements.rdf#rights): Information about rights held in and over the resource.  We agreed to use the CC0 version of the PIC badge, translating the rights information from RDF to OWL and the html to text.

[dc:source](http://dublincore.org/2010/10/11/dcelements.rdf#source): The described resource may be derived from the related resource in whole or in part. Recommended best practice is to identify the related resource by means of a string conforming to a formal identification system. (Class Level).

[dc:date](http://dublincore.org/2010/10/11/dcelements.rdf#date): A point or period of time associated with an event in the lifecycle of the resource. `(Note: this information could be inferred using owl:versionInfo contstructs) `

[dc:language](http://dublincore.org/2010/10/11/dcelements.rdf#language): A language of the resource. (Ontology level)

[dc:title](http://dublincore.org/2010/10/11/dcelements.rdf#title): A name given to the resource.

[dc:subject](http://dublincore.org/2010/10/11/dcelements.rdf#subject): The topic of the resource. We will use the [NCAR version of GCMD keywords](http://dataportal.ucar.edu/schemas/gcmd.owl) for now.

[dc:publisher](http://dublincore.org/2010/10/11/dcelements.rdf#publisher): An entity responsible for making the resource available.   We will use NSIDC for everything that isn't a pure WMO ontology (at least for the moment).


#### Ontology Versioning ####

For each version of an ontology, a versioning narrative will be added as an rdfs:comment in the form of a change log.  Detailed versioning information will be captured at the ontology level using owl versioning constructs.

A major and minor version will be established.

Minor version: Significant collection of individual changes deemed important enough to replace the current release. For example, adding new information (classes, properties), significant changes to annotation, or other useful features.

Major version: Major changes to the entire ontology, changes that have an impact on the inference model.
We can establish a version URI/IRI to specific version tag in Subversion.  Create a version PURL that will point to the SVN repository to a particular tag.  Come up with a current version tag for current distribution but does not include latest, work version.

[owl:versionInfo](http://www.w3.org/TR/owl-ref/#Annotations) :

owl:priorVersion

owl:deprecated

### Class, Property, Individual Level ###

[Source](http://dublincore.org/2010/10/11/dcelements.rdf#source): The described resource may be derived from the related resource in whole or in part. Recommended best practice is to identify the related resource by means of a string conforming to a formal identification system. (Class Level)

For example

reference form http://www.aari.nw.ru/gdsidb/docs/wmo/nomenclature/WMO_Nomenclature_draft_version1-0.pdf #Section $

## Recommended ##

[Coverage](http://dublincore.org/2010/10/11/dcelements.rdf#coverage): The spatial or temporal topic of the resource, the spatial applicability of the resource, or the jurisdiction under which the resource is relevant.
` To be discussed.  Selection from items in Optional set `

## Optional ##

[Desrcription](http://dublincore.org/2010/10/11/dcelements.rdf#description): An account of the resource.

[Contributor](http://dublincore.org/2010/10/11/dcelements.rdf#contributor): An entity responsible for making contributions to the resource.

[Type](http://dublincore.org/2010/10/11/dcelements.rdf#type): The nature or genre of the resource.

[Format](http://dublincore.org/2010/10/11/dcelements.rdf#format): The file format, physical medium, or dimensions of the resource.

[Identifier](http://dublincore.org/2010/10/11/dcelements.rdf#identifier):  An unambiguous reference to the resource within a given context.

[Relation](http://dublincore.org/2010/10/11/dcelements.rdf#relation): A related resource.


Check reference:  http://obi-ontology.org/page/MIREOT