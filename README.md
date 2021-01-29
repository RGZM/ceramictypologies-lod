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

-   lado:exactMatch (derived from skos:exactMatch) ~ Potform-\[]->Potform
-   lado:hasMemberItem (derived from skos:member) ~ Service_Collection-\[]->Potform
-   lado:hasBroaderItem (derived from skos:broader) ~ Potform-\[]->Tradition ||  Potform-\[]->GenericPotform
-   lado:hasNarrowerItem (derived from skos:narrower) ~ Tradition-\[]->Potform ||  GenericPotform-\[]->Potform
-   lado:hasSameRim (derived from skos:related) ~ Potform-\[]->Potform
-   lado:hasSameWall (derived from skos:related) ~ Potform-\[]->Potform
-   lado:hasSameFootring (derived from skos:related) ~ Potform-\[]->Potform
-   lado:hasSameGroove (derived from skos:related) ~ Potform-\[]->Potform
-   lado:hasSameRoulette (derived from skos:related) ~ Potform-\[]->Potform
-   lado:hasSameFlute (derived from skos:related) ~ Potform-\[]->Potform

![](https://raw.githubusercontent.com/RGZM/ceramictypologies-lod/main/objectproperties.PNG?token=AB6C2Q6SDS6JPUF3ZNFCN7LACQXL2)
