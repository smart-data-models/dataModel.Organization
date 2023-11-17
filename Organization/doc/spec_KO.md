<!-- 10-Header -->    
[![Smart Data Models](https://smartdatamodels.org/wp-content/uploads/2022/01/SmartDataModels_logo.png "Logo")](https://smartdatamodels.org)    
엔티티: 조직    
=======<!-- /10-Header -->    
<!-- 15-License -->    
[오픈 라이선스](https://github.com/smart-data-models//dataModel.Organization/blob/master/Organization/LICENSE.md)    
[문서 자동 생성](https://docs.google.com/presentation/d/e/2PACX-1vTs-Ng5dIAwkg91oTTUdt8ua7woBXhPnwavZ0FxgR8BsAI_Ek3C5q97Nd94HS8KhP-r_quD4H0fgyt3/pub?start=false&loop=false&delayms=3000#slide=id.gb715ace035_0_60)    
<!-- /15-License -->    
<!-- 20-Description -->    
글로벌 설명: **학교, NGO, 기업, 동호회 등의 조직으로, schema.org에서 매핑**됨    
버전: 0.0.3    
<!-- /20-Description -->    
<!-- 30-PropertiesList -->    
## 속성 목록    
<sup><sub>[*] 속성에 유형이 없는 것은 여러 유형 또는 다른 형식/패턴을 가질 수 있기 때문입니다</sub></sup>.    
- `address[object]`: 우편 주소  . Model: [https://schema.org/address](https://schema.org/address)	- `addressCountry[string]`: 국가. 예를 들어, 스페인  . Model: [https://schema.org/addressCountry](https://schema.org/addressCountry)    
	- `addressLocality[string]`: 도로명 주소가 있는 지역 및 해당 지역에 속한 지역  . Model: [https://schema.org/addressLocality](https://schema.org/addressLocality)    
	- `addressRegion[string]`: 해당 지역이 위치한 지역과 해당 국가의 지역  . Model: [https://schema.org/addressRegion](https://schema.org/addressRegion)    
	- `district[string]`: 지구는 일부 국가에서는 지방 정부에서 관리하는 행정 구역의 일종입니다.      
	- `postOfficeBoxNumber[string]`: 사서함 주소의 우체국 사서함 번호입니다. 예: 03578  . Model: [https://schema.org/postOfficeBoxNumber](https://schema.org/postOfficeBoxNumber)    
	- `postalCode[string]`: 우편 번호입니다. 예: 24004  . Model: [https://schema.org/https://schema.org/postalCode](https://schema.org/https://schema.org/postalCode)    
	- `streetAddress[string]`: 거리 주소  . Model: [https://schema.org/streetAddress](https://schema.org/streetAddress)    
	- `streetNr[string]`: 공공 도로의 특정 건물을 식별하는 번호      
- `aggregateRating[object]`: 여러 평점 또는 리뷰를 기반으로 한 평균 평점입니다. 프라이버시:'낮음'  	- `itemReviewed[*]`: 검토/평가 중인 항목입니다.      
	- `ratingCount`:       
	- `reviewCount`:       
- `alternateName[string]`: 이 항목의 대체 이름  - `areaServed[string]`: 서비스 또는 제공 품목이 제공되는 지리적 영역  . Model: [https://schema.org/Text](https://schema.org/Text)- `author[uri]`: 이 콘텐츠 또는 평점의 작성자입니다. 저자는 HTML 5에서 rel 태그를 통해 저자를 표시하는 특별한 메커니즘을 제공한다는 점에서 특별하다는 점에 유의하세요. 이는 다음과 동일하며 서로 바꿔서 사용할 수 있습니다.  . Model: [https://schema.org/URL](https://schema.org/URL)- `bestRating[number]`: 이 평점 시스템에서 허용되는 최고 값입니다. bestRating을 생략하면 5가 가정됩니다.  . Model: [https://schema.org/Number](https://schema.org/Number)- `dataProvider[string]`: 조화된 데이터 엔티티의 공급자를 식별하는 일련의 문자  - `dateCreated[date-time]`: 엔티티 생성 타임스탬프. 이는 일반적으로 스토리지 플랫폼에서 할당합니다.  - `dateModified[date-time]`: 엔티티의 마지막 수정 타임스탬프입니다. 이는 일반적으로 스토리지 플랫폼에서 할당합니다.  - `description[string]`: 이 항목에 대한 설명  - `id[*]`: 엔티티의 고유 식별자  - `legalName[string]`: 조직의 공식 이름(예: 등록된 회사명)  . Model: [https://schema.org/legalName](https://schema.org/legalName)- `location[*]`: 항목에 대한 지오숀 참조입니다. 포인트, 라인 문자열, 다각형, 멀티포인트, 멀티라인 문자열 또는 멀티폴리곤일 수 있습니다.  - `name[string]`: 이 항목의 이름  - `owner[array]`: 소유자의 고유 ID를 참조하는 JSON 인코딩된 문자 시퀀스가 포함된 목록입니다.  - `reviewAspect[string]`: 이 리뷰 또는 평가는 항목의 이 부분 또는 측면과 관련이 있습니다.  . Model: [https://schema.org/Text](https://schema.org/Text)- `seeAlso[*]`: 항목에 대한 추가 리소스를 가리키는 URL 목록  - `source[string]`: 엔티티 데이터의 원본 소스를 URL로 제공하는 문자 시퀀스입니다. 소스 공급자의 정규화된 도메인 이름 또는 소스 개체에 대한 URL을 사용하는 것이 좋습니다.  - `taxID[string]`: 조직 또는 개인의 세금/재정 ID(예: 미국의 경우 TIN, 스페인의 경우 CIF/NIF)  . Model: [https://schema.org/taxID](https://schema.org/taxID)- `type[string]`: NGSI 엔티티 유형. 조직이어야 합니다.  - `url[uri]`: 이 항목에 대한 설명이나 추가 정보를 제공하는 URL입니다.  <!-- /30-PropertiesList -->    
<!-- 35-RequiredProperties -->    
필수 속성    
- `id`  - `type`  <!-- /35-RequiredProperties -->    
<!-- 40-RequiredProperties -->    
<!-- /40-RequiredProperties -->    
<!-- 50-DataModelHeader -->    
## 속성에 대한 데이터 모델 설명    
알파벳순으로 정렬(자세한 내용을 보려면 클릭)    
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
## 페이로드 예시    
#### 조직 NGSI-v2 키 값 예제    
다음은 키-값으로 JSON-LD 형식의 조직 예제입니다. 이는 `옵션=키값`을 사용할 때 NGSI-v2와 호환되며 개별 엔티티의 컨텍스트 데이터를 반환합니다.    
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
  "taxID": "12345678900"  
}  
```  
</details>    
#### 조직 NGSI-v2 정규화 예제    
다음은 정규화된 JSON-LD 형식의 조직 예시입니다. 이는 옵션을 사용하지 않을 때 NGSI-v2와 호환되며 개별 엔티티의 컨텍스트 데이터를 반환합니다.    
<details><summary><strong>show/hide example</strong></summary>      
```json  
{  
  "id": "urn:ngsi-ld:Organization:34f91f29-aadd-45f7-ab9e-4fca2baffdd7",  
  "type": "Organization",  
  "dateCreated": {  
    "type": "DateTime",  
    "value": "2022-06-21T08:24:35.905712+02:00"  
  },  
  "dateModified": {  
    "type": "DateTime",  
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
        49.4,  
        8.68  
      ]  
    }  
  },  
  "address": {  
    "type": "StructuredValue",  
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
    "type": "Text",  
    "value": "https://www.example-organization-homepage.com"  
  },  
  "legalName": {  
    "type": "Text",  
    "value": "Beispielname GmbH"  
  },  
  "taxID": {  
    "type": "Text",  
    "value": "12345678900"  
  }  
}  
```  
</details>    
#### 조직 NGSI-LD 키 값 예제    
다음은 키-값으로 JSON-LD 형식의 조직 예제입니다. 이는 `옵션=키값`을 사용할 때 NGSI-LD와 호환되며 개별 엔티티의 컨텍스트 데이터를 반환합니다.    
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
#### 조직 NGSI-LD 정규화 예제    
다음은 정규화된 JSON-LD 형식의 조직 예시입니다. 이는 옵션을 사용하지 않을 때 NGSI-LD와 호환되며 개별 엔티티의 컨텍스트 데이터를 반환합니다.    
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
[FAQ 10](https://smartdatamodels.org/index.php/faqs/)을 참조하여 규모 단위를 다루는 방법에 대한 답변을 확인하세요.    
<!-- /95-Units -->    
<!-- 97-LastFooter -->    
---    
[Smart Data Models](https://smartdatamodels.org) +++ [Contribution Manual](https://bit.ly/contribution_manual) +++ [About](https://bit.ly/Introduction_SDM)<!-- /97-LastFooter -->    
