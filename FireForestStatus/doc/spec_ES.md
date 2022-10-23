<!-- 10-Header -->  
[![Smart Data Models](https://smartdatamodels.org/wp-content/uploads/2022/01/SmartDataModels_logo.png "Logo")](https://smartdatamodels.org)  
Entidad: FireForestStatus  
=========================<!-- /10-Header -->  
<!-- 15-License -->  
[Licencia abierta](https://github.com/smart-data-models//dataModel.Forestry/blob/master/FireForestStatus/LICENSE.md)  
[documento generado automáticamente](https://docs.google.com/presentation/d/e/2PACX-1vTs-Ng5dIAwkg91oTTUdt8ua7woBXhPnwavZ0FxgR8BsAI_Ek3C5q97Nd94HS8KhP-r_quD4H0fgyt3/pub?start=false&loop=false&delayms=3000#slide=id.gb715ace035_0_60)  
<!-- /15-License -->  
<!-- 20-Description -->  
Descripción global: **Esta entidad describe la posible presencia de humo y/o fuego en un bosque.**  
versión: 0.1.1  
<!-- /20-Description -->  
<!-- 30-PropertiesList -->  

## Lista de propiedades  

<sup><sub>[*] Si no hay un tipo en un atributo es porque puede tener varios tipos o diferentes formatos/patrones</sub></sup>  
- `address[object]`: La dirección postal  . Model: [https://schema.org/address](https://schema.org/address)- `alternateName[string]`: Un nombre alternativo para este artículo  - `areaServed[string]`: La zona geográfica en la que se presta un servicio o se ofrece un artículo  . Model: [https://schema.org/Text](https://schema.org/Text)- `dataProvider[string]`: Una secuencia de caracteres que identifica al proveedor de la entidad de datos armonizada.  - `dateCreated[string]`: Marca de tiempo de creación de la entidad. Suele ser asignada por la plataforma de almacenamiento.  - `dateModified[string]`: Marca de tiempo de la última modificación de la entidad. Normalmente será asignada por la plataforma de almacenamiento.  - `description[string]`: Una descripción de este artículo  - `dryLeavesDetected[number]`: Porcentaje de hojas secas detectadas  . Model: [https://schema.org/Number.](https://schema.org/Number.)- `fireDetected[boolean]`: Presencia de un incendio detectado por las cámaras.  . Model: [https://schema.org/Boolean](https://schema.org/Boolean)- `fireDetectedConfidence[number]`: Confianza en la detección de incendios mediante cámaras.  . Model: [https://schema.org/Number](https://schema.org/Number)- `fireForestDailyRiskIndex[number]`: Riesgo diario de incendio.  . Model: [https://schema.org/Number](https://schema.org/Number)- `fireRiskIndex[number]`: Índice de riesgo de incendio.  . Model: [https://schema.org/Number](https://schema.org/Number)- `fireWeatherIndex[number]`: Riesgo de incendio en función de las condiciones meteorológicas.  . Model: [https://schema.org/Number](https://schema.org/Number)- `greenLeavesDetected[number]`: Porcentaje de hojas verdes detectadas  . Model: [https://schema.org/Number.](https://schema.org/Number.)- `id[*]`: Identificador único de la entidad  - `litterCoverage[number]`: Porcentaje de superficie con restos  . Model: [https://schema.org/Number.](https://schema.org/Number.)- `location[*]`: Referencia Geojson al elemento. Puede ser Point, LineString, Polygon, MultiPoint, MultiLineString o MultiPolygon  - `name[string]`: El nombre de este artículo.  - `owner[array]`: Una lista que contiene una secuencia de caracteres codificada en JSON que hace referencia a los identificadores únicos de los propietarios  - `relativeHumidity[number]`: Humedad relativa un número entre 0 y 1 que representa el rango de 0% a 100%  . Model: [https://schema.org/Number](https://schema.org/Number)- `seeAlso[*]`: lista de uri que apuntan a recursos adicionales sobre el artículo  - `smokeDetected[boolean]`: Presencia de humo detectada por las cámaras.  . Model: [https://schema.org/Boolean](https://schema.org/Boolean)- `smokeDetectedConfidence[number]`: Confianza en la detección de humo mediante cámaras.  . Model: [https://schema.org/Number](https://schema.org/Number)- `soilTemperature[number]`: La temperatura del suelo observada en grados Celsius  . Model: [https://schema.org/Number](https://schema.org/Number)- `source[string]`: Una secuencia de caracteres que indica la fuente original de los datos de la entidad en forma de URL. Se recomienda que sea el nombre de dominio completo del proveedor de origen o la URL del objeto de origen.  - `type[string]`: Tipo de entidad NGSI. Tiene que ser FireForestStatus  <!-- /30-PropertiesList -->  
<!-- 35-RequiredProperties -->  
Propiedades requeridas  
- `id`  - `type`  <!-- /35-RequiredProperties -->  
<!-- 40-RequiredProperties -->  
<!-- /40-RequiredProperties -->  
<!-- 50-DataModelHeader -->  
## Descripción del modelo de datos de las propiedades  
Ordenados alfabéticamente (haga clic para ver los detalles)  
<!-- /50-DataModelHeader -->  
<!-- 60-ModelYaml -->  
<details><summary><strong>full yaml details</strong></summary>    
```yaml  
FireForestStatus:    
  description: 'This entity describes the possible presence of smoke and/or fire in a forest.'    
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
    dryLeavesDetected:    
      description: 'Percentage of dry leaves detected'    
      maximum: 1    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number.    
        type: Property    
    fireDetected:    
      description: 'Presence of a fire detected by cameras.'    
      type: boolean    
      x-ngsi:    
        model: https://schema.org/Boolean    
        type: Property    
    fireDetectedConfidence:    
      description: 'Confidence in fire detection by cameras.'    
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
      description: 'Risk of fire index.'    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
    fireWeatherIndex:    
      description: 'Risk of fire based on weather conditions.'    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
    greenLeavesDetected:    
      description: 'Percentage of green leaves detected'    
      maximum: 1    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number.    
        type: Property    
    id:    
      anyOf: &fireforeststatus_-_properties_-_owner_-_items_-_anyof    
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
    litterCoverage:    
      description: 'Percentage of surface with debris'    
      maximum: 1    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number.    
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
        anyOf: *fireforeststatus_-_properties_-_owner_-_items_-_anyof    
        description: 'Property. Unique identifier of the entity'    
      type: array    
      x-ngsi:    
        type: Property    
    relativeHumidity:    
      description: 'Relative Humidity a number between 0 and 1 representing the range of 0% to 100%'    
      maximum: 1    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
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
    smokeDetected:    
      description: 'Presence of smoke detected by cameras.'    
      type: boolean    
      x-ngsi:    
        model: https://schema.org/Boolean    
        type: Property    
    smokeDetectedConfidence:    
      description: 'Confidence in smoke detection by cameras.'    
      maximum: 1    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
    soilTemperature:    
      description: 'The observed soil temperature in Celsius degrees'    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
    source:    
      description: 'A sequence of characters giving the original source of the entity data as a URL. Recommended to be the fully qualified domain name of the source provider, or the URL to the source object.'    
      type: string    
      x-ngsi:    
        type: Property    
    type:    
      description: 'NGSI entity type. it has to be FireForestStatus'    
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
  x-disclaimer: 'Redistribution and use in source and binary forms, with or without modification, are permitted  provided that the license conditions are met. Copyleft (c) 2021 Contributors to Smart Data Models Program'    
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
## Ejemplo de carga útil  
#### FireForestStatus NGSI-v2 key-values Ejemplo  
Aquí hay un ejemplo de un FireForestStatus en formato JSON-LD como valores-clave. Esto es compatible con NGSI-v2 cuando se utiliza `options=keyValues` y devuelve los datos de contexto de una entidad individual.  
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
  "relativeHumidity": 0.70,  
  "soilTemperature": 25,  
  "greenLeavesDetected": 0.50,  
  "dryLeavesDetected": 0.20  
}  
```  
</details>  
#### FireForestStatus NGSI-v2 normalizado Ejemplo  
Aquí hay un ejemplo de un FireForestStatus en formato JSON-LD normalizado. Esto es compatible con NGSI-v2 cuando no se utilizan opciones y devuelve los datos de contexto de una entidad individual.  
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
    "type": "Array",  
    "value": [  
      "FireForestStatus.IPCZ.25073160",  
      "FireForestStatus.FPRB.78814414"  
    ]  
  },  
  "seeAlso": {  
    "type": "Array",  
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
    "type": "Number",  
    "value": 0  
  },  
  "fireForestDailyRiskIndex": {  
    "type": "Number",  
    "value": 1  
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
#### FireForestStatus NGSI-LD key-values Ejemplo  
Aquí hay un ejemplo de un FireForestStatus en formato JSON-LD como valores-clave. Esto es compatible con NGSI-LD cuando se utiliza `options=keyValues` y devuelve los datos de contexto de una entidad individual.  
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
#### FireForestStatus NGSI-LD normalizado Ejemplo  
Aquí hay un ejemplo de un FireForestStatus en formato JSON-LD normalizado. Esto es compatible con NGSI-LD cuando no se utilizan opciones y devuelve los datos de contexto de una entidad individual.  
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
Consulte [FAQ 10](https://smartdatamodels.org/index.php/faqs/) para obtener una respuesta sobre cómo tratar las unidades de magnitud  
<!-- /95-Units -->  
<!-- 97-LastFooter -->  
---  
[Smart Data Models](https://smartdatamodels.org) +++ [Contribution Manual](https://bit.ly/contribution_manual) +++ [About](https://bit.ly/Introduction_SDM)<!-- /97-LastFooter -->  
