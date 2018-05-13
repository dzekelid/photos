{
  "info": {
    "name": "Flickr Get Group Topic Info",
    "_postman_id": "d765dc53-c9bc-4a17-839e-a6094cf7e90c",
    "description": "Get information about a group discussion topic",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "photos",
      "item": [
        {
          "id": "911b6b58-ade1-4cb4-8910-9648c5c06dcd",
          "name": "getGroupTopicByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.groups.discuss.topics.getInfo?api_key=%7B%7D&group_id=%7B%7D&topic_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a group discussion topic"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0d20c4e-27e4-4066-a029-152a3c87685c"
            }
          ]
        }
      ]
    }
  ]
}