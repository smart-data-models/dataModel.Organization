<!-- 10-Header -->  
[![Smart Data Models](https://smartdatamodels.org/wp-content/uploads/2022/01/SmartDataModels_logo.png "Logo")](https://smartdatamodels.org)  
Entität: Organisation  
=====================<!-- /10-Header -->  
<!-- 15-License -->  
[Offene Lizenz](https://github.com/smart-data-models//dataModel.Organization/blob/master/Organization/LICENSE.md)  
[Dokument automatisch generiert](https://docs.google.com/presentation/d/e/2PACX-1vTs-Ng5dIAwkg91oTTUdt8ua7woBXhPnwavZ0FxgR8BsAI_Ek3C5q97Nd94HS8KhP-r_quD4H0fgyt3/pub?start=false&loop=false&delayms=3000#slide=id.gb715ace035_0_60)  
<!-- /15-License -->  
<!-- 20-Description -->  
Globale Beschreibung: **Eine Organisation wie z. B. eine Schule, eine Nichtregierungsorganisation, ein Unternehmen, ein Verein usw., abgebildet von schema.org**  
Version: 0.0.3  
<!-- /20-Description -->  
<!-- 30-PropertiesList -->  

## Liste der Eigenschaften  

<sup><sub>[*] Wenn es für ein Attribut keinen Typ gibt, kann es mehrere Typen oder verschiedene Formate/Muster haben</sub></sup>.  
- `address[object]`: Die Postanschrift  . Model: [https://schema.org/address](https://schema.org/address)	- `addressCountry[string]`: Das Land. Zum Beispiel, Spanien  . Model: [https://schema.org/addressCountry](https://schema.org/addressCountry)  
	- `addressLocality[string]`: Die Ortschaft, in der sich die Adresse befindet, und die in der Region liegt  . Model: [https://schema.org/addressLocality](https://schema.org/addressLocality)  
	- `addressRegion[string]`: Die Region, in der sich der Ort befindet, und die auf dem Land liegt  . Model: [https://schema.org/addressRegion](https://schema.org/addressRegion)  
	- `district[string]`: Ein Bezirk ist eine Art von Verwaltungseinheit, die in einigen Ländern von der lokalen Regierung verwaltet wird.    
	- `postOfficeBoxNumber[string]`: Die Postfachnummer für Postfachadressen. Zum Beispiel, 03578  . Model: [https://schema.org/postOfficeBoxNumber](https://schema.org/postOfficeBoxNumber)  
	- `postalCode[string]`: Die Postleitzahl. Zum Beispiel, 24004  . Model: [https://schema.org/https://schema.org/postalCode](https://schema.org/https://schema.org/postalCode)  
	- `streetAddress[string]`: Die Straßenanschrift  . Model: [https://schema.org/streetAddress](https://schema.org/streetAddress)  
- `aggregateRating[object]`: Die durchschnittliche Bewertung auf der Grundlage mehrerer Bewertungen oder Rezensionen. Datenschutz:'niedrig'  	- `itemReviewed[*]`: Der Artikel, der geprüft/bewertet wird.    
	- `ratingCount`:     
- `alternateName[string]`: Ein alternativer Name für diesen Artikel  - `areaServed[string]`: Das geografische Gebiet, in dem eine Dienstleistung oder ein angebotener Artikel erbracht wird  . Model: [https://schema.org/Text](https://schema.org/Text)- `author[uri]`: Der Autor dieses Inhalts oder dieser Bewertung. Bitte beachten Sie, dass author insofern eine Besonderheit darstellt, als HTML 5 einen speziellen Mechanismus zur Angabe der Urheberschaft über das rel-Tag bereitstellt. Dies ist gleichbedeutend mit diesem und kann austauschbar verwendet werden  . Model: [https://schema.org/URL](https://schema.org/URL)- `bestRating[number]`: Der höchste in diesem Bewertungssystem zulässige Wert. Wenn bestRating weggelassen wird, wird 5 angenommen.  . Model: [https://schema.org/Number](https://schema.org/Number)- `dataProvider[string]`: Eine Folge von Zeichen zur Identifizierung des Anbieters der harmonisierten Dateneinheit  - `dateCreated[date-time]`: Zeitstempel der Entitätserstellung. Dieser wird normalerweise von der Speicherplattform zugewiesen  - `dateModified[date-time]`: Zeitstempel der letzten Änderung der Entität. Dieser wird in der Regel von der Speicherplattform vergeben  - `description[string]`: Eine Beschreibung dieses Artikels  - `id[*]`: Eindeutiger Bezeichner der Entität  - `legalName[string]`: Der offizielle Name der Organisation, z. B. der eingetragene Firmenname  . Model: [https://schema.org/legalName](https://schema.org/legalName)- `location[*]`: Geojson-Referenz auf das Element. Es kann Punkt, LineString, Polygon, MultiPoint, MultiLineString oder MultiPolygon sein  - `name[string]`: Der Name dieses Artikels  - `owner[array]`: Eine Liste mit einer JSON-kodierten Zeichenfolge, die auf die eindeutigen Kennungen der Eigentümer verweist  - `reviewAspect[string]`: Diese Rezension oder Bewertung bezieht sich auf diesen Teil oder diese Facette des ArtikelsBesprochen  . Model: [https://schema.org/Text](https://schema.org/Text)- `seeAlso[*]`: Liste von URLs, die auf zusätzliche Ressourcen zu dem Artikel verweisen  - `source[string]`: Eine Folge von Zeichen, die die ursprüngliche Quelle der Entitätsdaten als URL angibt. Empfohlen wird der voll qualifizierte Domänenname des Quellanbieters oder die URL des Quellobjekts.  - `taxID[string]`: Die Steuer-/Fiskal-ID der Organisation oder Person, z. B. die TIN in den USA oder die CIF/NIF in Spanien  . Model: [https://schema.org/taxID](https://schema.org/taxID)- `type[string]`: NGSI-Entitätstyp. Es muss Organisation sein  - `url[uri]`: URL, die eine Beschreibung oder weitere Informationen zu diesem Artikel enthält  <!-- /30-PropertiesList -->  
<!-- 35-RequiredProperties -->  
Erforderliche Eigenschaften  
- `id`  - `type`  <!-- /35-RequiredProperties -->  
<!-- 40-RequiredProperties -->  
<!-- /40-RequiredProperties -->  
<!-- 50-DataModelHeader -->  
## Datenmodell Beschreibung der Eigenschaften  
Alphabetisch sortiert (für Details anklicken)  
<!-- /50-DataModelHeader -->  
<!-- 60-ModelYaml -->  
<details><summary><strong>full yaml details</strong></summary>    
```yaml  
Organization:    
  description: 'An organization such as a school, NGO, corporation, club, etc, mapped from schema.org'    
  properties:    
    address:    
      description: The mailing address    
      properties:    
        addressCountry:    
          description: 'The country. For example, Spain'    
          type: string    
          x-ngsi:    
            model: https://schema.org/addressCountry    
            type: Property    
        addressLocality:    
          description: 'The locality in which the street address is, and which is in the region'    
          type: string    
          x-ngsi:    
            model: https://schema.org/addressLocality    
            type: Property    
        addressRegion:    
          description: 'The region in which the locality is, and which is in the country'    
          type: string    
          x-ngsi:    
            model: https://schema.org/addressRegion    
            type: Property    
        district:    
          description: 'A district is a type of administrative division that, in some countries, is managed by the local government'    
          type: string    
          x-ngsi:    
            type: Property    
        postOfficeBoxNumber:    
          description: 'The post office box number for PO box addresses. For example, 03578'    
          type: string    
          x-ngsi:    
            model: https://schema.org/postOfficeBoxNumber    
            type: Property    
        postalCode:    
          description: 'The postal code. For example, 24004'    
          type: string    
          x-ngsi:    
            model: https://schema.org/https://schema.org/postalCode    
            type: Property    
        streetAddress:    
          description: The street address    
          type: string    
          x-ngsi:    
            model: https://schema.org/streetAddress    
            type: Property    
        streetNr:    
          description: Number identifying a specific property on a public street    
          type: string    
          x-ngsi:    
            type: Property    
      type: object    
      x-ngsi:    
        model: https://schema.org/address    
        type: Property    
    aggregateRating:    
      description: 'The average rating based on multiple ratings or reviews. Privacy:''low'''    
      properties:    
        itemReviewed:    
          anyOf:    
            - description: Identifier format of any NGSI entity    
              maxLength: 256    
              minLength: 1    
              pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
              type: string    
              x-ngsi:    
                type: Property    
            - description: Identifier format of any NGSI entity    
              format: uri    
              type: string    
              x-ngsi:    
                type: Property    
          description: 'The item that is being reviewed/rated. '    
          x-ngsi:    
            type: Relationship    
        ratingCount:    
          minimum: 0    
          type: number    
        reviewCount:    
          minimum: 0    
          type: number    
      type: object    
      x-ngsi:    
        type: Property    
    alternateName:    
      description: An alternative name for this item    
      type: string    
      x-ngsi:    
        type: Property    
    areaServed:    
      description: The geographic area where a service or offered item is provided    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    author:    
      description: The author of this content or rating. Please note that author is special in that HTML 5 provides a special mechanism for indicating authorship via the rel tag. That is equivalent to this and may be used interchangeably    
      format: uri    
      type: string    
      x-ngsi:    
        model: https://schema.org/URL    
        type: Relationship    
    bestRating:    
      description: 'The highest value allowed in this rating system. If bestRating is omitted, 5 is assumed. '    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
    dataProvider:    
      description: A sequence of characters identifying the provider of the harmonised data entity    
      type: string    
      x-ngsi:    
        type: Property    
    dateCreated:    
      description: Entity creation timestamp. This will usually be allocated by the storage platform    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    dateModified:    
      description: Timestamp of the last modification of the entity. This will usually be allocated by the storage platform    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    description:    
      description: A description of this item    
      type: string    
      x-ngsi:    
        type: Property    
    id:    
      anyOf:    
        - description: Identifier format of any NGSI entity    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
          x-ngsi:    
            type: Property    
        - description: Identifier format of any NGSI entity    
          format: uri    
          type: string    
          x-ngsi:    
            type: Property    
      description: Unique identifier of the entity    
      x-ngsi:    
        type: Property    
    legalName:    
      description: 'The official name of the organization, e.g. the registered company name'    
      type: string    
      x-ngsi:    
        model: https://schema.org/legalName    
        type: Property    
    location:    
      description: 'Geojson reference to the item. It can be Point, LineString, Polygon, MultiPoint, MultiLineString or MultiPolygon'    
      oneOf:    
        - description: Geojson reference to the item. Point    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                type: number    
              minItems: 2    
              type: array    
            type:    
              enum:    
                - Point    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON Point    
          type: object    
          x-ngsi:    
            type: GeoProperty    
        - description: Geojson reference to the item. LineString    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  type: number    
                minItems: 2    
                type: array    
              minItems: 2    
              type: array    
            type:    
              enum:    
                - LineString    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON LineString    
          type: object    
          x-ngsi:    
            type: GeoProperty    
        - description: Geojson reference to the item. Polygon    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  items:    
                    type: number    
                  minItems: 2    
                  type: array    
                minItems: 4    
                type: array    
              type: array    
            type:    
              enum:    
                - Polygon    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON Polygon    
          type: object    
          x-ngsi:    
            type: GeoProperty    
        - description: Geojson reference to the item. MultiPoint    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  type: number    
                minItems: 2    
                type: array    
              type: array    
            type:    
              enum:    
                - MultiPoint    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON MultiPoint    
          type: object    
          x-ngsi:    
            type: GeoProperty    
        - description: Geojson reference to the item. MultiLineString    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  items:    
                    type: number    
                  minItems: 2    
                  type: array    
                minItems: 2    
                type: array    
              type: array    
            type:    
              enum:    
                - MultiLineString    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON MultiLineString    
          type: object    
          x-ngsi:    
            type: GeoProperty    
        - description: Geojson reference to the item. MultiLineString    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  items:    
                    items:    
                      type: number    
                    minItems: 2    
                    type: array    
                  minItems: 4    
                  type: array    
                type: array    
              type: array    
            type:    
              enum:    
                - MultiPolygon    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON MultiPolygon    
          type: object    
          x-ngsi:    
            type: GeoProperty    
      x-ngsi:    
        type: GeoProperty    
    name:    
      description: The name of this item    
      type: string    
      x-ngsi:    
        type: Property    
    owner:    
      description: A List containing a JSON encoded sequence of characters referencing the unique Ids of the owner(s)    
      items:    
        anyOf:    
          - description: Identifier format of any NGSI entity    
            maxLength: 256    
            minLength: 1    
            pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
            type: string    
            x-ngsi:    
              type: Property    
          - description: Identifier format of any NGSI entity    
            format: uri    
            type: string    
            x-ngsi:    
              type: Property    
        description: Unique identifier of the entity    
        x-ngsi:    
          type: Property    
      type: array    
      x-ngsi:    
        type: Property    
    reviewAspect:    
      description: This Review or Rating is relevant to this part or facet of the itemReviewed    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    seeAlso:    
      description: list of uri pointing to additional resources about the item    
      oneOf:    
        - items:    
            format: uri    
            type: string    
          minItems: 1    
          type: array    
        - format: uri    
          type: string    
      x-ngsi:    
        type: Property    
    source:    
      description: 'A sequence of characters giving the original source of the entity data as a URL. Recommended to be the fully qualified domain name of the source provider, or the URL to the source object'    
      type: string    
      x-ngsi:    
        type: Property    
    taxID:    
      description: 'The Tax / Fiscal ID of the organization or person, e.g. the TIN in the US or the CIF/NIF in Spain'    
      type: string    
      x-ngsi:    
        model: https://schema.org/taxID    
        type: Property    
    type:    
      description: NGSI entity type. It has to be Organization    
      enum:    
        - Organization    
      type: string    
      x-ngsi:    
        type: Property    
    url:    
      description: URL which provides a description or further information about this item    
      format: uri    
      type: string    
      x-ngsi:    
        type: Property    
  required:    
    - id    
    - type    
  type: object    
  x-derived-from: https://schema.org/Organization    
  x-disclaimer: 'Redistribution and use in source and binary forms, with or without modification, are permitted  provided that the license conditions are met. Copyleft (c) 2022 Contributors to Smart Data Models Program'    
  x-license-url: https://github.com/smart-data-models/dataModel.Organization/blob/master/Organization/LICENSE.md    
  x-model-schema: https://smart-data-models.github.io/DataModel.Organization/Organization/schema.json    
  x-model-tags: ""    
  x-version: 0.0.3    
```  
</details>    
<!-- /60-ModelYaml -->  
<!-- 70-MiddleNotes -->  
<!-- /70-MiddleNotes -->  
<!-- 80-Examples -->  
## Beispiel-Nutzlasten  
#### Organisation NGSI-v2 Schlüsselwerte Beispiel  
Hier ist ein Beispiel für eine Organisation im JSON-LD-Format als Schlüsselwerte. Dies ist kompatibel mit NGSI-v2, wenn `options=keyValues` verwendet wird und liefert die Kontextdaten einer einzelnen Entität.  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "urn:ngsi-ld:Organization:34f91f29-aadd-45f7-ab9e-4fca2baffdd7",  
  "type": "Organization",  
  "dateCreated": "2022-06-21T08:24:35.905712+02:00",  
  "dateModified": "2022-06-22T09:24:35.905712+02:00",  
  "name": "Example Organization",  
  "location": {  
    "type": "Point",  
    "coordinates": [  
      49.40,  
      8.68  
    ]  
  },  
  "address": {  
    "addressLocality": "Heidelberg",  
    "postalCode": "69115",  
    "streetAddress": "Example-Street 42"  
  },  
  "areaServed": "Stadt Heidelberg",  
  "url": "https://www.example-organization-homepage.com",  
  "legalName": "Beispielname GmbH",  
  "taxID": "12345678900"  
}  
```  
</details>  
#### Organisation NGSI-v2 normalisiert Beispiel  
Hier ist ein Beispiel für eine Organisation im JSON-LD-Format in normalisierter Form. Dies ist kompatibel mit NGSI-v2, wenn keine Optionen verwendet werden, und liefert die Kontextdaten einer einzelnen Entität.  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "urn:ngsi-ld:Organization:34f91f29-aadd-45f7-ab9e-4fca2baffdd7",  
  "type": "Organization",  
  "dateCreated": {  
    "type": "Date-Time",  
    "value": "2022-06-21T08:24:35.905712+02:00"  
  },  
  "dateModified": {  
    "type": "Date-Time",  
    "value": "2022-06-22T09:24:35.905712+02:00"  
  },  
  "name": {  
    "type": "Text",  
    "value": "Example Organization"  
  },  
  "location": {  
    "type": "geo:json",  
    "value": {  
      "type": "Point",  
      "coordinates": [  
        49.40,  
        8.68  
      ]  
    }  
  },  
  "address": {  
    "type": "PostalAddress",  
    "value": {  
      "addressLocality": "Heidelberg",  
      "postalCode": "69115",  
      "streetAddress": "Example-Street 42"  
    }  
  },  
  "areaServed": {  
    "type": "Text",  
    "value": "Stadt Heidelberg"  
  },  
  "url": {  
    "type": "URI",  
    "value": "https://www.example-organization-homepage.com"  
  },  
  "legalName": {  
    "type": "Text",  
    "value": "Beispielname GmbH"  
  },  
  "taxID": {  
    "type": "Text",  
    "value": "12345678900"  
  },  
  "@context": [  
    "https://smart-data-models.github.io/DataModel.Organization/context.jsonld"  
  ]  
}  
```  
</details>  
#### Organisation NGSI-LD Schlüsselwerte Beispiel  
Hier ist ein Beispiel für eine Organisation im JSON-LD-Format als Schlüsselwerte. Dies ist kompatibel mit NGSI-LD, wenn `options=keyValues` verwendet wird und liefert die Kontextdaten einer einzelnen Entität.  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
    "id": "urn:ngsi-ld:Organization:34f91f29-aadd-45f7-ab9e-4fca2baffdd7",  
    "type": "Organization",  
    "dateCreated": "2022-06-21T08:24:35.905712+02:00",  
    "dateModified": "2022-06-22T09:24:35.905712+02:00",  
    "name": "Example Organization",  
    "location": {  
        "type": "Point",  
        "coordinates": [  
            49.4,  
            8.68  
        ]  
    },  
    "address": {  
        "addressLocality": "Heidelberg",  
        "postalCode": "69115",  
        "streetAddress": "Example-Street 42"  
    },  
    "areaServed": "Stadt Heidelberg",  
    "url": "https://www.example-organization-homepage.com",  
    "legalName": "Beispielname GmbH",  
    "taxID": "12345678900",  
    "@context": [  
        "https://smart-data-models.github.io/DataModel.Organization/context.jsonld",  
        "https://raw.githubusercontent.com/smart-data-models/dataModel.Organization/master/context.jsonld"  
    ]  
}  
```  
</details>  
#### Organisation NGSI-LD normalisiert Beispiel  
Hier ist ein Beispiel für eine Organisation im JSON-LD-Format in normalisierter Form. Dies ist kompatibel mit NGSI-LD, wenn keine Optionen verwendet werden, und liefert die Kontextdaten einer einzelnen Entität.  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
    "id": "urn:ngsi-ld:Organization:34f91f29-aadd-45f7-ab9e-4fca2baffdd7",  
    "type": "Organization",  
    "dateCreated": {  
        "type": "Property",  
        "value": "2022-06-21T08:24:35.905712+02:00"  
    },  
    "dateModified": {  
        "type": "Property",  
        "value": "2022-06-22T09:24:35.905712+02:00"  
    },  
    "name": {  
        "type": "Property",  
        "value": "Example Organization"  
    },  
    "location": {  
        "type": "GeoProperty",  
        "value": {  
            "type": "Point",  
            "coordinates": [  
                49.4,  
                8.68  
            ]  
        }  
    },  
    "address": {  
        "type": "Property",  
        "value": {  
            "addressLocality": "Heidelberg",  
            "postalCode": "69115",  
            "streetAddress": "Example-Street 42"  
        }  
    },  
    "areaServed": {  
        "type": "Property",  
        "value": "Stadt Heidelberg"  
    },  
    "url": {  
        "type": "Property",  
        "value": "https://www.example-organization-homepage.com"  
    },  
    "legalName": {  
        "type": "Property",  
        "value": "Beispielname GmbH"  
    },  
    "taxID": {  
        "type": "Property",  
        "value": "12345678900"  
    },  
    "@context": [  
        "https://smart-data-models.github.io/DataModel.Organization/context.jsonld",  
        "https://raw.githubusercontent.com/smart-data-models/dataModel.Organization/master/context.jsonld"  
    ]  
}  
```  
</details><!-- /80-Examples -->  
<!-- 90-FooterNotes -->  
<!-- /90-FooterNotes -->  
<!-- 95-Units -->  
Siehe [FAQ 10] (https://smartdatamodels.org/index.php/faqs/), um eine Antwort auf die Frage zu erhalten, wie man mit Größeneinheiten umgeht  
<!-- /95-Units -->  
<!-- 97-LastFooter -->  
---  
[Smart Data Models](https://smartdatamodels.org) +++ [Contribution Manual](https://bit.ly/contribution_manual) +++ [About](https://bit.ly/Introduction_SDM)<!-- /97-LastFooter -->  
