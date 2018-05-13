{
  "info": {
    "name": "Flickr Get Photo Sets",
    "_postman_id": "dac4c3d0-4319-475d-8e65-0021f235b7d4",
    "description": "Returns the albums belonging to the specified user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "photos",
      "item": [
        {
          "id": "8ee225fa-9cf3-418c-a7a2-280c8d145775",
          "name": "getAlbumsByPersonID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photosets.getList?api_key=%7B%7D&page=%7B%7D&per_page=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the albums belonging to the specified user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17be908d-b997-4369-9b64-44ff54f59a63"
            }
          ]
        }
      ]
    }
  ]
}