
# Link schema (Schema)

`ogc.api.common.part1.schemas.link` *v0.1*

This building block corresponds to the schema for an OGC API Common link

[*Status*](http://www.opengis.net/def/status): Under development

## Examples

### A link to an alternate representation
A link to a GeoJSON representation of the same resource.

#### json
```json
{
  "href": "http://data.example.com/buildings/123.json",
  "rel": "alternate",
  "type": "application/geo+json",
  "title": "This document as GeoJSON"
}

```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-ogcapi-common/build/annotated/api/common/part1/schemas/link/context.jsonld",
  "href": "http://data.example.com/buildings/123.json",
  "rel": "alternate",
  "type": "application/geo+json",
  "title": "This document as GeoJSON"
}
```

#### ttl
```ttl
@prefix dct: <http://purl.org/dc/terms/> .
@prefix ns1: <http://www.iana.org/assignments/> .
@prefix oa: <http://www.w3.org/ns/oa#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .

[] rdfs:label "This document as GeoJSON" ;
    dct:type "application/geo+json" ;
    ns1:relation <http://www.iana.org/assignments/relation/alternate> ;
    oa:hasTarget <http://data.example.com/buildings/123.json> .


```

## Schema

```yaml
type: object
required:
- href
- rel
properties:
  href:
    type: string
    description: Supplies the URI to a remote resource (or resource fragment).
    example: http://data.example.com/buildings/123
    x-jsonld-id: http://www.w3.org/ns/oa#hasTarget
    x-jsonld-type: '@id'
  rel:
    type: string
    description: The type or semantics of the relation.
    example: alternate
    x-jsonld-id: http://www.iana.org/assignments/relation
    x-jsonld-type: '@id'
    x-jsonld-base: http://www.iana.org/assignments/relation/
  type:
    type: string
    description: A hint indicating what the media type of the result of dereferencing
      the link should be.
    example: application/geo+json
    x-jsonld-id: http://purl.org/dc/terms/type
  hreflang:
    type: string
    description: A hint indicating what the language of the result of dereferencing
      the link should be.
    example: en
    x-jsonld-id: http://purl.org/dc/terms/language
  title:
    type: string
    description: Used to label the destination of a link such that it can be used
      as a human-readable identifier.
    example: Trierer Strasse 70, 53115 Bonn
    x-jsonld-id: http://www.w3.org/2000/01/rdf-schema#label
  length:
    type: integer
    x-jsonld-id: http://purl.org/dc/terms/extent
x-jsonld-prefixes:
  oa: http://www.w3.org/ns/oa#
  dct: http://purl.org/dc/terms/
  rdfs: http://www.w3.org/2000/01/rdf-schema#

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-ogcapi-common/build/annotated/api/common/part1/schemas/link/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-ogcapi-common/build/annotated/api/common/part1/schemas/link/schema.yaml)


# JSON-LD Context

```jsonld
{
  "@context": {
    "href": {
      "@id": "oa:hasTarget",
      "@type": "@id"
    },
    "rel": {
      "@context": {
        "@base": "http://www.iana.org/assignments/relation/"
      },
      "@id": "http://www.iana.org/assignments/relation",
      "@type": "@id"
    },
    "type": "dct:type",
    "hreflang": "dct:language",
    "title": "rdfs:label",
    "length": "dct:extent",
    "oa": "http://www.w3.org/ns/oa#",
    "dct": "http://purl.org/dc/terms/",
    "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
    "@version": 1.1
  }
}
```

You can find the full JSON-LD context here:
[context.jsonld](https://ogcincubator.github.io/bblocks-ogcapi-common/build/annotated/api/common/part1/schemas/link/context.jsonld)

## Sources

* [OGC API - Common - Part 1: Core](https://docs.ogc.org/is/19-072/19-072.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-ogcapi-common](https://github.com/ogcincubator/bblocks-ogcapi-common)
* Path: `_sources/part1/schemas/link`

