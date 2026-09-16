
# Conformance Classes schema (Schema)

`ogc.api.common.part1.schemas.confClasses` *v0.1*

This building block corresponds to the schema for an OGC API Common confClasses

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
type: object
required:
- conformsTo
properties:
  conformsTo:
    type: array
    items:
      type: string
      example: http://www.opengis.net/spec/ogcapi-common-1/1.0/conf/core

```

Links to the schema:

* YAML version: [schema.yaml](https://raw.githubusercontent.com/ogcincubator/bblocks-ogcapi-common/undefined/build/annotated/api/common/part1/schemas/confClasses/schema.json)
* JSON version: [schema.json](https://raw.githubusercontent.com/ogcincubator/bblocks-ogcapi-common/undefined/build/annotated/api/common/part1/schemas/confClasses/schema.yaml)

## Sources

* [OGC API - Common - Part 1: Core](https://docs.ogc.org/is/19-072/19-072.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-ogcapi-common](https://github.com/ogcincubator/bblocks-ogcapi-common)
* Path: `_sources/part1/schemas/confClasses`

