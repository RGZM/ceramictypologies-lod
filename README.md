# Ceramic Typologies Ontology (CeraTyOnt)

[![CITATION.cff](https://github.com/RGZM/ceramictypologies-lod/actions/workflows/cffvalidator.yml/badge.svg)](https://github.com/RGZM/ceramictypologies-lod/actions/workflows/cffvalidator.yml) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5767082.svg)](https://doi.org/10.5281/zenodo.5767082)

## Ontology

The ontology is based on `OWL`, `RDFS`, `PROV-O`, `CIDOC CRM`, `FOAF` includes `AMT`, and extends `SKOS` as well as `Wikidata`properties and classes.

## Prefixes

-   @PREFIX lado: <http://archaeology.link/ontology#>
-   @PREFIX skos: <http://www.w3.org/2004/02/skos/core#>
-   @PREFIX wdt: <http://www.wikidata.org/prop/direct/>
-   @PREFIX crm: <http://www.cidoc-crm.org/cidoc-crm/>
-   @PREFIX foaf: <http://xmlns.com/foaf/0.1/>

## Classes

Relevant classes from the `LADO Ontology` are:

-   lado:Tradition (skos:Concept, crm:E55_Type)
-   lado:GenericPotform (skos:Concept, crm:E55_Type)
-   lado:Potform (skos:Concept, crm:E55_Type)
-   lado:Service_Collection (skos:Collection, crm:E1_CRM_Entity)
-   lado:Publisher (skos:Concept, crm:E39_Actor, foaf:Person)

## Properties

Relevant properties are derived from `SKOS` properties:

-   lado:exactMatch (derived from skos:exactMatch) ~ Potform-\[lado:exactMatch]->Potform
-   lado:hasMemberItem (derived from skos:member) ~ Service_Collection-\[lado:hasMemberItem]->Potform
-   lado:hasBroaderItem (derived from skos:broader) ~ Potform-\[lado:hasBroaderItem]->Tradition ||  Potform-\[lado:hasBroaderItem]->GenericPotform
-   lado:hasNarrowerItem (derived from skos:narrower) ~ Tradition-\[lado:hasNarrowerItem]->Potform ||  GenericPotform-\[lado:hasNarrowerItem]->Potform
-   lado:hasSameRim (derived from skos:related) ~ Potform-\[lado:hasSameRim]->Potform
-   lado:hasSameWall (derived from skos:related) ~ Potform-\[lado:hasSameWall]->Potform
-   lado:hasSameFootring (derived from skos:related) ~ Potform-\[lado:hasSameFootring]->Potform
-   lado:hasSameGroove (derived from skos:related) ~ Potform-\[lado:hasSameGroove]->Potform
-   lado:hasSameRoulette (derived from skos:related) ~ Potform-\[lado:hasSameRoulette]->Potform
-   lado:hasSameFlute (derived from skos:related) ~ Potform-\[lado:hasSameFlute]->Potform
-   lado:hasPublisher (derived from skos:member) ~ Potform-\[lado:hasPublisher]->Publisher
-   lado:partiallyCoincidentWith (derived from wdt:P1382) ~ Potform-\[lado:partiallyCoincidentWith]->Potform
-   lado:partiallyNotCoincidentWith (inverse of lado:partiallyCoincidentWith) ~ Potform-\[lado:partiallyNotCoincidentWith]->Potform

## Credits

CC BY 4.0 - Florian Thiery M.Sc., Dr. Allard Mees FSA
