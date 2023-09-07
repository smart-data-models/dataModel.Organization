<!-- 10-Header -->  
[![Smart Data Models](https://smartdatamodels.org/wp-content/uploads/2022/01/SmartDataModels_logo.png "Logo")](https://smartdatamodels.org)  
实体：组织  
=====<!-- /10-Header -->  
<!-- 15-License -->  
[开放许可](https://github.com/smart-data-models//dataModel.Organization/blob/master/Organization/LICENSE.md)  
[文件自动生成](https://docs.google.com/presentation/d/e/2PACX-1vTs-Ng5dIAwkg91oTTUdt8ua7woBXhPnwavZ0FxgR8BsAI_Ek3C5q97Nd94HS8KhP-r_quD4H0fgyt3/pub?start=false&loop=false&delayms=3000#slide=id.gb715ace035_0_60)  
<!-- /15-License -->  
<!-- 20-Description -->  
全局描述：**一个组织，如学校、非政府组织、公司、俱乐部等，由 schema.org 映射**。  
版本： 0.0.3  
<!-- /20-Description -->  
<!-- 30-PropertiesList -->  

## 属性列表  

<sup><sub>[*] 如果属性中没有类型，是因为它可能有多个类型或不同的格式/模式</sub></sup>。  
- `address[object]`: 邮寄地址  . Model: [https://schema.org/address](https://schema.org/address)	- `addressCountry[string]`: 国家。例如，西班牙  . Model: [https://schema.org/addressCountry](https://schema.org/addressCountry)  
	- `addressLocality[string]`: 街道地址所在的地点，以及该地点所在的区域  . Model: [https://schema.org/addressLocality](https://schema.org/addressLocality)  
	- `addressRegion[string]`: 地点所在的地区，以及该地区位于哪个国家  . Model: [https://schema.org/addressRegion](https://schema.org/addressRegion)  
	- `district[string]`: 地区是一种行政区划，在一些国家由地方政府管理    
	- `postOfficeBoxNumber[string]`: 用于邮政信箱地址的邮政信箱号码。例如：03578  . Model: [https://schema.org/postOfficeBoxNumber](https://schema.org/postOfficeBoxNumber)  
	- `postalCode[string]`: 邮政编码。例如：24004  . Model: [https://schema.org/https://schema.org/postalCode](https://schema.org/https://schema.org/postalCode)  
	- `streetAddress[string]`: 街道地址  . Model: [https://schema.org/streetAddress](https://schema.org/streetAddress)  
- `aggregateRating[object]`: 基于多个评分或评论的平均评分。隐私:'低  	- `itemReviewed[*]`: 正在审查/评级的项目。    
	- `ratingCount`:     
- `alternateName[string]`: 该项目的替代名称  - `areaServed[string]`: 提供服务或提供物品的地理区域  . Model: [https://schema.org/Text](https://schema.org/Text)- `author[uri]`: 该内容或评级的作者。请注意，"作者 "的特殊性在于 HTML 5 提供了一种特殊机制，通过 rel 标签来表示作者身份。这等同于此，可交替使用  . Model: [https://schema.org/URL](https://schema.org/URL)- `bestRating[number]`: 该评级系统允许的最高值。如果省略 bestRating，则假定为 5。  . Model: [https://schema.org/Number](https://schema.org/Number)- `dataProvider[string]`: 标识统一数据实体提供者的字符序列  - `dateCreated[date-time]`: 实体创建时间戳。通常由存储平台分配  - `dateModified[date-time]`: 实体最后一次修改的时间戳。通常由存储平台分配  - `description[string]`: 项目描述  - `id[*]`: 实体的唯一标识符  - `legalName[string]`: 组织的正式名称，如注册公司名称  . Model: [https://schema.org/legalName](https://schema.org/legalName)- `location[*]`: 项目的 Geojson 引用。它可以是点、线条字符串、多边形、多点、多线条字符串或多多边形  - `name[string]`: 该项目的名称  - `owner[array]`: 包含一个 JSON 编码字符序列的列表，其中引用了所有者的唯一 Ids  - `reviewAspect[string]`: 此评论或评级与项目的此部分或方面相关已评论  . Model: [https://schema.org/Text](https://schema.org/Text)- `seeAlso[*]`: 指向有关该项目的其他资源的 uri 列表  - `source[string]`: 以 URL 形式给出实体数据原始来源的字符串。建议使用源提供者的完全合格域名或源对象的 URL  - `taxID[string]`: 组织或个人的税务/财政 ID，例如美国的 TIN 或西班牙的 CIF/NIF  . Model: [https://schema.org/taxID](https://schema.org/taxID)- `type[string]`: NGSI 实体类型。必须是组织  - `url[uri]`: 提供有关此项目的描述或更多信息的 URL  <!-- /30-PropertiesList -->  
<!-- 35-RequiredProperties -->  
所需属性  
- `id`  - `type`  <!-- /35-RequiredProperties -->  
<!-- 40-RequiredProperties -->  
<!-- /40-RequiredProperties -->  
<!-- 50-DataModelHeader -->  
## 属性的数据模型描述  
按字母顺序排列（点击查看详情）  
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
## 有效载荷示例  
#### 组织 NGSI-v2 密钥值示例  
下面是一个以 JSON-LD 格式作为键值的组织示例。当使用 `options=keyValues` 时，这与 NGSI-v2 兼容，并返回单个实体的上下文数据。  
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
#### 组织 NGSI-v2 标准化示例  
下面是一个规范化 JSON-LD 格式的 "组织 "示例。在不使用选项的情况下，它与 NGSI-v2 兼容，并返回单个实体的上下文数据。  
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
#### 组织 NGSI-LD 键值示例  
下面是一个以 JSON-LD 格式作为键值的组织示例。当使用 `options=keyValues` 时，它与 NGSI-LD 兼容，并返回单个实体的上下文数据。  
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
#### 组织 NGSI-LD 标准化示例  
下面是一个规范化 JSON-LD 格式的 "组织 "示例。在不使用选项时，它与 NGSI-LD 兼容，并返回单个实体的上下文数据。  
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
请参阅 [FAQ 10](https://smartdatamodels.org/index.php/faqs/)，获取如何处理幅度单位的答案。  
<!-- /95-Units -->  
<!-- 97-LastFooter -->  
---  
[Smart Data Models](https://smartdatamodels.org) +++ [Contribution Manual](https://bit.ly/contribution_manual) +++ [About](https://bit.ly/Introduction_SDM)<!-- /97-LastFooter -->  
