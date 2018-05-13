{
  "info": {
    "name": "Flickr Get Group Topic List",
    "_postman_id": "c4d0203f-b36c-4d01-a385-d29bc2778812",
    "description": "Get a list of discussion topics in a group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "photos",
      "item": [
        {
          "id": "6230d4fc-cead-4606-8dcf-74cfed990d7d",
          "name": "getGroupDiscussionsByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.groups.discuss.topics.getList?api_key=%7B%7D&group_id=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of discussion topics in a group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab852b5a-c655-4357-88ce-eb231109882f"
            }
          ]
        }
      ]
    }
  ]
}