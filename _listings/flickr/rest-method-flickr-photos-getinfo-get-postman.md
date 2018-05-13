{
  "info": {
    "name": "Flickr Get Photo",
    "_postman_id": "8c6de801-0f96-4dd2-8b7d-1b9a1cbeed90",
    "description": "Returns a photo",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "photos",
      "item": [
        {
          "id": "855a93a8-f4ae-4dac-9450-ccfd1bcac097",
          "name": "getPhotoByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photos.getInfo?api_key=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a photo"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8672ce2a-6a53-4e13-bfc6-eb4e48e2c851"
            }
          ]
        }
      ]
    }
  ]
}