
# Delimited list query parameter value (Datatype)

`ogc.api.common.part1.schemas.queryParamValueList` *v0.1*

The encoding of a query parameter value that is a delimited list of values, one of the two ways OGC API - Common allows passing more than one value for a parameter.

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: Delimited list query parameter value
description: 'A parameter value list encoded as a parameter name followed by a delimited
  list of values (as opposed to repeated name:value pairs for each value in the list).
  Parameter values containing lists SHOULD specify the delimiter to be used in the
  API definition; the default list item delimiter SHALL be the comma (","). Any list
  item value that includes a space or comma SHALL escape that character using the
  URI encoding rules from IETF RFC 3986. All empty entries SHALL be represented by
  the empty string - two successive commas indicate an empty item, as does a leading
  or trailing comma.

  Extend this datatype with a specific "items" schema (e.g. via "allOf") to constrain
  the type of the individual list values.'
type: array
items: {}

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-ogcapi-common/build/annotated/api/common/part1/schemas/queryParamValueList/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-ogcapi-common/build/annotated/api/common/part1/schemas/queryParamValueList/schema.yaml)

## Sources

* [OGC API - Common - Part 1: Core, Requirements /req/core/query-param-list-delimiter, /req/core/query-param-list-escape, /req/core/query-param-list-empty](https://docs.ogc.org/is/19-072/19-072.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-ogcapi-common](https://github.com/ogcincubator/bblocks-ogcapi-common)
* Path: `_sources/part1/schemas/queryParamValueList`

