# Serialized Regulation Documents

This page showcases an extract from the Spanish Urban Planning Regulations. These are sieralized in a HTML and JSON-LD representation.

## HTML Example

```
<!DOCTYPE html>
<html>
    <head>
        <meta content="text/html; charset=utf-8" http-equiv="Content-Type"/>
        <link href="https://www.dcom.org.uk/dcom.css" rel="stylesheet" type="text/css"/>
        <link href="https://www.dcom.org.uk/rase.css" rel="stylesheet" type="text/css"/>
        <title>
            Urban regulations
        </title>
        <meta content="en-gb" name="dcterms:language"/>
        <meta content="2005" name="ckterms:version"/>
        <meta content="2005-07-13" name="dcterms:dateCreated"/>
        <meta content="ES" name="dcterms:coverage.spatial"/>
        <meta content="ANY" name="dcterms:subject"/>
    </head>
    <body>
            <div data-rasetype="RequirementSection" id="1">
                <span id="1">
                <span id="1">
                    The
                  </span>
                    <span data-raseproperty=":type == :Parcel" data-rasetype="Application" id="2">
                        parcels
                    </span>
                    <span data-raseproperty=":HasUZCode == 19" data-rasetype="Application" id="3">with regulation 19</span>
                    <span id="4">  must adapt to the following conditions:
                        a) The
                        </span>
                        <span data-raseproperty=":RoadEdges forall =>(:EdgeLength >=12)" data-rasetype="Requirement" id="5">
                            new parcels must at least allow the possibility of building with a 12 meter front facing the vial
                        </span>
                    </span>
                <span data-rasetype="RequirementSection" id="6">
                    <span data-raseproperty=':ParcelRegistrationDate &lt;= "24/1/90"' data-rasetype="Application" id="1">
                        The estates that are registered in the Land Registry prior to the final approval of the General Planning Plan (24/1/90) may be built on provided that,
                    </span>
                    <span data-raseproperty=":RoadEdges forall =>(:EdgeLength >=10)" data-rasetype="Requirement" id="2">
                        due to the proposed layout and size, they allow the possibility to build with a 10 meter facade facing the vial.
                    </span>
                </span>
                <span id="7">
                    <span id="1">
                        <span id="1">
                            b) The
                            <span data-raseproperty=":BuildingDepth == :PlotDepth" data-rasetype="Requirement" id="1">
                                building will exhaust the totality of the preset building depth
                            </span>
                            .
                            <span id="2">
                                c)
                            </span>
                        </span>
                    </span>
                    <span data-rasetype="RequirementSection" id="2">
                        <span data-raseproperty=":RezoningResultsInBuildingDividedBetweenDividers  == true " data-rasetype="Application" id="1">
                             When the rezoning results in a building divided between what could be considered dividers
                        </span>
                        <span data-raseproperty=":LimitsOfDividingParcelsArePerpendicularToFacade == true " data-rasetype="Requirement" id="2">
                               , the limits of the dividing parcels of the building will be perpendicular to its facade
                        </span>
                        .
                    </span>
                </span>
            </div>
    </body>
</html>

```

## JSON-LD Example

