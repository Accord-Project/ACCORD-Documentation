# Serialized Regulation Documents

This page showcases an extract from the Finish Accessibility Regulations. These are sieralized in a HTML and JSON-LD representation.

## HTML Example

```
<!DOCTYPE html>
<html>

<head>
    <meta content="text/html; charset=UTF-8" http-equiv="Content-Type" />
    <link href="https://www.dcom.org.uk/dcom.css" rel="stylesheet" type="text/css" />
    <link href="https://www.dcom.org.uk/rase.css" rel="stylesheet" type="text/css" />
    <title>Government Decree on Accessibility of building</title>
<meta content="en-gb" name="dcterms:language" />
<meta content="4.5.2017/241" name="ckterms:version" />
<meta content="2017-01-01" name="dcterms:dateCreated" />    
<meta content="FI" name="dcterms:coverage.spatial" />
<meta content="ANY" name="dcterms:subject" />
</head>

<body>

    <section id="2" title="Passageway leading to a building">
        
        <div data-raseType="RequirementSection" id="1"><span id="1">There shall be an easily noticeable </span><span id="2"><span data-raseType="Application" data-raseProperty=":isPassageway == true " id="1">passageway </span></span><span id="3">with a width of at least </span><span id="4"><span data-raseType="Requirement" data-raseProperty=":Width > 1.2 " id="1">1,200 millimetres </span></span><span id="5">and a </span><span id="6"><span data-raseType="Requirement" data-raseProperty=":Smooth == true " id="1">smooth, </span></span><span id="7"><span data-raseType="Requirement" data-raseProperty=":Hard == true " id="1">hard </span></span><span id="8">and </span><span id="9"><span data-raseType="Requirement" data-raseProperty=":NonSlip == true " id="1">non-slippery </span></span><span id="10">surface that leads to the </span><span id="11"><span data-raseType="Application" data-raseProperty=":ConnectsWith exists =>(:type == :Building )" id="1">building </span></span><span id="12">from the </span><span id="13"><span data-raseType="Selection" data-raseProperty=":ConnectsWith exists =>(:type == :SiteBoundary )" id="1">boundary of the plot or building site </span></span><span id="14">and from the </span><span id="15"><span data-raseType="Selection" data-raseProperty=":ConnectsWith exists =>(:type == :ServiceArea )" id="1">space and area that serve the use of the building </span></span><span id="16">. </span><span id="17" data-raseType="RequirementSection"><span id="1">The gradient of the passageway located in an </span><span data-raseType="Application" data-raseProperty=":External == true " id="1">outdoor space </span><span id="3">may not </span><span id="4"><span data-raseType="Requirement" data-raseProperty=":Gradient &lt;= 5 :percent" id="1">exceed five per cent </span></span><span id="5" data-raseType="RequirementSection"><span id="6">If there are </span><span id="7"><span data-raseType="Application" data-raseProperty=":Contains exists =>(:type == :Step )" id="1">steps on the passageway </span></span><span id="8">, there shall also be a </span><span id="9"><span data-raseType="Requirement" data-raseProperty=":Contains exists =>(:type == :Ramp )" id="1">ramp </span></span><span id="10">or a </span><span id="11"><span data-raseType="Exception" data-raseProperty=":Contains exists =>(:IsLiftingDevice == true  &amp;&amp; :Permanent == true  &amp;&amp; :SuitableForWheelchair == true  &amp;&amp; :SuitableforWalkingFrame == true    )" id="1">permanently installed device intended for lifting persons that is suitable for a user of a wheelchair and walking frame with wheels. </span></span></span></span></div>

        <div data-raseType="ExceptionSection" id="2">The provisions of this subsection do not apply to a <span data-raseType="Requirement" data-raseProperty=":type == :House " id="2">detached house , semi-detached house or townhouse </span>if providing an <span data-raseType="Requirement" data-raseProperty=":SiteElevationDifferencesMakePassagewayImpossible == true " id="4">accessible passageway would be impossible considering the site and elevation differences </span>. </div>
        <div data-raseType="RequirementSection" id="3"><span id="1"><span id="1">The </span><span id="2"><span data-raseType="Application" data-raseProperty=":type == :Ramp " id="1">ramp </span></span><span id="3">referred to in subsection 1 above shall be easily </span><span id="6"><span data-raseType="Requirement" data-raseProperty=":Noticable == true" id="1">noticeable </span></span><span id="7">and </span><span id="8"><span data-raseType="Requirement" data-raseProperty=":Curvature == 0" id="1">straight </span></span><span id="9">with a </span><span id="10"><span data-raseType="Requirement" data-raseProperty=":Smooth == true " id="1">smooth, </span></span><span id="11"><span data-raseType="Requirement" data-raseProperty=":Hard == true " id="1">hard </span></span><span id="12">and </span><span id="13"><span data-raseType="Requirement" data-raseProperty=":NonSlip == true " id="1">non-slippery </span></span><span id="14">surface, </span><span id="15"><span data-raseType="Requirement" data-raseProperty=":Width >= 0.9 " id="1">width of at least 900 millimetres </span></span><span id="16">and, </span></span><span id="2"><span id="1" data-raseType="RequirementSection"><span id="1">if the ramp is </span><span id="2"><span data-raseType="Application" data-raseProperty=":ConnectedToFixedStructure == false " id="1">not connected to a fixed structure </span></span><span id="3">, </span><span id="4"><span data-raseType="Requirement" data-raseProperty=":Contains exists =>(:type == :ProtectiveEdge  &amp;&amp; :Height > 0.05  )" id="1">a protective edge of at least 50 millimetres in height. </span></span></span></span><span id="3">There shall be a </span><span id="4"><span data-raseType="Requirement" data-raseProperty=":Contains exists =>(:type == :Landing  &amp;&amp; :Orientation == :Horizontal  &amp;&amp; :LandingLength > 1.5   )" id="1">horizontal landing with a length of at least 1,500 millimetres at the lower and upper end of the ramp </span></span><span id="5">. The gradient of the ramp may </span><span id="6"><span data-raseType="Requirement" data-raseProperty=":Gradient &lt;= 5 :percent" id="1">not exceed five per cent </span></span><span id="7">. </span><span id="8" data-raseType="RequirementSection"> <span id="8">However, if the </span><span id="9"><span data-raseType="Application" data-raseProperty=":ElevationChange &lt;= 1 " id="1">elevation difference is no more than 1,000 millimetres </span></span><span id="10">, the ramp may </span><span id="11"><span data-raseType="Requirement" data-raseProperty=":Gradient &lt;= 8 :percent" id="1">not have a gradient of more than eight per cent </span></span><span id="12">. In that case, </span><span id="13"><span data-raseType="Requirement" data-raseProperty=":Contains not exists =>(:type == :Landing ) &amp;&amp; :ElevationChange &lt; 0.5  " id="1">the elevation difference of a continuous ramp may not be more than 500 millimetres </span></span><span id="14">, </span><span id="15"><span data-raseType="Exception" data-raseProperty=":Contains exists =>(:type == :Landing  &amp;&amp; :LandingLength >= 2  )" id="1">after which there shall be a horizontal intermediate landing with a length of at least 2,000 millimetres </span></span><span id="16">. </span></span><span id="9" data-raseType="RequirementSection"><span id="17">However, in an </span><span id="18"><span data-raseType="Application" data-raseProperty=":External == true " id="1">outdoor </span></span><span id="19">area the ramp may have a </span><span id="20"><span data-raseType="Application" data-raseProperty=":Gradient > 5 :percent" id="1">gradient of more than five per cent </span></span><span id="21">only if it can be kept in a condition comparable with that of an indoor ramp. </span><span id="22"><span data-raseType="Requirement" data-raseProperty="" id="1" data-references="Land Use and Building Act.117.d.2">Provisions on railings, handrails and other arrangements intended to prevent falling down and misstepping are laid down by decree issued under section 117d, subsection 2 of the Land Use and Building Act </span></span><span id="23">. </span></span></div>
        
        <div data-raseType="RequirementSection" id="4"><span id="1" data-raseType="RequirementSection"><span id="1">If </span><span id="2"><span data-raseType="Application" data-raseProperty=":Contains exists =>(:type == :ParkingSpace )" id="1">parking spaces are provided for a building, </span></span><span id="3">an </span><span id="4"><span data-raseType="Requirement" data-raseProperty=":HasAppropriateNumberOfDisabledParkingSpaces == true " id="1">adequate number of them </span></span><span id="5">, </span><span id="6"><span data-raseType="Requirement" data-raseProperty=":Contains exists =>(:type == :ParkingSpace  &amp;&amp; :IsAccessible == true  )" id="1">but at least one </span></span><span id="7">, shall be intended for the use of a person with mobility and functional impairment. </span><span id="8">Such a </span><span id="9"><span data-raseType="Application" data-raseProperty=":type == :ParkingSpace  &amp;&amp; :IsAccessible == true  " id="1">parking space </span></span><span id="10">shall have a width of at least </span><span id="11"><span data-raseType="Requirement" data-raseProperty=":Width >= 3.6 " id="1">3,600 millimetres </span></span><span id="12">and a length of at </span><span id="13"><span data-raseType="Requirement" data-raseProperty=":Length &lt;= 5 " id="1">least 5,000 millimetres </span></span><span id="14">and be marked with the </span><span id="15"><span data-raseType="Requirement" data-raseProperty=":MarkedWithInternationalSymbolOfAccess == true " id="1">International Symbol of Access. </span></span></span><span id="2">The provisions of this subsection do not apply to a </span><span id="3"><span data-raseType="Exception" data-raseProperty=":type == :House " id="1">detached house, semi-detached house or townhouse. </span></span></div>
    </section>
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
coverage: FI
title: Government Decree on Accessibility of building
issued: 2017-01-01
identifier: Government_Decree_on_Accessibility_of_building
$id: FI/Government_Decree_on_Accessibility_of_building
hasPart:
- $id: FI/Government_Decree_on_Accessibility_of_building/2
  identifier: "2"
  $type:
  - DocumentSubdivision
  title: Passageway leading to a building
  hasPart:
  - $type:
    - Statement
    - RequirementStatement
    $id: FI/Government_Decree_on_Accessibility_of_building/2.1
    identifier: "2.1"
    hasInlinePart:
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.1
      identifier: 2.1.1
      asText: There shall be an easily noticeable
      $type:
      - Statement
    - asText: passageway
      $id: FI/Government_Decree_on_Accessibility_of_building/2.1.2
      identifier: 2.1.2
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.1.2_method
        identifier: 2.1.2_method
        hasBSDDTarget:
          $id: terms:isPassageway
          $type:
          - $id
        hasComparator: CheckMethodComparator-eq
        $type:
        - BooleanCheckMethod
        hasValue: "true"
      $type:
      - CheckStatement
      - ApplicationStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.3
      identifier: 2.1.3
      asText: with a width of at least
      $type:
      - Statement
    - asText: "1,200 millimetres"
      $id: FI/Government_Decree_on_Accessibility_of_building/2.1.4
      identifier: 2.1.4
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.1.4_method
        identifier: 2.1.4_method
        hasBSDDTarget:
          $id: terms:Width
          $type:
          - $id
        hasComparator: CheckMethodComparator-gt
        $type:
        - NumericalCheckMethod
        hasValue: "1.2"
      $type:
      - CheckStatement
      - RequirementStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.5
      identifier: 2.1.5
      asText: and a
      $type:
      - Statement
    - asText: "smooth,"
      $id: FI/Government_Decree_on_Accessibility_of_building/2.1.6
      identifier: 2.1.6
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.1.6_method
        identifier: 2.1.6_method
        hasBSDDTarget:
          $id: terms:Smooth
          $type:
          - $id
        hasComparator: CheckMethodComparator-eq
        $type:
        - BooleanCheckMethod
        hasValue: "true"
      $type:
      - CheckStatement
      - RequirementStatement
    - asText: hard
      $id: FI/Government_Decree_on_Accessibility_of_building/2.1.7
      identifier: 2.1.7
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.1.7_method
        identifier: 2.1.7_method
        hasBSDDTarget:
          $id: terms:Hard
          $type:
          - $id
        hasComparator: CheckMethodComparator-eq
        $type:
        - BooleanCheckMethod
        hasValue: "true"
      $type:
      - CheckStatement
      - RequirementStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.8
      identifier: 2.1.8
      asText: and
      $type:
      - Statement
    - asText: non-slippery
      $id: FI/Government_Decree_on_Accessibility_of_building/2.1.9
      identifier: 2.1.9
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.1.9_method
        identifier: 2.1.9_method
        hasBSDDTarget:
          $id: terms:NonSlip
          $type:
          - $id
        hasComparator: CheckMethodComparator-eq
        $type:
        - BooleanCheckMethod
        hasValue: "true"
      $type:
      - CheckStatement
      - RequirementStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.10
      identifier: 2.1.10
      asText: surface that leads to the
      $type:
      - Statement
    - asText: building
      $id: FI/Government_Decree_on_Accessibility_of_building/2.1.11
      identifier: 2.1.11
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.1.11_method
        identifier: 2.1.11_method
        hasBSDDTarget:
          $id: terms:ConnectsWith
          $type:
          - $id
        $type:
        - CompositeCheckMethod
        hasNestedValue:
        - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.11_method.2
          identifier: 2.1.11_method.2
          hasBSDDTarget:
            $id: terms:type
            $type:
            - $id
          hasComparator: CheckMethodComparator-eq
          hasBSDDValue:
            $id: terms:Building
            $type:
            - $id
          $type:
          - CategoryCheckMethod
        hasOperator: CheckMethodOperator-exists
      $type:
      - CheckStatement
      - ApplicationStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.12
      identifier: 2.1.12
      asText: from the
      $type:
      - Statement
    - asText: boundary of the plot or building site
      $id: FI/Government_Decree_on_Accessibility_of_building/2.1.13
      identifier: 2.1.13
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.1.13_method
        identifier: 2.1.13_method
        hasBSDDTarget:
          $id: terms:ConnectsWith
          $type:
          - $id
        $type:
        - CompositeCheckMethod
        hasNestedValue:
        - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.13_method.2
          identifier: 2.1.13_method.2
          hasBSDDTarget:
            $id: terms:type
            $type:
            - $id
          hasComparator: CheckMethodComparator-eq
          hasBSDDValue:
            $id: terms:SiteBoundary
            $type:
            - $id
          $type:
          - CategoryCheckMethod
        hasOperator: CheckMethodOperator-exists
      $type:
      - CheckStatement
      - SelectionStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.14
      identifier: 2.1.14
      asText: and from the
      $type:
      - Statement
    - asText: space and area that serve the use of the building
      $id: FI/Government_Decree_on_Accessibility_of_building/2.1.15
      identifier: 2.1.15
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.1.15_method
        identifier: 2.1.15_method
        hasBSDDTarget:
          $id: terms:ConnectsWith
          $type:
          - $id
        $type:
        - CompositeCheckMethod
        hasNestedValue:
        - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.15_method.2
          identifier: 2.1.15_method.2
          hasBSDDTarget:
            $id: terms:type
            $type:
            - $id
          hasComparator: CheckMethodComparator-eq
          hasBSDDValue:
            $id: terms:ServiceArea
            $type:
            - $id
          $type:
          - CategoryCheckMethod
        hasOperator: CheckMethodOperator-exists
      $type:
      - CheckStatement
      - SelectionStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.16
      identifier: 2.1.16
      asText: "."
      $type:
      - Statement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17
      identifier: 2.1.17
      hasInlinePart:
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.1
        identifier: 2.1.17.1
        asText: The gradient of the passageway located in an
        $type:
        - Statement
      - asText: outdoor space
        $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.2
        identifier: 2.1.17.2
        isOperationalizedBy:
          $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.2_method
          identifier: 2.1.17.2_method
          hasBSDDTarget:
            $id: terms:External
            $type:
            - $id
          hasComparator: CheckMethodComparator-eq
          $type:
          - BooleanCheckMethod
          hasValue: "true"
        $type:
        - CheckStatement
        - ApplicationStatement
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.3
        identifier: 2.1.17.3
        asText: may not
        $type:
        - Statement
      - asText: exceed five per cent
        $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.4
        identifier: 2.1.17.4
        isOperationalizedBy:
          $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.4_method
          identifier: 2.1.17.4_method
          hasBSDDTarget:
            $id: terms:Gradient
            $type:
            - $id
          hasComparator: CheckMethodComparator-le
          $type:
          - NumericalCheckMethod
          hasValue: "5"
          hasUnit:
            $type:
            - $id
            $id: units:percent
        $type:
        - CheckStatement
        - RequirementStatement
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5
        identifier: 2.1.17.5
        hasInlinePart:
        - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5.1
          identifier: 2.1.17.5.1
          asText: If there are
          $type:
          - Statement
        - asText: steps on the passageway
          $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5.2
          identifier: 2.1.17.5.2
          isOperationalizedBy:
            $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5.2_method
            identifier: 2.1.17.5.2_method
            hasBSDDTarget:
              $id: terms:Contains
              $type:
              - $id
            $type:
            - CompositeCheckMethod
            hasNestedValue:
            - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5.2_method.2
              identifier: 2.1.17.5.2_method.2
              hasBSDDTarget:
                $id: terms:type
                $type:
                - $id
              hasComparator: CheckMethodComparator-eq
              hasBSDDValue:
                $id: terms:Step
                $type:
                - $id
              $type:
              - CategoryCheckMethod
            hasOperator: CheckMethodOperator-exists
          $type:
          - CheckStatement
          - ApplicationStatement
        - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5.3
          identifier: 2.1.17.5.3
          asText: ", there shall also be a"
          $type:
          - Statement
        - asText: ramp
          $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5.4
          identifier: 2.1.17.5.4
          isOperationalizedBy:
            $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5.4_method
            identifier: 2.1.17.5.4_method
            hasBSDDTarget:
              $id: terms:Contains
              $type:
              - $id
            $type:
            - CompositeCheckMethod
            hasNestedValue:
            - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5.4_method.2
              identifier: 2.1.17.5.4_method.2
              hasBSDDTarget:
                $id: terms:type
                $type:
                - $id
              hasComparator: CheckMethodComparator-eq
              hasBSDDValue:
                $id: terms:Ramp
                $type:
                - $id
              $type:
              - CategoryCheckMethod
            hasOperator: CheckMethodOperator-exists
          $type:
          - CheckStatement
          - RequirementStatement
        - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5.5
          identifier: 2.1.17.5.5
          asText: or a
          $type:
          - Statement
        - asText: permanently installed device intended for lifting persons that is suitable for a user of a wheelchair and walking frame with wheels.
          $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5.6
          identifier: 2.1.17.5.6
          isOperationalizedBy:
            $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5.6_method
            identifier: 2.1.17.5.6_method
            hasBSDDTarget:
              $id: terms:Contains
              $type:
              - $id
            $type:
            - CompositeCheckMethod
            hasNestedValue:
            - $type:
              - CompositeCheckMethod
              $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5.6_method.2
              hasComparator: CheckMethodComparator-logicalAND
              hasNestedTarget:
                $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5.6_method.2.1
                identifier: 2.1.17.5.6_method.2.1
                hasBSDDTarget:
                  $id: terms:IsLiftingDevice
                  $type:
                  - $id
                hasComparator: CheckMethodComparator-eq
                $type:
                - BooleanCheckMethod
                hasValue: "true"
              hasNestedValue:
              - $type:
                - CompositeCheckMethod
                $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5.6_method.2.2
                hasComparator: CheckMethodComparator-logicalAND
                hasNestedTarget:
                  $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5.6_method.2.2.1
                  identifier: 2.1.17.5.6_method.2.2.1
                  hasBSDDTarget:
                    $id: terms:Permanent
                    $type:
                    - $id
                  hasComparator: CheckMethodComparator-eq
                  $type:
                  - BooleanCheckMethod
                  hasValue: "true"
                hasNestedValue:
                - $type:
                  - CompositeCheckMethod
                  $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5.6_method.2.2.2
                  hasComparator: CheckMethodComparator-logicalAND
                  hasNestedTarget:
                    $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5.6_method.2.2.2.1
                    identifier: 2.1.17.5.6_method.2.2.2.1
                    hasBSDDTarget:
                      $id: terms:SuitableForWheelchair
                      $type:
                      - $id
                    hasComparator: CheckMethodComparator-eq
                    $type:
                    - BooleanCheckMethod
                    hasValue: "true"
                  hasNestedValue:
                  - $id: FI/Government_Decree_on_Accessibility_of_building/2.1.17.5.6_method.2.2.2.2
                    identifier: 2.1.17.5.6_method.2.2.2.2
                    hasBSDDTarget:
                      $id: terms:SuitableforWalkingFrame
                      $type:
                      - $id
                    hasComparator: CheckMethodComparator-eq
                    $type:
                    - BooleanCheckMethod
                    hasValue: "true"
            hasOperator: CheckMethodOperator-exists
          $type:
          - CheckStatement
          - ExceptionStatement
        $type:
        - CheckStatement
        - RequirementStatement
      $type:
      - CheckStatement
      - RequirementStatement
  - $type:
    - Statement
    - ExceptionStatement
    $id: FI/Government_Decree_on_Accessibility_of_building/2.2
    identifier: "2.2"
    hasInlinePart:
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.2.1
      identifier: 2.2.1
      asText: The provisions of this subsection do not apply to a
      $type:
      - Statement
    - asText: "detached house , semi-detached house or townhouse"
      $id: FI/Government_Decree_on_Accessibility_of_building/2.2.2
      identifier: 2.2.2
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.2.2_method
        identifier: 2.2.2_method
        hasBSDDTarget:
          $id: terms:type
          $type:
          - $id
        hasComparator: CheckMethodComparator-eq
        hasBSDDValue:
          $id: terms:House
          $type:
          - $id
        $type:
        - CategoryCheckMethod
      $type:
      - CheckStatement
      - RequirementStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.2.3
      identifier: 2.2.3
      asText: if providing an
      $type:
      - Statement
    - asText: accessible passageway would be impossible considering the site and elevation differences
      $id: FI/Government_Decree_on_Accessibility_of_building/2.2.4
      identifier: 2.2.4
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.2.4_method
        identifier: 2.2.4_method
        hasBSDDTarget:
          $id: terms:SiteElevationDifferencesMakePassagewayImpossible
          $type:
          - $id
        hasComparator: CheckMethodComparator-eq
        $type:
        - BooleanCheckMethod
        hasValue: "true"
      $type:
      - CheckStatement
      - RequirementStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.2.5
      identifier: 2.2.5
      asText: "."
      $type:
      - Statement
  - $type:
    - Statement
    - RequirementStatement
    $id: FI/Government_Decree_on_Accessibility_of_building/2.3
    identifier: "2.3"
    hasInlinePart:
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.1
      identifier: 2.3.1
      asText: The
      $type:
      - Statement
    - asText: ramp
      $id: FI/Government_Decree_on_Accessibility_of_building/2.3.2
      identifier: 2.3.2
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.3.2_method
        identifier: 2.3.2_method
        hasBSDDTarget:
          $id: terms:type
          $type:
          - $id
        hasComparator: CheckMethodComparator-eq
        hasBSDDValue:
          $id: terms:Ramp
          $type:
          - $id
        $type:
        - CategoryCheckMethod
      $type:
      - CheckStatement
      - ApplicationStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.3
      identifier: 2.3.3
      asText: referred to in subsection 1 above shall be easily
      $type:
      - Statement
    - asText: noticeable
      $id: FI/Government_Decree_on_Accessibility_of_building/2.3.4
      identifier: 2.3.4
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.3.4_method
        identifier: 2.3.4_method
        hasBSDDTarget:
          $id: terms:Noticable
          $type:
          - $id
        hasComparator: CheckMethodComparator-eq
        $type:
        - BooleanCheckMethod
        hasValue: "true"
      $type:
      - CheckStatement
      - RequirementStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.5
      identifier: 2.3.5
      asText: and
      $type:
      - Statement
    - asText: straight
      $id: FI/Government_Decree_on_Accessibility_of_building/2.3.6
      identifier: 2.3.6
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.3.6_method
        identifier: 2.3.6_method
        hasBSDDTarget:
          $id: terms:Curvature
          $type:
          - $id
        hasComparator: CheckMethodComparator-eq
        $type:
        - NumericalCheckMethod
        hasValue: "0"
      $type:
      - CheckStatement
      - RequirementStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.7
      identifier: 2.3.7
      asText: with a
      $type:
      - Statement
    - asText: "smooth,"
      $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8
      identifier: 2.3.8
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8_method
        identifier: 2.3.8_method
        hasBSDDTarget:
          $id: terms:Smooth
          $type:
          - $id
        hasComparator: CheckMethodComparator-eq
        $type:
        - BooleanCheckMethod
        hasValue: "true"
      $type:
      - CheckStatement
      - RequirementStatement
    - asText: hard
      $id: FI/Government_Decree_on_Accessibility_of_building/2.3.9
      identifier: 2.3.9
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.3.9_method
        identifier: 2.3.9_method
        hasBSDDTarget:
          $id: terms:Hard
          $type:
          - $id
        hasComparator: CheckMethodComparator-eq
        $type:
        - BooleanCheckMethod
        hasValue: "true"
      $type:
      - CheckStatement
      - RequirementStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.10
      identifier: 2.3.10
      asText: and
      $type:
      - Statement
    - asText: non-slippery
      $id: FI/Government_Decree_on_Accessibility_of_building/2.3.11
      identifier: 2.3.11
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.3.11_method
        identifier: 2.3.11_method
        hasBSDDTarget:
          $id: terms:NonSlip
          $type:
          - $id
        hasComparator: CheckMethodComparator-eq
        $type:
        - BooleanCheckMethod
        hasValue: "true"
      $type:
      - CheckStatement
      - RequirementStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.12
      identifier: 2.3.12
      asText: "surface,"
      $type:
      - Statement
    - asText: width of at least 900 millimetres
      $id: FI/Government_Decree_on_Accessibility_of_building/2.3.13
      identifier: 2.3.13
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.3.13_method
        identifier: 2.3.13_method
        hasBSDDTarget:
          $id: terms:Width
          $type:
          - $id
        hasComparator: CheckMethodComparator-ge
        $type:
        - NumericalCheckMethod
        hasValue: "0.9"
      $type:
      - CheckStatement
      - RequirementStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.14
      identifier: 2.3.14
      asText: "and,"
      $type:
      - Statement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.1
      identifier: 2.3.1
      hasInlinePart:
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.1.1
        identifier: 2.3.1.1
        asText: if the ramp is
        $type:
        - Statement
      - asText: not connected to a fixed structure
        $id: FI/Government_Decree_on_Accessibility_of_building/2.3.1.2
        identifier: 2.3.1.2
        isOperationalizedBy:
          $id: FI/Government_Decree_on_Accessibility_of_building/2.3.1.2_method
          identifier: 2.3.1.2_method
          hasBSDDTarget:
            $id: terms:ConnectedToFixedStructure
            $type:
            - $id
          hasComparator: CheckMethodComparator-eq
          $type:
          - BooleanCheckMethod
          hasValue: "false"
        $type:
        - CheckStatement
        - ApplicationStatement
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.1.3
        identifier: 2.3.1.3
        asText: ","
        $type:
        - Statement
      - asText: a protective edge of at least 50 millimetres in height.
        $id: FI/Government_Decree_on_Accessibility_of_building/2.3.1.4
        identifier: 2.3.1.4
        isOperationalizedBy:
          $id: FI/Government_Decree_on_Accessibility_of_building/2.3.1.4_method
          identifier: 2.3.1.4_method
          hasBSDDTarget:
            $id: terms:Contains
            $type:
            - $id
          $type:
          - CompositeCheckMethod
          hasNestedValue:
          - $type:
            - CompositeCheckMethod
            $id: FI/Government_Decree_on_Accessibility_of_building/2.3.1.4_method.2
            hasComparator: CheckMethodComparator-logicalAND
            hasNestedTarget:
              $id: FI/Government_Decree_on_Accessibility_of_building/2.3.1.4_method.2.1
              identifier: 2.3.1.4_method.2.1
              hasBSDDTarget:
                $id: terms:type
                $type:
                - $id
              hasComparator: CheckMethodComparator-eq
              hasBSDDValue:
                $id: terms:ProtectiveEdge
                $type:
                - $id
              $type:
              - CategoryCheckMethod
            hasNestedValue:
            - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.1.4_method.2.2
              identifier: 2.3.1.4_method.2.2
              hasBSDDTarget:
                $id: terms:Height
                $type:
                - $id
              hasComparator: CheckMethodComparator-gt
              $type:
              - NumericalCheckMethod
              hasValue: "0.05"
          hasOperator: CheckMethodOperator-exists
        $type:
        - CheckStatement
        - RequirementStatement
      $type:
      - CheckStatement
      - RequirementStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.16
      identifier: 2.3.16
      asText: There shall be a
      $type:
      - Statement
    - asText: "horizontal landing with a length of at least 1,500 millimetres at the lower and upper end of the ramp"
      $id: FI/Government_Decree_on_Accessibility_of_building/2.3.17
      identifier: 2.3.17
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.3.17_method
        identifier: 2.3.17_method
        hasBSDDTarget:
          $id: terms:Contains
          $type:
          - $id
        $type:
        - CompositeCheckMethod
        hasNestedValue:
        - $type:
          - CompositeCheckMethod
          $id: FI/Government_Decree_on_Accessibility_of_building/2.3.17_method.2
          hasComparator: CheckMethodComparator-logicalAND
          hasNestedTarget:
            $id: FI/Government_Decree_on_Accessibility_of_building/2.3.17_method.2.1
            identifier: 2.3.17_method.2.1
            hasBSDDTarget:
              $id: terms:type
              $type:
              - $id
            hasComparator: CheckMethodComparator-eq
            hasBSDDValue:
              $id: terms:Landing
              $type:
              - $id
            $type:
            - CategoryCheckMethod
          hasNestedValue:
          - $type:
            - CompositeCheckMethod
            $id: FI/Government_Decree_on_Accessibility_of_building/2.3.17_method.2.2
            hasComparator: CheckMethodComparator-logicalAND
            hasNestedTarget:
              $id: FI/Government_Decree_on_Accessibility_of_building/2.3.17_method.2.2.1
              identifier: 2.3.17_method.2.2.1
              hasBSDDTarget:
                $id: terms:Orientation
                $type:
                - $id
              hasComparator: CheckMethodComparator-eq
              hasBSDDValue:
                $id: terms:Horizontal
                $type:
                - $id
              $type:
              - CategoryCheckMethod
            hasNestedValue:
            - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.17_method.2.2.2
              identifier: 2.3.17_method.2.2.2
              hasBSDDTarget:
                $id: terms:LandingLength
                $type:
                - $id
              hasComparator: CheckMethodComparator-gt
              $type:
              - NumericalCheckMethod
              hasValue: "1.5"
        hasOperator: CheckMethodOperator-exists
      $type:
      - CheckStatement
      - RequirementStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.18
      identifier: 2.3.18
      asText: . The gradient of the ramp may
      $type:
      - Statement
    - asText: not exceed five per cent
      $id: FI/Government_Decree_on_Accessibility_of_building/2.3.19
      identifier: 2.3.19
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.3.19_method
        identifier: 2.3.19_method
        hasBSDDTarget:
          $id: terms:Gradient
          $type:
          - $id
        hasComparator: CheckMethodComparator-le
        $type:
        - NumericalCheckMethod
        hasValue: "5"
        hasUnit:
          $type:
          - $id
          $id: units:percent
      $type:
      - CheckStatement
      - RequirementStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.20
      identifier: 2.3.20
      asText: "."
      $type:
      - Statement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8
      identifier: 2.3.8
      hasInlinePart:
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.1
        identifier: 2.3.8.1
        asText: "However, if the"
        $type:
        - Statement
      - asText: "elevation difference is no more than 1,000 millimetres"
        $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.2
        identifier: 2.3.8.2
        isOperationalizedBy:
          $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.2_method
          identifier: 2.3.8.2_method
          hasBSDDTarget:
            $id: terms:ElevationChange
            $type:
            - $id
          hasComparator: CheckMethodComparator-le
          $type:
          - NumericalCheckMethod
          hasValue: "1"
        $type:
        - CheckStatement
        - ApplicationStatement
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.3
        identifier: 2.3.8.3
        asText: ", the ramp may"
        $type:
        - Statement
      - asText: not have a gradient of more than eight per cent
        $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.4
        identifier: 2.3.8.4
        isOperationalizedBy:
          $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.4_method
          identifier: 2.3.8.4_method
          hasBSDDTarget:
            $id: terms:Gradient
            $type:
            - $id
          hasComparator: CheckMethodComparator-le
          $type:
          - NumericalCheckMethod
          hasValue: "8"
          hasUnit:
            $type:
            - $id
            $id: units:percent
        $type:
        - CheckStatement
        - RequirementStatement
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.5
        identifier: 2.3.8.5
        asText: ". In that case,"
        $type:
        - Statement
      - asText: the elevation difference of a continuous ramp may not be more than 500 millimetres
        $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.6
        identifier: 2.3.8.6
        isOperationalizedBy:
          $type:
          - CompositeCheckMethod
          $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.6_method
          hasComparator: CheckMethodComparator-logicalAND
          hasNestedTarget:
            $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.6_method.1
            identifier: 2.3.8.6_method.1
            hasBSDDTarget:
              $id: terms:Contains
              $type:
              - $id
            $type:
            - CompositeCheckMethod
            hasNestedValue:
            - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.6_method.1.2
              identifier: 2.3.8.6_method.1.2
              hasBSDDTarget:
                $id: terms:type
                $type:
                - $id
              hasComparator: CheckMethodComparator-eq
              hasBSDDValue:
                $id: terms:Landing
                $type:
                - $id
              $type:
              - CategoryCheckMethod
            hasOperator: CheckMethodOperator-notExists
          hasNestedValue:
          - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.6_method.2
            identifier: 2.3.8.6_method.2
            hasBSDDTarget:
              $id: terms:ElevationChange
              $type:
              - $id
            hasComparator: CheckMethodComparator-lt
            $type:
            - NumericalCheckMethod
            hasValue: "0.5"
        $type:
        - CheckStatement
        - RequirementStatement
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.7
        identifier: 2.3.8.7
        asText: ","
        $type:
        - Statement
      - asText: "after which there shall be a horizontal intermediate landing with a length of at least 2,000 millimetres"
        $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.8
        identifier: 2.3.8.8
        isOperationalizedBy:
          $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.8_method
          identifier: 2.3.8.8_method
          hasBSDDTarget:
            $id: terms:Contains
            $type:
            - $id
          $type:
          - CompositeCheckMethod
          hasNestedValue:
          - $type:
            - CompositeCheckMethod
            $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.8_method.2
            hasComparator: CheckMethodComparator-logicalAND
            hasNestedTarget:
              $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.8_method.2.1
              identifier: 2.3.8.8_method.2.1
              hasBSDDTarget:
                $id: terms:type
                $type:
                - $id
              hasComparator: CheckMethodComparator-eq
              hasBSDDValue:
                $id: terms:Landing
                $type:
                - $id
              $type:
              - CategoryCheckMethod
            hasNestedValue:
            - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.8_method.2.2
              identifier: 2.3.8.8_method.2.2
              hasBSDDTarget:
                $id: terms:LandingLength
                $type:
                - $id
              hasComparator: CheckMethodComparator-ge
              $type:
              - NumericalCheckMethod
              hasValue: "2"
          hasOperator: CheckMethodOperator-exists
        $type:
        - CheckStatement
        - ExceptionStatement
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.8.9
        identifier: 2.3.8.9
        asText: "."
        $type:
        - Statement
      $type:
      - CheckStatement
      - RequirementStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.9
      identifier: 2.3.9
      hasInlinePart:
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.9.1
        identifier: 2.3.9.1
        asText: "However, in an"
        $type:
        - Statement
      - asText: outdoor
        $id: FI/Government_Decree_on_Accessibility_of_building/2.3.9.2
        identifier: 2.3.9.2
        isOperationalizedBy:
          $id: FI/Government_Decree_on_Accessibility_of_building/2.3.9.2_method
          identifier: 2.3.9.2_method
          hasBSDDTarget:
            $id: terms:External
            $type:
            - $id
          hasComparator: CheckMethodComparator-eq
          $type:
          - BooleanCheckMethod
          hasValue: "true"
        $type:
        - CheckStatement
        - ApplicationStatement
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.9.3
        identifier: 2.3.9.3
        asText: area the ramp may have a
        $type:
        - Statement
      - asText: gradient of more than five per cent
        $id: FI/Government_Decree_on_Accessibility_of_building/2.3.9.4
        identifier: 2.3.9.4
        isOperationalizedBy:
          $id: FI/Government_Decree_on_Accessibility_of_building/2.3.9.4_method
          identifier: 2.3.9.4_method
          hasBSDDTarget:
            $id: terms:Gradient
            $type:
            - $id
          hasComparator: CheckMethodComparator-gt
          $type:
          - NumericalCheckMethod
          hasValue: "5"
          hasUnit:
            $type:
            - $id
            $id: units:percent
        $type:
        - CheckStatement
        - ApplicationStatement
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.9.5
        identifier: 2.3.9.5
        asText: only if it can be kept in a condition comparable with that of an indoor ramp.
        $type:
        - Statement
      - asText: "Provisions on railings, handrails and other arrangements intended to prevent falling down and misstepping are laid down by decree issued under section 117d, subsection 2 of the Land Use and Building Act"
        $id: FI/Government_Decree_on_Accessibility_of_building/2.3.9.6
        identifier: 2.3.9.6
        references: Land Use and Building Act.117.d.2
        $type:
        - CheckStatement
        - RequirementStatement
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.3.9.7
        identifier: 2.3.9.7
        asText: "."
        $type:
        - Statement
      $type:
      - CheckStatement
      - RequirementStatement
  - $type:
    - Statement
    - RequirementStatement
    $id: FI/Government_Decree_on_Accessibility_of_building/2.4
    identifier: "2.4"
    hasInlinePart:
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1
      identifier: 2.4.1
      hasInlinePart:
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.1
        identifier: 2.4.1.1
        asText: If
        $type:
        - Statement
      - asText: "parking spaces are provided for a building,"
        $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.2
        identifier: 2.4.1.2
        isOperationalizedBy:
          $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.2_method
          identifier: 2.4.1.2_method
          hasBSDDTarget:
            $id: terms:Contains
            $type:
            - $id
          $type:
          - CompositeCheckMethod
          hasNestedValue:
          - $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.2_method.2
            identifier: 2.4.1.2_method.2
            hasBSDDTarget:
              $id: terms:type
              $type:
              - $id
            hasComparator: CheckMethodComparator-eq
            hasBSDDValue:
              $id: terms:ParkingSpace
              $type:
              - $id
            $type:
            - CategoryCheckMethod
          hasOperator: CheckMethodOperator-exists
        $type:
        - CheckStatement
        - ApplicationStatement
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.3
        identifier: 2.4.1.3
        asText: an
        $type:
        - Statement
      - asText: adequate number of them
        $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.4
        identifier: 2.4.1.4
        isOperationalizedBy:
          $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.4_method
          identifier: 2.4.1.4_method
          hasBSDDTarget:
            $id: terms:HasAppropriateNumberOfDisabledParkingSpaces
            $type:
            - $id
          hasComparator: CheckMethodComparator-eq
          $type:
          - BooleanCheckMethod
          hasValue: "true"
        $type:
        - CheckStatement
        - RequirementStatement
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.5
        identifier: 2.4.1.5
        asText: ","
        $type:
        - Statement
      - asText: but at least one
        $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.6
        identifier: 2.4.1.6
        isOperationalizedBy:
          $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.6_method
          identifier: 2.4.1.6_method
          hasBSDDTarget:
            $id: terms:Contains
            $type:
            - $id
          $type:
          - CompositeCheckMethod
          hasNestedValue:
          - $type:
            - CompositeCheckMethod
            $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.6_method.2
            hasComparator: CheckMethodComparator-logicalAND
            hasNestedTarget:
              $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.6_method.2.1
              identifier: 2.4.1.6_method.2.1
              hasBSDDTarget:
                $id: terms:type
                $type:
                - $id
              hasComparator: CheckMethodComparator-eq
              hasBSDDValue:
                $id: terms:ParkingSpace
                $type:
                - $id
              $type:
              - CategoryCheckMethod
            hasNestedValue:
            - $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.6_method.2.2
              identifier: 2.4.1.6_method.2.2
              hasBSDDTarget:
                $id: terms:IsAccessible
                $type:
                - $id
              hasComparator: CheckMethodComparator-eq
              $type:
              - BooleanCheckMethod
              hasValue: "true"
          hasOperator: CheckMethodOperator-exists
        $type:
        - CheckStatement
        - RequirementStatement
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.7
        identifier: 2.4.1.7
        asText: ", shall be intended for the use of a person with mobility and functional impairment."
        $type:
        - Statement
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.8
        identifier: 2.4.1.8
        asText: Such a
        $type:
        - Statement
      - asText: parking space
        $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.9
        identifier: 2.4.1.9
        isOperationalizedBy:
          $type:
          - CompositeCheckMethod
          $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.9_method
          hasComparator: CheckMethodComparator-logicalAND
          hasNestedTarget:
            $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.9_method.1
            identifier: 2.4.1.9_method.1
            hasBSDDTarget:
              $id: terms:type
              $type:
              - $id
            hasComparator: CheckMethodComparator-eq
            hasBSDDValue:
              $id: terms:ParkingSpace
              $type:
              - $id
            $type:
            - CategoryCheckMethod
          hasNestedValue:
          - $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.9_method.2
            identifier: 2.4.1.9_method.2
            hasBSDDTarget:
              $id: terms:IsAccessible
              $type:
              - $id
            hasComparator: CheckMethodComparator-eq
            $type:
            - BooleanCheckMethod
            hasValue: "true"
        $type:
        - CheckStatement
        - ApplicationStatement
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.10
        identifier: 2.4.1.10
        asText: shall have a width of at least
        $type:
        - Statement
      - asText: "3,600 millimetres"
        $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.11
        identifier: 2.4.1.11
        isOperationalizedBy:
          $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.11_method
          identifier: 2.4.1.11_method
          hasBSDDTarget:
            $id: terms:Width
            $type:
            - $id
          hasComparator: CheckMethodComparator-ge
          $type:
          - NumericalCheckMethod
          hasValue: "3.6"
        $type:
        - CheckStatement
        - RequirementStatement
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.12
        identifier: 2.4.1.12
        asText: and a length of at
        $type:
        - Statement
      - asText: "least 5,000 millimetres"
        $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.13
        identifier: 2.4.1.13
        isOperationalizedBy:
          $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.13_method
          identifier: 2.4.1.13_method
          hasBSDDTarget:
            $id: terms:Length
            $type:
            - $id
          hasComparator: CheckMethodComparator-le
          $type:
          - NumericalCheckMethod
          hasValue: "5"
        $type:
        - CheckStatement
        - RequirementStatement
      - $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.14
        identifier: 2.4.1.14
        asText: and be marked with the
        $type:
        - Statement
      - asText: International Symbol of Access.
        $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.15
        identifier: 2.4.1.15
        isOperationalizedBy:
          $id: FI/Government_Decree_on_Accessibility_of_building/2.4.1.15_method
          identifier: 2.4.1.15_method
          hasBSDDTarget:
            $id: terms:MarkedWithInternationalSymbolOfAccess
            $type:
            - $id
          hasComparator: CheckMethodComparator-eq
          $type:
          - BooleanCheckMethod
          hasValue: "true"
        $type:
        - CheckStatement
        - RequirementStatement
      $type:
      - CheckStatement
      - RequirementStatement
    - $id: FI/Government_Decree_on_Accessibility_of_building/2.4.2
      identifier: 2.4.2
      asText: The provisions of this subsection do not apply to a
      $type:
      - Statement
    - asText: "detached house, semi-detached house or townhouse."
      $id: FI/Government_Decree_on_Accessibility_of_building/2.4.3
      identifier: 2.4.3
      isOperationalizedBy:
        $id: FI/Government_Decree_on_Accessibility_of_building/2.4.3_method
        identifier: 2.4.3_method
        hasBSDDTarget:
          $id: terms:type
          $type:
          - $id
        hasComparator: CheckMethodComparator-eq
        hasBSDDValue:
          $id: terms:House
          $type:
          - $id
        $type:
        - CategoryCheckMethod
      $type:
      - CheckStatement
      - ExceptionStatement

```
