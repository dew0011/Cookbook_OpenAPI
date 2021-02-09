# Cookbook_OpenAPI

OpenAPI 3.0 sepcification for a mock cookbook mini-API. 

Please feel free to view the documentation in your preferred OpenAPI renderer. Or open the yaml file in the Swagger online eidtor: https://swagger.io/tools/swagger-editor/ 

## Design Principles
This API holds recipes that are broken into summary, preparation and ingredient sections to allow quick loading of each section in the customers' applications as needed. In the API, customers can search the recipes, create new recipes [POST], update entire sections or individual items [PUT] or, likewise, [DELETE] items or individual sections, including the recipe as a whole. As most users will be accessing the API to perform a certain action, e.g. to search, create, update or delete, the API is structured by method rather than resource.

The documentation also refers to a theoretical second mini API, the ingredients API. This was kept seprate from this API as it contains immutable data on the nutition information of different food items and commerical food products. This also keeps the API design simple, which is appropraite for a simplistic theorectical application such as this.

## Tools

The software and tools used in creating this project:
- **Stoplight**: Here I outlined the basic struture and put in place reusable components, taking advantage of the GUI to streamline this process
- **Virtual Studio Code**: For bug fixes, adjustments of raw code and visualistion in Swagger and Redoc through the OpenAPI plugin
- **Redocly**: To extract the yaml file into separate files for easy editing in VSCode