```javascript
---
'@base': https://regulations.accordproject.eu/
'@context':
- https://w3id.org/lbd/aec3po/aec3po.jsonld
- terms: https://identifier.buildingsmart.org/uri/accord/ACCORD-1.0/
  functions: https://functions.accordproject.eu/
$type:
- Document
subject: ANY
coverage: ES
title: Urban regulations
issued: 2005-07-13
identifier: Urban_regulations
$id: ES/Urban_regulations
hasPart:
- $id: ES/Urban_regulations/1
  identifier: "1"
  $type:
  - DocumentSubdivision
  - RequirementStatement
  hasPart:
  - $type:
    - Statement
    $id: ES/Urban_regulations/1.1
    identifier: "1.1"
    hasInlinePart:
    - $id: ES/Urban_regulations/1.1.1
      identifier: 1.1.1
      asText: The
      $type:
      - Statement
    - asText: parcels
      $id: ES/Urban_regulations/1.1.2
      identifier: 1.1.2
      isOperationalizedBy:
        $id: ES/Urban_regulations/1.1.2_method
        identifier: 1.1.2_method
        hasBSDDTarget:
          $id: terms:type
          $type:
          - $id
        hasComparator: CheckMethodComparator-eq
        hasBSDDValue:
          $id: terms:Parcel
          $type:
          - $id
        $type:
        - CategoryCheckMethod
      $type:
      - CheckStatement
      - ApplicationStatement
    - asText: with regulation 19
      $id: ES/Urban_regulations/1.1.3
      identifier: 1.1.3
      isOperationalizedBy:
        $id: ES/Urban_regulations/1.1.3_method
        identifier: 1.1.3_method
        hasBSDDTarget:
          $id: terms:HasUZCode
          $type:
          - $id
        hasComparator: CheckMethodComparator-eq
        $type:
        - NumericalCheckMethod
        hasValue: "19"
      $type:
      - CheckStatement
      - ApplicationStatement
    - $id: ES/Urban_regulations/1.1.4
      identifier: 1.1.4
      asText: |-
        must adapt to the following conditions:
                                a) The
      $type:
      - Statement
    - asText: new parcels must at least allow the possibility of building with a 12 meter front facing the vial
      $id: ES/Urban_regulations/1.1.5
      identifier: 1.1.5
      isOperationalizedBy:
        $id: ES/Urban_regulations/1.1.5_method
        identifier: 1.1.5_method
        hasBSDDTarget:
          $id: terms:RoadEdges
          $type:
          - $id
        $type:
        - CompositeCheckMethod
        hasNestedValue:
        - $id: ES/Urban_regulations/1.1.5_method.2
          identifier: 1.1.5_method.2
          hasBSDDTarget:
            $id: terms:EdgeLength
            $type:
            - $id
          hasComparator: CheckMethodComparator-ge
          $type:
          - NumericalCheckMethod
          hasValue: "12"
        hasOperator: CheckMethodOperator-forall
      $type:
      - CheckStatement
      - RequirementStatement
  - $type:
    - Statement
    - RequirementStatement
    $id: ES/Urban_regulations/1.6
    identifier: "1.6"
    hasInlinePart:
    - asText: "The estates that are registered in the Land Registry prior to the final approval of the General Planning Plan (24/1/90) may be built on provided that,"
      $id: ES/Urban_regulations/1.6.1
      identifier: 1.6.1
      isOperationalizedBy:
        $id: ES/Urban_regulations/1.6.1_method
        identifier: 1.6.1_method
        hasBSDDTarget:
          $id: terms:ParcelRegistrationDate
          $type:
          - $id
        hasComparator: CheckMethodComparator-le
        $type:
        - CategoryCheckMethod
        hasValue: 24/1/90
      $type:
      - CheckStatement
      - ApplicationStatement
    - asText: "due to the proposed layout and size, they allow the possibility to build with a 10 meter facade facing the vial."
      $id: ES/Urban_regulations/1.6.2
      identifier: 1.6.2
      isOperationalizedBy:
        $id: ES/Urban_regulations/1.6.2_method
        identifier: 1.6.2_method
        hasBSDDTarget:
          $id: terms:RoadEdges
          $type:
          - $id
        $type:
        - CompositeCheckMethod
        hasNestedValue:
        - $id: ES/Urban_regulations/1.6.2_method.2
          identifier: 1.6.2_method.2
          hasBSDDTarget:
            $id: terms:EdgeLength
            $type:
            - $id
          hasComparator: CheckMethodComparator-ge
          $type:
          - NumericalCheckMethod
          hasValue: "10"
        hasOperator: CheckMethodOperator-forall
      $type:
      - CheckStatement
      - RequirementStatement
  - $type:
    - Statement
    $id: ES/Urban_regulations/1.7
    identifier: "1.7"
    hasInlinePart:
    - $id: ES/Urban_regulations/1.7.1
      identifier: 1.7.1
      asText: b) The
      $type:
      - Statement
    - asText: building will exhaust the totality of the preset building depth
      $id: ES/Urban_regulations/1.7.2
      identifier: 1.7.2
      isOperationalizedBy:
        $id: ES/Urban_regulations/1.7.2_method
        identifier: 1.7.2_method
        hasBSDDTarget:
          $id: terms:BuildingDepth
          $type:
          - $id
        hasComparator: CheckMethodComparator-eq
        hasBSDDValue:
          $id: terms:PlotDepth
          $type:
          - $id
        $type:
        - CategoryCheckMethod
      $type:
      - CheckStatement
      - RequirementStatement
    - $id: ES/Urban_regulations/1.7.3
      identifier: 1.7.3
      asText: .c)
      $type:
      - Statement
    - $id: ES/Urban_regulations/1.7.4
      identifier: 1.7.4
      asText: c)
      $type:
      - Statement
    - $id: ES/Urban_regulations/1.7.2
      identifier: 1.7.2
      hasInlinePart:
      - asText: When the rezoning results in a building divided between what could be considered dividers
        $id: ES/Urban_regulations/1.7.2.1
        identifier: 1.7.2.1
        isOperationalizedBy:
          $id: ES/Urban_regulations/1.7.2.1_method
          identifier: 1.7.2.1_method
          hasBSDDTarget:
            $id: terms:RezoningResultsInBuildingDividedBetweenDividers
            $type:
            - $id
          hasComparator: CheckMethodComparator-eq
          $type:
          - BooleanCheckMethod
          hasValue: "true"
        $type:
        - CheckStatement
        - ApplicationStatement
      - asText: ", the limits of the dividing parcels of the building will be perpendicular to its facade"
        $id: ES/Urban_regulations/1.7.2.2
        identifier: 1.7.2.2
        isOperationalizedBy:
          $id: ES/Urban_regulations/1.7.2.2_method
          identifier: 1.7.2.2_method
          hasBSDDTarget:
            $id: terms:LimitsOfDividingParcelsArePerpendicularToFacade
            $type:
            - $id
          hasComparator: CheckMethodComparator-eq
          $type:
          - BooleanCheckMethod
          hasValue: "true"
        $type:
        - CheckStatement
        - RequirementStatement
      - $id: ES/Urban_regulations/1.7.2.3
        identifier: 1.7.2.3
        asText: "."
        $type:
        - Statement
      $type:
      - CheckStatement
      - RequirementStatement


```
