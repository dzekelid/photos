{
  "info": {
    "name": "Flickr Get Photo Set Photos",
    "_postman_id": "90c57afb-81d9-4219-aab7-38cc715a6d22",
    "description": "Returns a list of photos in an album.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "photos",
      "item": [
        {
          "id": "01e4022e-ab0f-40f7-9785-497e4cd84285",
          "name": "getAlbumByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photosets.getPhotos?api_key=%7B%7D&photoset_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of photos in an album"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "072e07a9-0bd6-4709-b068-333b174dbbaa"
            }
          ]
        }
      ]
    }
  ]
}