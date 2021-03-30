# UP42 OpenAPI specification

## Introduction

This repository contains the [UP42](https://up42.com)
[OpenAPI](https://swagger.io/specification/) specification.

The specification follows the API development. It reflects the current
state of the API. It is a continous work in progress since the API
will change over time and the specification follows it.

## Operations

### View locally

You'll need to install Docker for this.

Run the following command:

```
docker run -it --rm -p 8080:80 \
  -v $(pwd)/:/usr/share/nginx/html/swagger/ \
  -e SPEC_URL=swagger/openapi.yaml redocly/redoc
```

This will serve the API definition locally at http://localhost:8080/ .

## Creating issues and contributing

The specification is completely open and hence if you find any issue
with it please do at least one of the following things:

 1. Open an issue here.
 2. Mail <mailto:support@up42.com> and/or come and chat with us at
    [gitter support chat room ](https://gitter.im/up42-com/support).
    
Pull requests are very much welcomed and you will be given credit for
your contribution. After all in github all commits get assigned to the
commiter.

## License

Since this is documentation the license is the
[Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](http://creativecommons.org/licenses/by-nc-nd/4.0/).

