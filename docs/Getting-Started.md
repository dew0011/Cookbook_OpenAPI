# Getting-Started

Instructions on how to get started using the cookbook mini-API.

## Structure

The API has three main endpoints.
- `/recipes` for searching the database or adding new recipes to the database
- `/recipes/ingredients` to modify the ingredients of a recipe
- `recipes/preparation` to modify the preparation steps needed for a recipe

## Your first request - Searching the database

Feeling hungry? Us too. For our first request, let's try searching the API for recipes that use bananas. We will use the `/recipes` endpoint.

Here is the example of the curl request.
```bash
curl http://localhost:3000/recipes?ingredients='banana'
```

Alternatively, you may navigate to the [endpoint documentation](../reference/Cookbook-OpenAPI.v1.yaml) and 'Try it out' in the GUI.


