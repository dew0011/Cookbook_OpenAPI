# Cookbook_OpenAPI

An OpenAPI 3.0 specification for a mock cookbook mini-API. 

The cookbook_openAPI outlines a REST API for developers to use to create, store and modify recipes in their application. 

## Usage

The YAML file can be viewed in the Swagger online editor: https://swagger.io/tools/swagger-editor/ or your preferred OpenAPI renderer. 

## Motivation
I created this documentation to get hands on experience in API documentation and explore REST API structure. This is a work in progress and is evolving as I learn more. 

If you are also exploring this space, please feel free to use this as a starting place. There are many, many places where this documentation and the underlying API structure could be improved and built on. At the bottom I have given a list of some of the [fantastic resources](##Thank_you) I have used in putting this documentation together. 

## Design Principles
### Endpoint layout
The cookbook_openAPI holds recipes that are broken into three broad resources: recipe (the summary or meta data of the recipe), preparation and ingredients. The premise is that this allows rapid loading of each section in the customers' applications, as they do not have to pull the whole recipe at once. This also permits more flexibility in how the data is displayed.

Following this natural structure, the API endpoints have been tagged so that they are grouped together by resource in the rendered documentation. 

### Keeping it small
The documentation also refers to a theoretical second mini-API, the Ingredients API. This API was not incorporated into the cookbook_OpenAPI as it contains immutable data on the nutrition information of different food items and commercial food products. This also keeps the API design simple, which is appropriate for a simplistic theoretical application such as this.

## Tools
I used various tools in creating this documentation:
- **Stoplight**: Here I outlined the basic structure and put in place reusable components, taking advantage of the GUI to streamline this process
- **Virtual Studio Code**: For bug fixes, adjustments of raw code and visualisation of the rendered document in both Swagger and Redoc through the OpenAPI plugin
- **Redocly**: To extract the YAML file into separate files for easy editing in VSCode

## Thank you
I used many resources in creating this project. Here are some notable mentions:
- An invaluable guide and tutorial on documenting APIs: https://idratherbewriting.com/learnapidoc/
- A great overview of README.md docs best practices &#128521; : https://www.welcometothejungle.com/en/articles/btc-readme-documentation-best-practices 
- A clear explanation of the core terminology: https://medium.com/bunq-developers-corner/the-difference-between-resources-endpoints-objects-and-items-in-the-bunq-api-documentation-6b774473542


### Resources
- https://spec.commonmark.org
- https://httpstatuses.com/
- https://yaml-multiline.info/


### Specification guidelines
I looked at a number of these. They offer different examples and terminology, which is useful in navigating new concepts. 
- https://spec.openapis.org/oas/v3.0.3
- https://opensource.zalando.com/restful-api-guidelines
- https://swagger.io/docs/specification/about/ 






