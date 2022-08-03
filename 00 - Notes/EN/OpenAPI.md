---
version: "0.0.0"
published: true
---
uplinks::[API](./API.md)
tags:: #lang/en #type/term 
# OpenAPI
- An [API specification](https://github.com/OAI/OpenAPI-Specification) (description format) for REST APIs
- Forrmerly known as[Swagger](./Swagger.md)Specification
- Used to describe
	- Available endpoints and its operations — `POST /users`
	- Operation parameters — Input and Output
	- Authentication methods
	- Contact information, license, ToS, etc.

## Structure
- Written in[YAML](./YAML.md)or[JSON](./JSON.md)
- All keyword names are case-sensitive.
- [Basic Structure](https://swagger.io/docs/specification/basic-structure/)
	- Metadata
		- Title
		- Description
		- Version —[Semantic Versioning](./Semantic Versioning.md)
	- Servers — API Server Base Url
	- Paths — API endpoints
		- Parameters
		- Request Body
		- Responses
	- Components — Define common data structures used in API
		- Prevent duplication
		- Reference via `$ref` whenever a `schema` is required
	- Authentication
		- HTTP Authentication — Basic, Bearer
		- API key
		- OAuth 2
		- OpenID

## Why use OpenAPI ?
Tools to ease the development of APIs
- [Swagger Editor](https://editor.swagger.io/) — browser-based editor to help write OpenAPI specs — e.g. autocompletion
- [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) to **generate a server stub and client libraries** for your API
- [Swagger UI](https://github.com/swagger-api/swagger-ui)to generate **interactive API documentation** that kets users try out API calls in browser
- Connect to other API-related tools
	- [SoapUI](https://soapui.org/) to create automated tests
	- [Open Source Tools](https://swagger.io/tools/open-source/open-source-integrations/)
	- [Commercial Tools](https://swagger.io/commercial-tools/)
## References
- https://swagger.io/docs/specification/about/
- https://support.smartbear.com/swaggerhub/docs/tutorials/openapi-3-tutorial.html


