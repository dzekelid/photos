{
  "info": {
    "name": "Flickr Get Favorite Context",
    "_postman_id": "22524165-8b2e-4401-aca7-21088f102ecb",
    "description": "Returns next and previous favorites for a photo in a user's favorites",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "photos",
      "item": [
        {
          "id": "7a7302e9-21b5-4dcd-9280-413152d07f35",
          "name": "getFavoritesContextByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.favorites.getContext?api_key=%7B%7D&photo_id=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns next and previous favorites for a photo in a user's favorites"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f9741eb-8126-4bbb-9a32-5e6a1cb63985"
            }
          ]
        }
      ]
    }
  ]
}