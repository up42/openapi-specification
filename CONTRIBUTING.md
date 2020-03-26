# Contibuting to the UP42 OpenAPI specification

## Introduction

### Purpose

This document codifies the guidelines for contributing to the UP42
OpenAPI specification.

This document establishes the guidelines that contributors SHOULD
follow so that the  API is consistently documented.

### Recomended Reading

 1. [OpenAPI tutorial](https://idratherbewriting.com/learnapidoc/pubapis_openapi_tutorial_overview.html).
 2. [OpenAPI specification](https://swagger.io/docs/specification/about/).

###  Requirements language

The keywords "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT",
"SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this
document are to be interpreted as described in [RFC2119](https://www.ietf.org/rfc/rfc2119.txt).


### Titlecase usage

When describing paths or components MUST use **TitleCase**.

#### Example

```yaml
identifier: ThisOperationIdentifier
```

```yaml
$ref: '#/components/schemas/MySchemaNameInTitleCase'
```

### Describing request bodies and parameters

Care SHOULD be taken to not have inline request bodies and/or
parameters schemas or
examples. Unless they are extremely simple and can be described in a
couple of lines. If that is not the case, then you MUST use a
[component](https://swagger.io/docs/specification/components/). This
also allows for re-using it in other parts of the document.


### Describing responses

The above prescription for request bodies and/or parameters also
applies. Unless the response can fit in a couple of lines you MUST
use a [component](https://swagger.io/docs/specification/components/).

#### Example

```yaml
401:
  $ref: '#/components/responses/Unauthorized'
```
