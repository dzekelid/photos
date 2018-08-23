{
  "info": {
    "name": "Flickr Get Group Pools",
    "_postman_id": "bfec42e1-60ab-4acd-be2d-d43250fad344",
    "description": "Returns next and previous photos for a photo in a group pool",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "photos",
      "item": [
        {
          "id": "38487ce8-570d-43b2-8ed2-083ed8bf6702",
          "name": "getGroupPhotosByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.groups.pools.getContext?api_key=%7B%7D&group_id=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns next and previous photos for a photo in a group pool"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "273a89cd-7c04-495c-b022-6d32be7caa4a"
            }
          ]
        }
      ]
    }
  ]
}