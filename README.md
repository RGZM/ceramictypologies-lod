# Ceramic Typologies Ontology

## Ontology

The ontology is based on `OWL`, `RDFS`, `PROV-O`, `CIDOC CRM`, includes `AMT`, `FOAF`, `GeoSPARQL`, and extends `SKOS` properties and classes.

## Classes

Relevant classes from the `LADO Ontology` are:

-   lado:Tradition (skos:Concept, crm:E55_Type)
-   lado:GenericPotform (skos:Concept, crm:E55_Type)
-   lado:Potform (skos:Concept, crm:E55_Type)
-   lado:Shape_Collection (skos:Collection, crm:E1_CRM_Entity)

![](https://raw.githubusercontent.com/RGZM/ceramictypologies-lod/main/classes.PNG?token=AB6C2Q6DFV2NSCJ52M4JFSTACQXLW)

## Properties

Relevant properties are derived from `SKOS` properties:

-   lado:exactMatch (derived from skos:exactMatch) ~ Potform-\[skos:exactMatch]->Potform
-   lado:hasMemberItem (derived from skos:member) ~ Service_Collection-\[skos:member]->Potform
-   lado:hasBroaderItem (derived from skos:broader) ~ Potform-\[skos:broader]->Tradition ||  Potform-\[skos:broader]->GenericPotform
-   lado:hasNarrowerItem (derived from skos:narrower) ~ Tradition-\[skos:narrower]->Potform ||  GenericPotform-\[skos:narrower]->Potform
-   lado:hasSameRim (derived from skos:related) ~ Potform-\[skos:related]->Potform
-   lado:hasSameWall (derived from skos:related) ~ Potform-\[skos:related]->Potform
-   lado:hasSameFootring (derived from skos:related) ~ Potform-\[skos:related]->Potform
-   lado:hasSameGroove (derived from skos:related) ~ Potform-\[skos:related]->Potform
-   lado:hasSameRoulette (derived from skos:related) ~ Potform-\[skos:related]->Potform
-   lado:hasSameFlute (derived from skos:related) ~ Potform-\[skos:related]->Potform

![](https://raw.githubusercontent.com/RGZM/ceramictypologies-lod/main/objectproperties.PNG?token=AB6C2Q6SDS6JPUF3ZNFCN7LACQXL2)

## Credits

CC BY 4.0 - Florian Thiery M.Sc., Dr. Allard Mees FSA
