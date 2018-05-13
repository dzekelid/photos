{
  "info": {
    "name": "Flickr Get Group Replies",
    "_postman_id": "cacb8b2f-846f-4831-902a-94ff1006494f",
    "description": "Get information on a group topic reply",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "photos",
      "item": [
        {
          "id": "f14f7870-6024-4f49-97d8-1b87825a1927",
          "name": "getGroupTopicRepliesByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.groups.discuss.replies.getInfo?api_key=%7B%7D&group_id=%7B%7D&reply_id=%7B%7D&topic_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information on a group topic reply"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08eab3c6-c4d7-450d-9c26-0222b92c852d"
            }
          ]
        }
      ]
    }
  ]
}