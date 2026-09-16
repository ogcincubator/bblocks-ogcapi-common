
# Double query parameter value (Datatype)

`ogc.api.common.part1.schemas.queryParamValueDouble` *v0.1*

The encoding of a double (exponential-format) query parameter value: a decimal mantissa followed, optionally, by an integer exponent.

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: Double query parameter value
description: 'Double values SHALL be represented by a mantissa followed, optionally,
  by the character "e", followed by an exponent. The exponent SHALL be an integer.
  The mantissa SHALL be a decimal number, following the same lexical rules as a decimal
  query parameter value. If "e" and the exponent are omitted, an exponent value of
  0 is assumed.

  Recommendation /rec/core/query-param-value-special: the special values positive
  and negative infinity and not-a-number SHOULD be represented using the strings "inf",
  "-inf" and "nan" respectively, where supported.'
type: number

```

Links to the schema:

* YAML version: [schema.yaml](https://raw.githubusercontent.com/ogcincubator/bblocks-ogcapi-common/undefined/build/annotated/api/common/part1/schemas/queryParamValueDouble/schema.json)
* JSON version: [schema.json](https://raw.githubusercontent.com/ogcincubator/bblocks-ogcapi-common/undefined/build/annotated/api/common/part1/schemas/queryParamValueDouble/schema.yaml)

## Sources

* [OGC API - Common - Part 1: Core, Requirement /req/core/query-param-value-double](https://docs.ogc.org/is/19-072/19-072.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-ogcapi-common](https://github.com/ogcincubator/bblocks-ogcapi-common)
* Path: `_sources/part1/schemas/queryParamValueDouble`

