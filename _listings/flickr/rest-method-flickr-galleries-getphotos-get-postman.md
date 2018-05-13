{
  "info": {
    "name": "Flickr Get Gallery Photos",
    "_postman_id": "ee50442f-9370-4d57-a3a5-aa7b49a924cb",
    "description": "Returns a list of photos in a gallery.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "photos",
      "item": [
        {
          "id": "17fc4db7-a5ef-4758-b1cc-04498026df53",
          "name": "getGalleryPhotosByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.galleries.getPhotos?api_key=%7B%7D&gallery_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of photos in a gallery"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "024dbfc3-9daf-4d6a-a25c-82b11f65e4cf"
            }
          ]
        }
      ]
    }
  ]
}