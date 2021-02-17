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

Or try it out in Postman: [![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/28e76c71be48476b5a6b)
