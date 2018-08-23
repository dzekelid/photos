{
  "info": {
    "name": "Flickr Get Groups",
    "_postman_id": "5d26f008-551c-4a68-9bf7-19566d0119e9",
    "description": "Get information about a group",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "photos",
      "item": [
        {
          "id": "4d616dd0-b250-418c-b095-f7cee3c855ca",
          "name": "getGroupByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.groups.getInfo?api_key=%7B%7D&group_id=%7B%7D&group_path_alias=%7B%7D&lang=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4fa0fc51-b5e9-47df-a943-ca8292e47de6"
            }
          ]
        }
      ]
    }
  ]
}