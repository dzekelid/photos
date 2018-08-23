{
  "info": {
    "name": "Flickr Photos Comments Delete Comment",
    "_postman_id": "3f6be678-524f-4bc7-84c2-dcf13b96336d",
    "description": "Delete comment as the currently authenticated user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "923b89b2-926e-4c92-9600-4cd80641b2f6",
          "name": "getRestMethodFlickr.activity.usercomments",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.activity.userComments?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of recent activity on photos commented on by the calling user. Do not poll this method more than once an hour."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc19906a-d70d-41e5-b45b-961f84bc801e"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "4d9d58a4-f746-4df4-a3dc-f858a2fd9c60",
          "name": "postRestMethodFlickr.photos.comments.addcomment",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.comments.addComment?api_key=%7B%7D&comment_text=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add comment to a photo as the currently authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be398726-7102-49fc-be73-f7f7b043b86d"
            }
          ]
        },
        {
          "id": "cbbe224c-12ed-4f22-8396-62bc68b8fe87",
          "name": "postRestMethodFlickr.photos.comments.deletecomment",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.comments.deleteComment?api_key=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delete comment as the currently authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48db66f5-6aa8-4750-815f-0d4474bcc2f2"
            }
          ]
        }
      ]
    }
  ]
}