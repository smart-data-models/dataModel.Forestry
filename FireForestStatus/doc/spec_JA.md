<!-- 10-Header -->    
[![Smart Data Models](https://smartdatamodels.org/wp-content/uploads/2022/01/SmartDataModels_logo.png "Logo")](https://smartdatamodels.org)    
エンティティFireForestStatus    
======================<!-- /10-Header -->    
<!-- 15-License -->    
[オープン・ライセンス](https://github.com/smart-data-models//dataModel.Forestry/blob/master/FireForestStatus/LICENSE.md)    
[文書は自動的に生成される](https://docs.google.com/presentation/d/e/2PACX-1vTs-Ng5dIAwkg91oTTUdt8ua7woBXhPnwavZ0FxgR8BsAI_Ek3C5q97Nd94HS8KhP-r_quD4H0fgyt3/pub?start=false&loop=false&delayms=3000#slide=id.gb715ace035_0_60)    
<!-- /15-License -->    
<!-- 20-Description -->    
グローバル記述**このエンティティは、森林における煙および/または火災の存在の可能性を記述する。    
バージョン: 0.1.1    
<!-- /20-Description -->    
<!-- 30-PropertiesList -->    
## プロパティのリスト    
<sup><sub>[*] 属性に型がない場合は、複数の型があるか、異なるフォーマット/パターンがある可能性があるためです</sub></sup>。    
- `address[object]`: 郵送先住所  . Model: [https://schema.org/address](https://schema.org/address)	- `addressCountry[string]`: 国。例えば、スペイン  . Model: [https://schema.org/addressCountry](https://schema.org/addressCountry)    
	- `addressLocality[string]`: 番地がある地域と、その地域に含まれる地域  . Model: [https://schema.org/addressLocality](https://schema.org/addressLocality)    
	- `addressRegion[string]`: その地域がある地域、またその国がある地域  . Model: [https://schema.org/addressRegion](https://schema.org/addressRegion)    
	- `district[string]`: 地区とは行政区画の一種で、国によっては地方自治体によって管理されている。      
	- `postOfficeBoxNumber[string]`: 私書箱の住所のための私書箱番号。例：03578  . Model: [https://schema.org/postOfficeBoxNumber](https://schema.org/postOfficeBoxNumber)    
	- `postalCode[string]`: 郵便番号。例：24004  . Model: [https://schema.org/https://schema.org/postalCode](https://schema.org/https://schema.org/postalCode)    
	- `streetAddress[string]`: 番地  . Model: [https://schema.org/streetAddress](https://schema.org/streetAddress)    
- `alternateName[string]`: この項目の別名  - `areaServed[string]`: サービスまたは提供品が提供される地理的地域  . Model: [https://schema.org/Text](https://schema.org/Text)- `dataProvider[string]`: ハーモナイズされたデータ・エンティティの提供者を識別する一連の文字。  - `dateCreated[date-time]`: エンティティの作成タイムスタンプ。これは通常、ストレージプラットフォームによって割り当てられます。  - `dateModified[date-time]`: エンティティの最終変更のタイムスタンプ。これは通常、ストレージプラットフォームによって割り当てられる。  - `description[string]`: この商品の説明  - `dryLeavesDetected[number]`: 検出された乾燥葉の割合  . Model: [https://schema.org/Number](https://schema.org/Number)- `fireDetected[boolean]`: カメラが検知した火災の有無  . Model: [https://schema.org/Boolean](https://schema.org/Boolean)- `fireDetectedConfidence[number]`: カメラによる火災検知の信頼性  . Model: [https://schema.org/Number](https://schema.org/Number)- `fireForestDailyRiskIndex[number]`: 日常的な火災のリスク。  . Model: [https://schema.org/Number](https://schema.org/Number)- `fireRiskIndex[number]`: 火災リスク指数  . Model: [https://schema.org/Number](https://schema.org/Number)- `fireWeatherIndex[number]`: 気象条件に基づく火災のリスク  . Model: [https://schema.org/Number](https://schema.org/Number)- `greenLeavesDetected[number]`: 検出された緑葉の割合  . Model: [https://schema.org/Number](https://schema.org/Number)- `id[*]`: エンティティの一意識別子  - `litterCoverage[number]`: 破片のある表面の割合  . Model: [https://schema.org/Number](https://schema.org/Number)- `location[*]`: アイテムへの Geojson 参照。Point、LineString、Polygon、MultiPoint、MultiLineString、MultiPolygon のいずれか。  - `name[string]`: このアイテムの名前  - `owner[array]`: 所有者の固有IDを参照するJSONエンコードされた文字列を含むリスト。  - `relativeHumidity[number]`: 相対湿度 0%～100%の範囲を表す0～1の数値。  . Model: [https://schema.org/Number](https://schema.org/Number)- `seeAlso[*]`: アイテムに関する追加リソースを指すURIのリスト  - `smokeDetected[boolean]`: カメラが検知した煙の有無  . Model: [https://schema.org/Boolean](https://schema.org/Boolean)- `smokeDetectedConfidence[number]`: カメラによる煙検知の信頼性  . Model: [https://schema.org/Number](https://schema.org/Number)- `soilTemperature[number]`: 観測された土壌温度（摂氏  . Model: [https://schema.org/Number](https://schema.org/Number)- `source[string]`: エンティティ・データの元のソースを URL として示す一連の文字。ソース・プロバイダの完全修飾ドメイン名、またはソース・オブジェクトの URL を推奨する。  - `type[string]`: NGSIのエンティティタイプは、FireForestStatusでなければならない。  <!-- /30-PropertiesList -->    
<!-- 35-RequiredProperties -->    
必須プロパティ    
- `id`  - `type`  <!-- /35-RequiredProperties -->    
<!-- 40-RequiredProperties -->    
<!-- /40-RequiredProperties -->    
<!-- 50-DataModelHeader -->    
## プロパティのデータモデル記述    
アルファベット順（クリックで詳細表示）    
<!-- /50-DataModelHeader -->    
<!-- 60-ModelYaml -->    
<details><summary><strong>full yaml details</strong></summary>      
```yaml    
FireForestStatus:      
  description: This entity describes the possible presence of smoke and/or fire in a forest.      
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
    dryLeavesDetected:      
      description: Percentage of dry leaves detected      
      maximum: 1      
      minimum: 0      
      type: number      
      x-ngsi:      
        model: https://schema.org/Number      
        type: Property      
    fireDetected:      
      description: Presence of a fire detected by cameras      
      type: boolean      
      x-ngsi:      
        model: https://schema.org/Boolean      
        type: Property      
    fireDetectedConfidence:      
      description: Confidence in fire detection by cameras      
      maximum: 1      
      minimum: 0      
      type: number      
      x-ngsi:      
        model: https://schema.org/Number      
        type: Property      
    fireForestDailyRiskIndex:      
      description: 'Daily risk of fire. '      
      minimum: 0      
      type: number      
      x-ngsi:      
        model: https://schema.org/Number      
        type: Property      
    fireRiskIndex:      
      description: Risk of fire index      
      minimum: 0      
      type: number      
      x-ngsi:      
        model: https://schema.org/Number      
        type: Property      
    fireWeatherIndex:      
      description: Risk of fire based on weather conditions      
      minimum: 0      
      type: number      
      x-ngsi:      
        model: https://schema.org/Number      
        type: Property      
    greenLeavesDetected:      
      description: Percentage of green leaves detected      
      maximum: 1      
      minimum: 0      
      type: number      
      x-ngsi:      
        model: https://schema.org/Number      
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
    litterCoverage:      
      description: Percentage of surface with debris      
      maximum: 1      
      minimum: 0      
      type: number      
      x-ngsi:      
        model: https://schema.org/Number      
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
    relativeHumidity:      
      description: Relative Humidity a number between 0 and 1 representing the range of 0% to 100%      
      maximum: 1      
      minimum: 0      
      type: number      
      x-ngsi:      
        model: https://schema.org/Number      
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
    smokeDetected:      
      description: Presence of smoke detected by cameras      
      type: boolean      
      x-ngsi:      
        model: https://schema.org/Boolean      
        type: Property      
    smokeDetectedConfidence:      
      description: Confidence in smoke detection by cameras      
      maximum: 1      
      minimum: 0      
      type: number      
      x-ngsi:      
        model: https://schema.org/Number      
        type: Property      
    soilTemperature:      
      description: The observed soil temperature in Celsius degrees      
      type: number      
      x-ngsi:      
        model: https://schema.org/Number      
        type: Property      
    source:      
      description: 'A sequence of characters giving the original source of the entity data as a URL. Recommended to be the fully qualified domain name of the source provider, or the URL to the source object'      
      type: string      
      x-ngsi:      
        type: Property      
    type:      
      description: NGSI entity type. it has to be FireForestStatus      
      enum:      
        - FireForestStatus      
      type: string      
      x-ngsi:      
        type: Property      
  required:      
    - id      
    - type      
  type: object      
  x-derived-from: ""      
  x-disclaimer: 'Redistribution and use in source and binary forms, with or without modification, are permitted  provided that the license conditions are met. Copyleft (c) 2022 Contributors to Smart Data Models Program'      
  x-license-url: https://github.com/smart-data-models/dataModel.Forestry/blob/master/FireForestStatus/LICENSE.md      
  x-model-schema: https://smart-data-models.github.io/dataModel.Forestry/FireForestStatus/schema.json      
  x-model-tags: ""      
  x-version: 0.1.1      
```    
</details>      
<!-- /60-ModelYaml -->    
<!-- 70-MiddleNotes -->    
<!-- /70-MiddleNotes -->    
<!-- 80-Examples -->    
## ペイロードの例    
#### FireForestStatus NGSI-v2 キー値の例    
以下はFireForestStatusをJSON-LD形式でkey-valuesとした例である。これはNGSI-v2と互換性があり、`options=keyValues`を使用すると、個々のエンティティのコンテキストデータを返す。    
<details><summary><strong>show/hide example</strong></summary>      
```json  
{  
  "id": "FireForestStatus-South-1",  
  "type": "FireForestStatus",  
  "dateObserved": "2021-02-24T00:00:00Z",  
  "location": {  
    "type": "Point",  
    "coordinates": [  
      42.206302,  
      -7.887465  
    ]  
  },  
  "name": "Ourense Forest - South",  
  "description": "Status of the Ourense Forest (south)",  
  "refDevice": {  
    "type": "Relationship",  
    "object": [  
      "ground-humidity-sensor:1"  
    ]  
  },  
  "smokeDetected": false,  
  "smokeDetectedConfidence": 0.9,  
  "fireDetected": false,  
  "fireDetectedConfidence": 0.8,  
  "fireRiskIndex": 0.1,  
  "litterCoverage": 0.6,  
  "relativeHumidity": 0.7,  
  "soilTemperature": 25,  
  "greenLeavesDetected": 0.5,  
  "dryLeavesDetected": 0.2  
}  
```  
</details>    
#### FireForestStatus NGSI-v2 正規化例    
以下は、正規化された JSON-LD 形式の FireForestStatus の例である。これはNGSI-v2と互換性があり、オプションを使用しない場合、個々のエンティティのコンテキストデータを返します。    
<details><summary><strong>show/hide example</strong></summary>      
```json  
{  
  "id": "FireForestStatus.id.JPEX.39548913",  
  "type": "FireForestStatus",  
  "dateCreated": {  
    "type": "DateTime",  
    "value": "2011-04-09T04:07:43Z"  
  },  
  "dateModified": {  
    "type": "DateTime",  
    "value": "2011-04-09T04:07:43Z"  
  },  
  "source": {  
    "type": "Text",  
    "value": ""  
  },  
  "name": {  
    "type": "Text",  
    "value": "Ourense Forest - South"  
  },  
  "alternateName": {  
    "type": "Text",  
    "value": "Ourense Forest - South"  
  },  
  "description": {  
    "type": "Text",  
    "value": "Status of the Ourense Forest (south)"  
  },  
  "dataProvider": {  
    "type": "Text",  
    "value": ""  
  },  
  "owner": {  
    "type": "StructuredValue",  
    "value": [  
      "FireForestStatus.IPCZ.25073160",  
      "FireForestStatus.FPRB.78814414"  
    ]  
  },  
  "seeAlso": {  
    "type": "StructuredValue",  
    "value": [  
      "FireForestStatus.XZGT.71938385",  
      "FireForestStatus.GBWU:95431484"  
    ]  
  },  
  "location": {  
    "type": "geo:json",  
    "value": {  
      "type": "Point",  
      "coordinates": [  
        42.206302,  
        -7.887465  
      ]  
    }  
  },  
  "address": {  
    "type": "StructuredValue",  
    "value": {  
      "streetAddress": "",  
      "addressLocality": "Ourense",  
      "addressRegion": "Galicia",  
      "addressCountry": "ES",  
      "postalCode": "",  
      "postOfficeBoxNumber": "",  
      "areaServed": ""  
    }  
  },  
  "areaServed": {  
    "type": "Text",  
    "value": ""  
  },  
  "smokeDetected": {  
    "type": "Boolean",  
    "value": false  
  },  
  "smokeDetectedConfidence": {  
    "type": "Number",  
    "value": 0.9  
  },  
  "fireDetected": {  
    "type": "Boolean",  
    "value": false  
  },  
  "fireDetectedConfidence": {  
    "type": "Number",  
    "value": 0.8  
  },  
  "fireRiskIndex": {  
    "type": "Number",  
    "value": 0.1  
  },  
  "fireWeatherIndex ": {  
    "type": "Boolean",  
    "value": false  
  },  
  "fireForestDailyRiskIndex": {  
    "type": "Boolean",  
    "value": true  
  },  
  "litterCoverage": {  
    "type": "Number",  
    "value": 0.6  
  },  
  "relativeHumidity": {  
    "type": "Number",  
    "value": 0.7  
  },  
  "soilTemperature": {  
    "type": "Number",  
    "value": 25  
  },  
  "greenLeavesDetected": {  
    "type": "Number",  
    "value": 0.5  
  },  
  "dryLeavesDetected": {  
    "type": "Number",  
    "value": 0.2  
  }  
}  
```  
</details>    
#### FireForestStatus NGSI-LD キー値の例    
以下はFireForestStatusをJSON-LD形式でkey-valuesとした例である。これは NGSI-LD と互換性があり、`options=keyValues` を使うと個々のエンティティのコンテキストデータを返す。    
<details><summary><strong>show/hide example</strong></summary>      
```json  
{  
  "id": "urn:ngsi-ld:FireForestStatus:FireForestStatus-South-1",  
  "type": "FireForestStatus",  
  "dateObserved": "2021-02-24T00:00:00Z",  
  "description": "Status of the Ourense Forest (south)",  
  "dryLeavesDetected": 0.2,  
  "fireDetected": false,  
  "fireDetectedConfidence": 0.8,  
  "fireRiskIndex": 0.1,  
  "greenLeavesDetected": 0.5,  
  "litterCoverage": 0.6,  
  "location": {  
    "type": "Point",  
    "coordinates": [  
      42.206302,  
      -7.887465  
    ]  
  },  
  "name": "Ourense Forest - South",  
  "refDevice": [  
    "urn:ngsi-ld:Device:ground-humidity-sensor-1"  
  ],  
  "relativeHumidity": 0.7,  
  "smokeDetected": false,  
  "smokeDetectedConfidence": 0.9,  
  "soilTemperature": 25,  
  "@context": [  
    "https://uri.etsi.org/ngsi-ld/v1/ngsi-ld-core-context.jsonld",  
    "https://raw.githubusercontent.com/smart-data-models/dataModel.Forestry/master/context.jsonld"  
  ]  
}  
```  
</details>    
#### FireForestStatus NGSI-LD 正規化例    
以下は、正規化された JSON-LD 形式の FireForestStatus の例である。これは、オプションを使用しない場合のNGSI-LDと互換性があり、個々のエンティティのコンテキストデータを返します。    
<details><summary><strong>show/hide example</strong></summary>      
```json  
{  
    "id": "urn:ngsi-ld:FireForestStatus:id:JPEX:39548913",  
    "type": "FireForestStatus",  
    "address": {  
        "type": "Property",  
        "value": {  
            "streetAddress": "",  
            "addressLocality": "Ourense",  
            "addressRegion": "Galicia",  
            "addressCountry": "ES",  
            "postalCode": "",  
            "postOfficeBoxNumber": "",  
            "areaServed": ""  
        }  
    },  
    "alternateName": {  
        "type": "Property",  
        "value": "Ourense Forest - South"  
    },  
    "areaServed": {  
        "type": "Property",  
        "value": ""  
    },  
    "dataProvider": {  
        "type": "Property",  
        "value": ""  
    },  
    "dateCreated": {  
        "type": "Property",  
        "value": {  
            "@type": "DateTime",  
            "@value": "2011-04-09T04:07:43Z"  
        }  
    },  
    "dateModified": {  
        "type": "Property",  
        "value": {  
            "@type": "DateTime",  
            "@value": "2011-04-09T04:07:43Z"  
        }  
    },  
    "description": {  
        "type": "Property",  
        "value": "Status of the Ourense Forest (south)"  
    },  
    "dryLeavesDetected": {  
        "type": "Property",  
        "value": 0.2  
    },  
    "fireDetected": {  
        "type": "Property",  
        "value": false  
    },  
    "fireDetectedConfidence": {  
        "type": "Property",  
        "value": 0.8  
    },  
    "fireForestDailyRiskIndex": {  
        "type": "Property",  
        "value": 864.6  
    },  
    "fireRiskIndex": {  
        "type": "Property",  
        "value": 0.1  
    },  
    "fireWeatherIndex ": {  
        "type": "Property",  
        "value": 864.6  
    },  
    "greenLeavesDetected": {  
        "type": "Property",  
        "value": 0.5  
    },  
    "litterCoverage": {  
        "type": "Property",  
        "value": 0.6  
    },  
    "location": {  
        "type": "Property",  
        "value": {  
            "type": "Point",  
            "coordinates": [  
                42.206302,  
                -7.887465  
            ]  
        }  
    },  
    "name": {  
        "type": "Property",  
        "value": "Ourense Forest - South"  
    },  
    "owner": {  
        "type": "Property",  
        "value": [  
            "urn:ngsi-ld:FireForestStatus:items:IPCZ:25073160",  
            "urn:ngsi-ld:FireForestStatus:items:FPRB:78814414"  
        ]  
    },  
    "relativeHumidity": {  
        "type": "Property",  
        "value": 0.7  
    },  
    "seeAlso": {  
        "type": "Property",  
        "value": [  
            "urn:ngsi-ld:FireForestStatus:items:XZGT:71938385",  
            "urn:ngsi-ld:FireForestStatus:items:GBWU:95431484"  
        ]  
    },  
    "smokeDetected": {  
        "type": "Property",  
        "value": false  
    },  
    "smokeDetectedConfidence": {  
        "type": "Property",  
        "value": 0.9  
    },  
    "soilTemperature": {  
        "type": "Property",  
        "value": 25  
    },  
    "source": {  
        "type": "Property",  
        "value": ""  
    },  
    "@context": [  
        "https://uri.etsi.org/ngsi-ld/v1/ngsi-ld-core-context.jsonld",  
        "https://raw.githubusercontent.com/smart-data-models/dataModel.Forestry/master/context.jsonld"  
    ]  
}  
```  
</details><!-- /80-Examples -->    
<!-- 90-FooterNotes -->    
<!-- /90-FooterNotes -->    
<!-- 95-Units -->    
マグニチュード単位の扱い方については、[FAQ 10](https://smartdatamodels.org/index.php/faqs/)を参照のこと。    
<!-- /95-Units -->    
<!-- 97-LastFooter -->    
---    
[Smart Data Models](https://smartdatamodels.org) +++ [Contribution Manual](https://bit.ly/contribution_manual) +++ [About](https://bit.ly/Introduction_SDM)<!-- /97-LastFooter -->    
