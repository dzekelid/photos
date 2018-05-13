{
  "info": {
    "name": "Flickr Get Favorite List",
    "_postman_id": "028ecff2-568e-4254-b601-dc2460ca9448",
    "description": "Returns a list of the user's favorite photos. Only photos which the calling user has permission to see are returned.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "photos",
      "item": [
        {
          "id": "5d007b48-38cf-4bdd-a0fb-f3e86ea587b0",
          "name": "getFavoritesByPersonID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.favorites.getList?api_key=%7B%7D&max_fave_date=%7B%7D&min_fave_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the user's favorite photos"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b81d59d7-9b55-4ea5-a0f0-530c1ec30bad"
            }
          ]
        }
      ]
    }
  ]
}