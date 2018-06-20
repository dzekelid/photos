{
  "info": {
    "name": "Flickr Photosets Comments Edit Comment",
    "_postman_id": "9e3c8b6f-3fdb-42d3-b8e9-fb60c2d05a3a",
    "description": "Edit the text of a comment as the currently authenticated user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "7b0c07e1-cbc7-44b6-8d1a-804ee871d9de",
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
              "id": "bb791eb5-78db-448b-94bb-ccd750d31520"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "24b3a6b2-65ca-4f3e-9681-02db65ccb08e",
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
              "id": "f3f583de-284d-41d5-b3b1-425435c1e59c"
            }
          ]
        },
        {
          "id": "e494e2e6-980a-4c09-b054-8d9fea2ce4ba",
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
              "id": "3a6bfc08-c71a-43cb-92fa-a78f548aa9dc"
            }
          ]
        },
        {
          "id": "aed6ab92-94eb-40ee-aeb9-0a4ed703484a",
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
              "id": "cb42a983-8566-4bf5-87b5-0b5a868af743"
            }
          ]
        },
        {
          "id": "cd9b1db0-6780-4f2e-8af7-79468795b7e9",
          "name": "getRestMethodFlickr.photos.comments.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.comments.getList?api_key=%7B%7D&format=%7B%7D&max_comment_date=%7B%7D&min_comment_date=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the comments for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b0a35a7-e8e0-424d-8f7d-d4401ac0386f"
            }
          ]
        },
        {
          "id": "eb6e0f19-33f0-40f8-a54d-f8d6dd5a0f6c",
          "name": "getRestMethodFlickr.photos.comments.getrecentforcontacts",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.comments.getRecentForContacts?api_key=%7B%7D&contacts_filter=%7B%7D&date_lastcomment=%7B%7D&extras=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return the list of photos belonging to your contacts that have been commented on recently."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "652b9d74-c4ad-4802-a1da-23c16aa28593"
            }
          ]
        }
      ]
    },
    {
      "name": "Photosets",
      "item": [
        {
          "id": "3da89d67-641e-4b8a-9215-6fac37217c47",
          "name": "postRestMethodFlickr.photosets.comments.addcomment",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.comments.addComment?api_key=%7B%7D&comment_text=%7B%7D&format=%7B%7D&photoset_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a comment to a photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1c61bde-de72-49ba-aca8-add33ec728bf"
            }
          ]
        },
        {
          "id": "6dad3f24-e852-4527-8f56-5d05ef4a41bc",
          "name": "postRestMethodFlickr.photosets.comments.deletecomment",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.comments.deleteComment?api_key=%7B%7D&comment_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a photoset comment as the currently authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42b6fbf5-cfc7-4988-a110-9188fc90f766"
            }
          ]
        },
        {
          "id": "57710103-51db-46da-afc0-7b2670d8d558",
          "name": "postRestMethodFlickr.photosets.comments.editcomment",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.comments.editComment?api_key=%7B%7D&comment_id=%7B%7D&comment_text=%7B%7D",
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
              "id": "5d3eeb38-d880-4992-a32a-4d6548606aaf"
            }
          ]
        }
      ]
    }
  ]
}