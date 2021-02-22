#  Cookbook Open-API Specification

This mini-API gives you access to our database of recipes and lets you or your users create and curate your own collection. 

## The API has three main endpoints.

- [**/recipes**](recipes-page) to search the database or add new recipes
- [**/recipes/ingredients**](ingredients-page) to access the ingredients of a recipe
- [**/recipes/preparation**](preparation-page) to access the preparation steps of a recipe

All of our endpoints can be tested in Postman: <br>
[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/28e76c71be48476b5a6b)

## Getting started - Searching the database

If you are familiar with Postman or prefer using a GUI try out the below exercises in Postman: <br>
[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/28e76c71be48476b5a6b)

Feeling hungry? Us too. For our first request, let's try searching the API for recipes that use yoghurt. We will use the **/recipes** endpoint.

```bash
curl http://localhost:3000/recipes?ingredients='yoghurt'
```
Above we wrote 'yoghurt' but you can also spell this as 'yogurt'. We can use grep terms to return results for multiple spelling variants.
```bash
curl http://localhost:3000/recipes?ingredients='yog.*urt'
```

[Explore the API -> ](redoc.html)