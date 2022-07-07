[![Smart Data Models](https://smartdatamodels.org/wp-content/uploads/2022/01/SmartDataModels_logo.png "Logo")](https://smartdatamodels.org)  
Entità: Organizzazione  
======================  
[Licenza aperta](https://github.com/smart-data-models//dataModel.Organization/blob/master/Organization/LICENSE.md)  
[documento generato automaticamente](https://docs.google.com/presentation/d/e/2PACX-1vTs-Ng5dIAwkg91oTTUdt8ua7woBXhPnwavZ0FxgR8BsAI_Ek3C5q97Nd94HS8KhP-r_quD4H0fgyt3/pub?start=false&loop=false&delayms=3000#slide=id.gb715ace035_0_60)  
Descrizione globale: **Un'organizzazione come una scuola, una ONG, un'azienda, un club, ecc, mappata da schema.org**  
versione: 0.0.2  

## Elenco delle proprietà  

- `address`: L'indirizzo postale  - `aggregateRating`: La valutazione media basata su più valutazioni o recensioni. Privacy:'basso'  - `alternateName`: Un nome alternativo per questa voce  - `areaServed`: L'area geografica in cui viene fornito il servizio o l'articolo offerto.  - `author`: L'autore di questo contenuto o valutazione. Si noti che author è speciale in quanto HTML 5 fornisce un meccanismo speciale per indicare la paternità tramite il tag rel. È equivalente a questo e può essere usato in modo intercambiabile.  - `bestRating`: Il valore più alto consentito in questo sistema di valutazione. Se bestRating è omesso, si assume 5.  - `dataProvider`: Una sequenza di caratteri che identifica il fornitore dell'entità di dati armonizzata.  - `dateCreated`: Timestamp di creazione dell'entità. Di solito viene assegnato dalla piattaforma di archiviazione.  - `dateModified`: Timestamp dell'ultima modifica dell'entità. Di solito viene assegnato dalla piattaforma di archiviazione.  - `description`: Descrizione dell'articolo  - `id`: Identificatore univoco dell'entità  - `legalName`: Il nome ufficiale dell'organizzazione, ad esempio la ragione sociale registrata.  - `location`: Riferimento geojson all'elemento. Può essere un punto, una stringa di linea, un poligono, un multi-punto, una stringa di linea o un poligono multiplo.  - `name`: Il nome di questo elemento.  - `owner`: Un elenco contenente una sequenza di caratteri codificata JSON che fa riferimento agli ID univoci dei proprietari.  - `reviewAspect`: Questa recensione o valutazione è pertinente a questa parte o aspetto dell'articoloRevisionato  - `seeAlso`: elenco di uri che puntano a risorse aggiuntive sull'elemento  - `source`: Una sequenza di caratteri che indica la fonte originale dei dati dell'entità come URL. Si consiglia di utilizzare il nome di dominio completamente qualificato del provider di origine o l'URL dell'oggetto di origine.  - `taxID`: Il codice fiscale dell'organizzazione o della persona, ad esempio il TIN negli Stati Uniti o il CIF/NIF in Spagna.  - `url`: URL che fornisce una descrizione o ulteriori informazioni su questo elemento.    
Proprietà richieste  
- `id`  - `type`  ## Modello di dati descrizione delle proprietà  
Ordinati in ordine alfabetico (clicca per i dettagli)  
<details><summary><strong>full yaml details</strong></summary>    
```yaml  
Organization:    
  description: 'An organization such as a school, NGO, corporation, club, etc, mapped from schema.org'    
  properties:    
    address:    
      description: 'The mailing address'    
      properties:    
        addressCountry:    
          description: 'Property. The country. For example, Spain. Model:''https://schema.org/addressCountry'''    
          type: string    
        addressLocality:    
          description: 'Property. The locality in which the street address is, and which is in the region. Model:''https://schema.org/addressLocality'''    
          type: string    
        addressRegion:    
          description: 'Property. The region in which the locality is, and which is in the country. Model:''https://schema.org/addressRegion'''    
          type: string    
        postOfficeBoxNumber:    
          description: 'Property. The post office box number for PO box addresses. For example, 03578. Model:''https://schema.org/postOfficeBoxNumber'''    
          type: string    
        postalCode:    
          description: 'Property. The postal code. For example, 24004. Model:''https://schema.org/https://schema.org/postalCode'''    
          type: string    
        streetAddress:    
          description: 'Property. The street address. Model:''https://schema.org/streetAddress'''    
          type: string    
      type: object    
      x-ngsi:    
        model: https://schema.org/address    
        type: Property    
    aggregateRating:    
      description: 'The average rating based on multiple ratings or reviews. Privacy:''low'''    
      properties:    
        itemReviewed:    
          anyOf:    
            - description: 'Property. Identifier format of any NGSI entity'    
              maxLength: 256    
              minLength: 1    
              pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
              type: string    
            - description: 'Property. Identifier format of any NGSI entity'    
              format: uri    
              type: string    
          description: 'Relationship. The item that is being reviewed/rated. '    
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
      description: 'An alternative name for this item'    
      type: string    
      x-ngsi:    
        type: Property    
    areaServed:    
      description: 'The geographic area where a service or offered item is provided'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    author:    
      description: 'The author of this content or rating. Please note that author is special in that HTML 5 provides a special mechanism for indicating authorship via the rel tag. That is equivalent to this and may be used interchangeably.'    
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
      description: 'A sequence of characters identifying the provider of the harmonised data entity.'    
      type: string    
      x-ngsi:    
        type: Property    
    dateCreated:    
      description: 'Entity creation timestamp. This will usually be allocated by the storage platform.'    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    dateModified:    
      description: 'Timestamp of the last modification of the entity. This will usually be allocated by the storage platform.'    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    description:    
      description: 'A description of this item'    
      type: string    
      x-ngsi:    
        type: Property    
    id:    
      anyOf: &organization_-_properties_-_owner_-_items_-_anyof    
        - description: 'Property. Identifier format of any NGSI entity'    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
        - description: 'Property. Identifier format of any NGSI entity'    
          format: uri    
          type: string    
      description: 'Unique identifier of the entity'    
      x-ngsi:    
        type: Property    
    legalName:    
      description: 'The official name of the organization, e.g. the registered company name.'    
      type: string    
      x-ngsi:    
        model: https://schema.org/legalName    
        type: Property    
    location:    
      description: 'Geojson reference to the item. It can be Point, LineString, Polygon, MultiPoint, MultiLineString or MultiPolygon'    
      oneOf:    
        - description: 'Geoproperty. Geojson reference to the item. Point'    
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
          title: 'GeoJSON Point'    
          type: object    
        - description: 'Geoproperty. Geojson reference to the item. LineString'    
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
          title: 'GeoJSON LineString'    
          type: object    
        - description: 'Geoproperty. Geojson reference to the item. Polygon'    
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
          title: 'GeoJSON Polygon'    
          type: object    
        - description: 'Geoproperty. Geojson reference to the item. MultiPoint'    
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
          title: 'GeoJSON MultiPoint'    
          type: object    
        - description: 'Geoproperty. Geojson reference to the item. MultiLineString'    
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
          title: 'GeoJSON MultiLineString'    
          type: object    
        - description: 'Geoproperty. Geojson reference to the item. MultiLineString'    
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
          title: 'GeoJSON MultiPolygon'    
          type: object    
      x-ngsi:    
        type: Geoproperty    
    name:    
      description: 'The name of this item.'    
      type: string    
      x-ngsi:    
        type: Property    
    owner:    
      description: 'A List containing a JSON encoded sequence of characters referencing the unique Ids of the owner(s)'    
      items:    
        anyOf: *organization_-_properties_-_owner_-_items_-_anyof    
        description: 'Property. Unique identifier of the entity'    
      type: array    
      x-ngsi:    
        type: Property    
    reviewAspect:    
      description: 'This Review or Rating is relevant to this part or facet of the itemReviewed'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    seeAlso:    
      description: 'list of uri pointing to additional resources about the item'    
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
      description: 'A sequence of characters giving the original source of the entity data as a URL. Recommended to be the fully qualified domain name of the source provider, or the URL to the source object.'    
      type: string    
      x-ngsi:    
        type: Property    
    taxID:    
      description: 'The Tax / Fiscal ID of the organization or person, e.g. the TIN in the US or the CIF/NIF in Spain.'    
      type: string    
      x-ngsi:    
        model: https://schema.org/taxID    
        type: Property    
    url:    
      description: 'URL which provides a description or further information about this item.'    
      format: uri    
      type: string    
      x-ngsi:    
        type: Property    
  required:    
    - id    
    - type    
  type: object    
  x-derived-from: https://schema.org/Organization    
  x-disclaimer: 'Redistribution and use in source and binary forms, with or without modification, are permitted  provided that the license conditions are met. Copyleft (c) 2021 Contributors to Smart Data Models Program'    
  x-license-url: https://github.com/smart-data-models/dataModel.Organization/blob/master/Organization/LICENSE.md    
  x-model-schema: https://smart-data-models.github.io/DataModel.Organization/Organization/schema.json    
  x-model-tags: ""    
  x-version: 0.0.2    
```  
</details>    
## Esempi di payload  
#### Organizzazione Valori chiave NGSI-v2 Esempio  
Ecco un esempio di Organizzazione in formato JSON-LD come valori-chiave. Questo è compatibile con NGSI-v2 quando si usa `options=keyValues` e restituisce i dati di contesto di una singola entità.  
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
#### Organizzazione NGSI-v2 normalizzata Esempio  
Ecco un esempio di Organizzazione in formato JSON-LD normalizzato. Questo è compatibile con NGSI-v2 quando non si utilizzano le opzioni e restituisce i dati di contesto di una singola entità.  
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
#### Organizzazione Valori chiave NGSI-LD Esempio  
Ecco un esempio di Organizzazione in formato JSON-LD come valori-chiave. Questo è compatibile con NGSI-LD quando si usa `options=keyValues` e restituisce i dati di contesto di una singola entità.  
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
  "taxID": "12345678900",  
  "@context": [  
    "https://smart-data-models.github.io/DataModel.Organization/context.jsonld"  
  ]  
}  
```  
#### Organizzazione NGSI-LD normalizzata Esempio  
Ecco un esempio di Organizzazione in formato JSON-LD normalizzato. Questo è compatibile con NGSI-LD quando non si utilizzano le opzioni e restituisce i dati di contesto di una singola entità.  
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
        49.40,  
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
    "https://smart-data-models.github.io/DataModel.Organization/context.jsonld"  
  ]  
}  
```  
Vedere [FAQ 10](https://smartdatamodels.org/index.php/faqs/) per ottenere una risposta su come gestire le unità di grandezza.  
