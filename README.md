# The OpenAPI Specification | 开放API规范

---

### 中文翻译进行中，欢迎大家协助翻译
https://github.com/fishead/OpenAPI-Specification

##### 翻译进度
- [x] [Definitions](versions/3.0.0.zhCN.md#definitions)
	- [x] [OpenAPI Document](versions/3.0.0.zhCN.md#oasDocument)
	- [x] [Path Templating](versions/3.0.0.zhCN.md#pathTemplating)
	- [x] [Media Types](versions/3.0.0.zhCN.md#mediaTypes)
	- [x] [HTTP Status Codes](versions/3.0.0.zhCN.md#httpCodes)
- [x] [Specification](versions/3.0.0.zhCN.md#specification)
	- [x] [Versions](versions/3.0.0.zhCN.md#versions)
	- [x] [Format](versions/3.0.0.zhCN.md#format)
	- [x] [Document Structure](versions/3.0.0.zhCN.md#documentStructure)
	- [x] [Data Types](versions/3.0.0.zhCN.md#dataTypes)
	- [x] [Rich Text Formatting](versions/3.0.0.zhCN.md#richText)
	- [x] [Relative References In URLs](versions/3.0.0.zhCN.md#relativeReferences)
	- [ ] [Schema](versions/3.0.0.zhCN.md#schema)
		- [x] [OpenAPI Object](versions/3.0.0.zhCN.md#oasObject)
		- [x] [Info Object](versions/3.0.0.zhCN.md#infoObject)
		- [x] [Contact Object](versions/3.0.0.zhCN.md#contactObject)
		- [x] [License Object](versions/3.0.0.zhCN.md#licenseObject)
		- [x] [Server Object](versions/3.0.0.zhCN.md#serverObject)
		- [x] [Server Variable Object](versions/3.0.0.zhCN.md#serverVariableObject)
		- [x] [Components Object](versions/3.0.0.zhCN.md#componentsObject)
		- [x] [Paths Object](versions/3.0.0.zhCN.md#pathsObject)
		- [x] [Path Item Object](versions/3.0.0.zhCN.md#pathItemObject)
		- [x] [Operation Object](versions/3.0.0.zhCN.md#operationObject)
		- [x] [External Documentation Object](versions/3.0.0.zhCN.md#externalDocumentationObject)
		- [x] [Parameter Object](versions/3.0.0.zhCN.md#parameterObject)
		- [x] [Request Body Object](versions/3.0.0.zhCN.md#requestBodyObject)
		- [x] [Media Type Object](versions/3.0.0.zhCN.md#mediaTypeObject)
		- [x] [Encoding Object](versions/3.0.0.zhCN.md#encodingObject)
		- [x] [Responses Object](versions/3.0.0.zhCN.md#responsesObject)
		- [x] [Response Object](versions/3.0.0.zhCN.md#responseObject)
		- [x] [Callback Object](versions/3.0.0.zhCN.md#callbackObject)
		- [x] [Example Object](versions/3.0.0.zhCN.md#exampleObject)
		- [ ] [Link Object](versions/3.0.0.zhCN.md#linkObject)
		- [x] [Header Object](versions/3.0.0.zhCN.md#headerObject)
		- [ ] [Tag Object](versions/3.0.0.zhCN.md#tagObject)
		- [ ] [Reference Object](versions/3.0.0.zhCN.md#referenceObject)
		- [ ] [Schema Object](versions/3.0.0.zhCN.md#schemaObject)
		- [ ] [Discriminator Object](versions/3.0.0.zhCN.md#discriminatorObject)
		- [x] [XML Object](versions/3.0.0.zhCN.md#xmlObject)
		- [x] [Security Scheme Object](versions/3.0.0.zhCN.md#securitySchemeObject)
		- [x] [OAuth Flows Object](versions/3.0.0.zhCN.md#oauthFlowsObject)
		- [x] [OAuth Flow Object](versions/3.0.0.zhCN.md#oauthFlowObject)
		- [ ] [Security Requirement Object](versions/3.0.0.zhCN.md#securityRequirementObject)
	- [x] [Specification Extensions](versions/3.0.0.zhCN.md#specificationExtensions)
	- [ ] [Security Filtering](versions/3.0.0.zhCN.md#securityFiltering)
- [ ] [Appendix A: Revision History](versions/3.0.0.zhCN.md#revisionHistory)


---

[![Build Status](https://travis-ci.org/OAI/OpenAPI-Specification.svg?branch=master)](https://travis-ci.org/OAI/OpenAPI-Specification)

![](https://avatars3.githubusercontent.com/u/16343502?v=3&s=200)

The OpenAPI Specification is a community-driven open specification within the [OpenAPI Initiative](https://www.openapis.org/), a Linux Foundation Collaborative Project.

The OpenAPI Specification (OAS) defines a standard, programming language-agnostic interface description for [REST APIs](https://en.wikipedia.org/wiki/Representational_state_transfer), which allows both humans and computers to discover and understand the capabilities of a service without requiring access to source code, additional documentation, or inspection of network traffic. When properly defined via OpenAPI, a consumer can understand and interact with the remote service with a minimal amount of implementation logic. Similar to what interface descriptions have done for lower-level programming, the OpenAPI Specification removes guesswork in calling a service.

Use cases for machine-readable API definition documents include, but are not limited to: interactive documentation; code generation for documentation, clients, and servers; and automation of test cases. OpenAPI documents describe an API's services and are represented in either YAML or JSON formats. These documents may either be produced and served statically or be generated dynamically from an application.

The OpenAPI Specification does not require rewriting existing APIs. It does not require binding any software to a service — the service being described may not even be owned by the creator of its description. It does, however, require the capabilities of the service be described in the structure of the OpenAPI Specification. Not all services can be described by OpenAPI — this specification is not intended to cover every possible style of REST APIs. The OpenAPI Specification does not mandate a specific development process such as design-first or code-first. It does facilitate either technique by establishing clear interactions with a REST API.

This GitHub project is the starting point for OpenAPI. Here you will find the information you need about the OpenAPI Specification, simple examples of what it looks like, and some general information regarding the project.

## Current Version - 3.0.3

The current version of the OpenAPI specification is [OpenAPI Specification 3.0.3](versions/3.0.3.md).

### Future Versions

[3.1.0](https://github.com/OAI/OpenAPI-Specification/tree/v3.1.0-dev) - The next MINOR version. Non-breaking changes should be submitted against this branch.

### Previous Versions

This repository also contains the [OpenAPI Specification 2.0](versions/2.0.md), which is identical to the Swagger 2.0 specification before it was renamed to "OpenAPI Specification", as well as the Swagger 1.2 and Swagger 2.0 specifications.

Each folder in this repository, such as [examples](examples) and [schemas](schemas), should contain folders pertaining to the current and previous versions of the specification.

## See It in Action

If you just want to see it work, check out the [list of current examples](examples/v3.0).

## Tools and Libraries

Looking to see how you can create your own OpenAPI definition, present it, or otherwise use it? Check out the growing
[list of 3.0 implementations](IMPLEMENTATIONS.md).

## Participation

The current process for development of the OpenAPI Specification is described in
[Development Guidelines](DEVELOPMENT.md).
Development of the next version of the OpenAPI Specification is guided by the [Technical Steering Committee (TSC)](https://www.openapis.org/participate/how-to-contribute/governance#TDC). This group of committers bring their API expertise, incorporate feedback from the community, and expand the group of committers as appropriate. All development activity on the future specification will be performed as features and merged into this branch. Upon release of the future specification, this branch will be merged to master.

The TSC holds weekly web conferences to review open pull requests and discuss open issues related to the evolving OpenAPI Specification. Participation in weekly calls and scheduled working sessions is open to the community. You can view the [TSC calendar online](https://openapi.groups.io/g/tsc/calendar), and import it to your calendar using the [iCal link](https://openapi.groups.io/g/tsc/ics/1105671/1995679554/feed.ics).

The OpenAPI Initiative encourages participation from individuals and companies alike. If you want to participate in the evolution of the OpenAPI Specification, consider taking the following actions:

* Review the [current specification](versions/3.0.3.md). The human-readable markdown file _is the source of truth_ for the specification.
* Review the [development](DEVELOPMENT.md) process so you understand how the spec is evolving.
* Check the [issues](https://github.com/OAI/OpenAPI-Specification/issues) and [pull requests](https://github.com/OAI/OpenAPI-Specification/pulls) to see if someone has already documented your idea or feedback on the specification. You can follow an existing conversation by subscribing to the existing issue or PR.
* Create an issue to describe a new concern. If possible, propose a solution.

Not all feedback can be accommodated and there may be solid arguments for or against a change being appropriate for the specification.

## Licensing

See: [License (Apache-2.0)](https://github.com/OAI/OpenAPI-Specification/blob/master/LICENSE)

![Analytics](https://ga-beacon.appspot.com/UA-831873-42/readme.md?pixel)
