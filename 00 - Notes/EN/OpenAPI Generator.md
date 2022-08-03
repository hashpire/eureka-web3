---
version: "0.0.0"
published: true
---
uplinks::[OpenAPI](./OpenAPI.md)
tags:: #lang/en #type/tool
# OpenAPI Generator
A tool to generate clients, servers, and documentation from[OpenAPI](./OpenAPI.md)2.0/3.x documents

## Main Features
- More than 50+ client generators
	- Automatically generate and distribute clients as part of official SDKs
- More than 40+ server stub generators
	- Some support Inversion of Control
- Schema Generators
	- MySQL, GraphQL, protobuf
- Generate Documentation
	- HTML, Cwiki, Markdown
- Config Generators
	- Apache2 Configuration

## Installation
### npm
```bash
# install the latest version of "openapi-generator-cli"

npm install @openapitools/openapi-generator-cli -g

# use a specific version of "openapi-generator-cli"

openapi-generator-cli version-manager set 5.3.0
```

### Homebrew
```bash
brew install openapi-generator
```

## Usage
```bash
# Generate a ruby client from a valid petstore.yaml doc
openapi-generator-cli generate -i petstore.yaml -g ruby -o /tmp/test/
```
## See Also
1.[OpenAPI Generator vs Swagger Codegen](./OpenAPI%20Generator%20vs%20Swagger%20Codegen.md)

## References
1. https://openapi-generator.tech/
