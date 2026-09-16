
# Link schema (Schema)

`ogc.api.common.part1.schemas.link` *v0.1*

This building block corresponds to the schema for an OGC API Common link

[*Status*](http://www.opengis.net/def/status): Under development

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
  rel:
    type: string
    description: The type or semantics of the relation.
    example: alternate
  type:
    type: string
    description: A hint indicating what the media type of the result of dereferencing
      the link should be.
    example: application/geo+json
  hreflang:
    type: string
    description: A hint indicating what the language of the result of dereferencing
      the link should be.
    example: en
  title:
    type: string
    description: Used to label the destination of a link such that it can be used
      as a human-readable identifier.
    example: Trierer Strasse 70, 53115 Bonn
  length:
    type: integer

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-ogcapi-common/build/annotated/api/common/part1/schemas/link/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-ogcapi-common/build/annotated/api/common/part1/schemas/link/schema.yaml)

## Sources

* [OGC API - Common - Part 1: Core](https://docs.ogc.org/is/19-072/19-072.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-ogcapi-common](https://github.com/ogcincubator/bblocks-ogcapi-common)
* Path: `_sources/part1/schemas/link`

