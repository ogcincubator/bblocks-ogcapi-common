
# Exception schema (Schema)

`ogc.api.common.part1.schemas.exception` *v0.1*

This building block corresponds to the schema for an OGC API Common exception

[*Status*](http://www.opengis.net/def/status): Under development

## Examples

### A resource-not-found error
#### json
```json
{
  "type": "http://www.opengis.net/def/exceptions/ogcapi-common-1/1.0/no-such-resource",
  "title": "Resource not found",
  "status": 404,
  "detail": "The requested collection does not exist on this server."
}

```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-ogcapi-common/build/annotated/api/common/part1/schemas/exception/context.jsonld",
  "type": "http://www.opengis.net/def/exceptions/ogcapi-common-1/1.0/no-such-resource",
  "title": "Resource not found",
  "status": 404,
  "detail": "The requested collection does not exist on this server."
}
```

#### ttl
```ttl
@prefix dct: <http://purl.org/dc/terms/> .
@prefix httpv: <http://www.w3.org/2011/http#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

[] a <http://www.opengis.net/def/exceptions/ogcapi-common-1/1.0/no-such-resource> ;
    dct:description "The requested collection does not exist on this server." ;
    dct:title "Resource not found" ;
    httpv:statusCodeNumber 404 .


```

## Schema

```yaml
title: Exception Schema
description: JSON schema for exceptions based on RFC 7807
type: object
required:
- type
properties:
  type:
    type: string
    x-jsonld-id: '@type'
  title:
    type: string
    x-jsonld-id: http://purl.org/dc/terms/title
  status:
    type: integer
    x-jsonld-id: http://www.w3.org/2011/http#statusCodeNumber
  detail:
    type: string
    x-jsonld-id: http://purl.org/dc/terms/description
  instance:
    type: string
    x-jsonld-id: '@id'
x-jsonld-prefixes:
  dct: http://purl.org/dc/terms/
  httpv: http://www.w3.org/2011/http#

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-ogcapi-common/build/annotated/api/common/part1/schemas/exception/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-ogcapi-common/build/annotated/api/common/part1/schemas/exception/schema.yaml)


# JSON-LD Context

```jsonld
{
  "@context": {
    "type": "@type",
    "title": "dct:title",
    "status": "httpv:statusCodeNumber",
    "detail": "dct:description",
    "instance": "@id",
    "dct": "http://purl.org/dc/terms/",
    "httpv": "http://www.w3.org/2011/http#",
    "@version": 1.1
  }
}
```

You can find the full JSON-LD context here:
[context.jsonld](https://ogcincubator.github.io/bblocks-ogcapi-common/build/annotated/api/common/part1/schemas/exception/context.jsonld)

## Sources

* [OGC API - Common - Part 1: Core](https://docs.ogc.org/is/19-072/19-072.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-ogcapi-common](https://github.com/ogcincubator/bblocks-ogcapi-common)
* Path: `_sources/part1/schemas/exception`

