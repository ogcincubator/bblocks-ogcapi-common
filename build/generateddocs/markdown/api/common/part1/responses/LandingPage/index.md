
# LandingPage response (Response)

`ogc.api.common.part1.responses.LandingPage` *v0.1*

The response for the OGC API landing page resource.

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
description: The landing page provides links to the API definition (link relations
  `service-desc` and `service-doc`), the Conformance declaration (path `/conformance`,
  link relation `http://www.opengis.net/def/rel/ogc/1.0/conformance`), and to other
  resources.
content:
  application/json:
    schema:
      $ref: https://raw.githubusercontent.com/ogcincubator/bblocks-ogcapi-common/undefined/build/annotated/api/common/part1/schemas/landingPage/schema.yaml
  text/html:
    schema:
      type: string

```

Links to the schema:

* YAML version: [schema.yaml](https://raw.githubusercontent.com/ogcincubator/bblocks-ogcapi-common/undefined/build/annotated/api/common/part1/responses/LandingPage/schema.json)
* JSON version: [schema.json](https://raw.githubusercontent.com/ogcincubator/bblocks-ogcapi-common/undefined/build/annotated/api/common/part1/responses/LandingPage/schema.yaml)

## Sources

* [OGC API - Common - Part 1: Core](https://docs.ogc.org/is/19-072/19-072.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-ogcapi-common](https://github.com/ogcincubator/bblocks-ogcapi-common)
* Path: `_sources/part1/responses/LandingPage`

