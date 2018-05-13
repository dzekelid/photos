{
  "info": {
    "name": "Flickr Get Photo Set",
    "_postman_id": "ed1bc678-8a96-4430-8d48-5a869a93032c",
    "description": "Returns next and previous photos for a photo in a set",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "photos",
      "item": [
        {
          "id": "d1f917d4-79ca-4bef-a720-d00a83ac4aa3",
          "name": "getAlbumContextByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photosets.getContext?api_key=%7B%7D&photoset_id=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns next and previous photos for a photo in a set"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7068abf9-f071-4b60-81f0-b917ea8b82d1"
            }
          ]
        }
      ]
    }
  ]
}