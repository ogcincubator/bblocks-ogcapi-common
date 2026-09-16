
# ConformanceDeclaration response (Response)

`ogc.api.common.part1.responses.ConformanceDeclaration` *v0.1*

The response for the OGC API conformance declaration resource.

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
description: 'The URIs of all conformance classes supported by the server.

  To support "generic" clients that want to access multiple OGC API implementations
  - and not "just" a specific API / server, the server declares the conformance classes
  it implements and conforms to.'
content:
  application/json:
    schema:
      $ref: https://ogcincubator.github.io/bblocks-ogcapi-common/build/annotated/api/common/part1/schemas/confClasses/schema.yaml
    example:
      conformsTo:
      - http://www.opengis.net/spec/ogcapi-common-1/1.0/conf/core
  text/html:
    schema:
      type: string

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-ogcapi-common/build/annotated/api/common/part1/responses/ConformanceDeclaration/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-ogcapi-common/build/annotated/api/common/part1/responses/ConformanceDeclaration/schema.yaml)

## Sources

* [OGC API - Common - Part 1: Core](https://docs.ogc.org/is/19-072/19-072.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-ogcapi-common](https://github.com/ogcincubator/bblocks-ogcapi-common)
* Path: `_sources/part1/responses/ConformanceDeclaration`

