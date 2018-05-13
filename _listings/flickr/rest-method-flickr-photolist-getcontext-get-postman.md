{
  "info": {
    "name": "Flickr Get Photo Lists",
    "_postman_id": "45da7c66-c60f-43f9-8e7a-d8b894c67640",
    "description": "Returns next and previous photos in a photo list",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "photos",
      "item": [
        {
          "id": "447600a3-7709-488b-8384-ed3886b07a32",
          "name": "getPhotolistContextByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photolist.getContext?api_key=%7B%7D&photolist_id=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns next and previous photos in a photo list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00e449b5-5205-4068-89be-d8d7b591ea6d"
            }
          ]
        }
      ]
    }
  ]
}