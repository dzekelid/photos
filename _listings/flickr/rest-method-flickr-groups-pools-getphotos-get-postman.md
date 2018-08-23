{
  "info": {
    "name": "Flickr Get Group Pool Photos",
    "_postman_id": "9d5f7a5e-c405-4362-934f-b4368bada7b8",
    "description": "Returns a list of pool photos for a given group",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "photos",
      "item": [
        {
          "id": "05ec0f68-9489-49d8-8073-b766ef49a998",
          "name": "getGroupPhotosByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.groups.pools.getPhotos?api_key=%7B%7D&group_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of pool photos for a given group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54028cfc-fa53-4b58-a05f-9e1a0996a86d"
            }
          ]
        }
      ]
    }
  ]
}