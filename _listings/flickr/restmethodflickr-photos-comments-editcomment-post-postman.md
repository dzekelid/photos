{
  "info": {
    "name": "Flickr Photos Comments Edit Comment",
    "_postman_id": "a849cda8-1772-4681-8670-57bf28da9bb2",
    "description": "Edit the text of a comment as the currently authenticated user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "1b735f00-b219-4d2f-8631-316a87667fb2",
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
              "id": "165d6727-44b6-48e1-8738-85ff807e4e9c"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "17e0de83-c1e1-43a8-94a9-621cce6407f0",
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
              "id": "d3572341-af8a-4e42-a129-f1c2e8fdda05"
            }
          ]
        },
        {
          "id": "9918ca20-bc5e-4d47-ac42-6e3ab8471a95",
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
              "id": "0855fcb2-bdf9-4ee0-b53e-77a09951ea64"
            }
          ]
        },
        {
          "id": "89491908-e44b-4188-bc57-85d1f8c71c84",
          "name": "postRestMethodFlickr.photos.comments.editcomment",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.comments.editComment?api_key=%7B%7D&comment_id=%7B%7D&comment_text=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Edit the text of a comment as the currently authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a1376cb-225c-428c-8471-b3479ab3ea68"
            }
          ]
        }
      ]
    }
  ]
}