
# Decimal query parameter value (Datatype)

`ogc.api.common.part1.schemas.queryParamValueDecimal` *v0.1*

The encoding of a decimal query parameter value: decimal digits separated by a period as a decimal indicator.

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: Decimal query parameter value
description: Decimal values SHALL be represented by a finite-length sequence of decimal
  digits separated by a period as a decimal indicator. An optional leading negative
  ("-") sign is allowed (positive, "+", is assumed if omitted). Leading and trailing
  zeroes are optional, and if the fractional part is zero, the period and following
  zero(es) can be omitted.
type: number

```

Links to the schema:

* YAML version: [schema.yaml](https://raw.githubusercontent.com/ogcincubator/bblocks-ogcapi-common/undefined/build/annotated/api/common/part1/schemas/queryParamValueDecimal/schema.json)
* JSON version: [schema.json](https://raw.githubusercontent.com/ogcincubator/bblocks-ogcapi-common/undefined/build/annotated/api/common/part1/schemas/queryParamValueDecimal/schema.yaml)

## Sources

* [OGC API - Common - Part 1: Core, Requirement /req/core/query-param-value-decimal](https://docs.ogc.org/is/19-072/19-072.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-ogcapi-common](https://github.com/ogcincubator/bblocks-ogcapi-common)
* Path: `_sources/part1/schemas/queryParamValueDecimal`

