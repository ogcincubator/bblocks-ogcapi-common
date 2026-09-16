# OGC API Common

Building blocks for OGC API - Common.


OGC API - Common is a multi-part standard that documents the set of common practices and 
shared requirements that have emerged from the development of Resource Oriented Architectures 
and Web APIs within the OGC. Standards developers will use these building-blocks in the 
construction of other OGC Standards that relate to Web APIs. The result is a modular suite 
of coherent API standards which can be adapted by a system designer for the unique requirements 
of their system. As such, this OGC API Standard serves as the "OWS Common" standard for 
resource-oriented OGC APIs. 

Consistent with the architecture of the Web, this specification uses a resource architecture 
that conforms to principles of Representational State Transfer (REST).

This OGC API Standard establishes a common pattern that is based on OpenAPI. 


## Building Blocks

### `ogc.api.common.part1.schemas.confClasses` — Conformance Classes schema

**Type:** schema

This building block corresponds to the schema for an OGC API Common confClasses

### `ogc.api.common.part1.schemas.exception` — Exception schema

**Type:** schema

This building block corresponds to the schema for an OGC API Common exception

### `ogc.api.common.part1.schemas.link` — Link schema

**Type:** schema

This building block corresponds to the schema for an OGC API Common link

### `ogc.api.common.part1.schemas.queryParamValueBoolean` — Boolean query parameter value

**Type:** datatype

The encoding of a boolean query parameter value: the lowercase strings "true" and "false".

### `ogc.api.common.part1.schemas.queryParamValueDecimal` — Decimal query parameter value

**Type:** datatype

The encoding of a decimal query parameter value: decimal digits separated by a period as a decimal indicator.

### `ogc.api.common.part1.schemas.queryParamValueDouble` — Double query parameter value

**Type:** datatype

The encoding of a double (exponential-format) query parameter value: a decimal mantissa followed, optionally, by an integer exponent.

### `ogc.api.common.part1.schemas.queryParamValueInteger` — Integer query parameter value

**Type:** datatype

The encoding of an integer query parameter value: a finite-length sequence of decimal digits with an optional leading negative sign.

### `ogc.api.common.part1.schemas.queryParamValueList` — Delimited list query parameter value

**Type:** datatype

The encoding of a query parameter value that is a delimited list of values, one of the two ways OGC API - Common allows passing more than one value for a parameter.

### `ogc.api.common.part1.responses.ConformanceDeclaration` — ConformanceDeclaration response

**Type:** response

The response for the OGC API conformance declaration resource.

### `ogc.api.common.part1.responses.Exception` — Exception response

**Type:** response

An RFC 7807 "Problem Details" error response, as recommended by OGC API - Common for any error situation.

### `ogc.api.common.part1.schemas.landingPage` — Landing Page schema

**Type:** schema

This building block corresponds to the schema for an OGC API Common landingPage

### `ogc.api.common.part1.paths.Conformance` — Conformance path

**Type:** path

The conformance declaration ("{root}/conformance"), listing the conformance classes implemented by this API.

### `ogc.api.common.part1.responses.LandingPage` — LandingPage response

**Type:** response

The response for the OGC API landing page resource.

### `ogc.api.common.part1.paths.LandingPage` — LandingPage path

**Type:** path

The OGC API landing page ("{root}/"), the single starting point for discovering the resources exposed by the API.

### `ogc.api.common.part1.api` — OGC API - Common

**Type:** api

OGC API - Common OpenAPI-based building block, combining the landing page, conformance declaration and API definition resources into a single OpenAPI document.

