# elasticsearchdocs


GET /products1/_search
{
    "query" : {
        "term" : { "Sku":"147648" }
    }
}


GET products1/_search
{
  "query": {
    "terms": {
      "_id": [ "5295", "3" ] 
    }
  }
}



//delete the item
POST products1/_delete_by_query
{
  "query": {
    "term" : { "Sku":"147648" }
  }
}
