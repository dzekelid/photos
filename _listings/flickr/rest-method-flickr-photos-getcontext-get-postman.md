{
  "info": {
    "name": "Flickr Get Photos",
    "_postman_id": "038692fc-63bb-44ff-9bd9-3d6ae70def3e",
    "description": "Returns next and previous photos for a photo in a photostream",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "photos",
      "item": [
        {
          "id": "2dd37d6e-1184-4330-bdc4-84adf71c49f2",
          "name": "getPhotostreamContextByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photos.getContext?api_key=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns next and previous photos for a photo in a photostream"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23d9bb77-8963-4370-8740-bf8f95c382c6"
            }
          ]
        }
      ]
    }
  ]
}