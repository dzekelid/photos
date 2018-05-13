{
  "info": {
    "name": "Flickr Get Photo Licenses",
    "_postman_id": "a3f687aa-26e0-4a84-993c-f424d2cdff97",
    "description": "Fetches a list of available photo licenses for Flickr",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "photos",
      "item": [
        {
          "id": "4a1c249e-c7e3-4ab5-90cc-3cefda9e48b3",
          "name": "getLicenseByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photos.licenses.getInfo?api_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches a list of available photo licenses for Flickr"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24a5b2b0-85ae-4da5-8fd3-413669928c39"
            }
          ]
        }
      ]
    }
  ]
}