{
  "info": {
    "name": "Flickr Photosets Comments Get List",
    "_postman_id": "97dad6ae-9665-48c9-8d4c-5c30b857ac6c",
    "description": "Returns the comments for a photoset.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "0e1c19c9-bcb0-4397-9434-028a4d570b41",
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
              "id": "3434c687-6eee-4666-951a-55ee58618332"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "71eb7b38-3eab-4d09-9eb4-be59e2eed5a5",
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
              "id": "aa3a92b6-27a3-484c-9931-3216c65dc951"
            }
          ]
        },
        {
          "id": "869d87be-3e54-496b-9873-285f158cbc8e",
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
              "id": "1cf28b44-5d1c-4ddc-b212-a6849911341e"
            }
          ]
        },
        {
          "id": "ba0048f4-3af8-4895-b18d-3d9c079c9e43",
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
              "id": "84185896-42e4-42a0-ba9b-78fb2858015d"
            }
          ]
        },
        {
          "id": "76d97304-d384-4a91-b9f8-754a95b17a34",
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
              "id": "a4dd6c6b-bd05-431c-ae18-fc4b9e1a3d6e"
            }
          ]
        },
        {
          "id": "33785d95-d651-4359-92a9-d41d3c5e6afb",
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
              "id": "b5b2d0dd-c202-4f52-bba2-705553feaa2f"
            }
          ]
        }
      ]
    },
    {
      "name": "Photosets",
      "item": [
        {
          "id": "75d9d008-1ec4-4ce0-9b99-c1cd36ba0fd8",
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
              "id": "f28c3a6b-69e1-4b46-82c8-17891ea7589b"
            }
          ]
        },
        {
          "id": "a2f12bb0-5f1f-4c09-bafd-8c2f27ef445d",
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
              "id": "cf6566b7-ed54-44ae-bc50-9af9dc0cb8d0"
            }
          ]
        },
        {
          "id": "c73b09f8-6303-4be0-83e1-65a67cc8f271",
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
              "id": "9fb0c335-ac5b-4c98-92b0-cb3dca4235d8"
            }
          ]
        },
        {
          "id": "19e557bb-f26a-468f-95cc-cc1281cf9658",
          "name": "getRestMethodFlickr.photosets.comments.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.comments.getList?api_key=%7B%7D&format=%7B%7D&photoset_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the comments for a photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85ba19e2-ce91-4e88-b900-66d4d729aea2"
            }
          ]
        }
      ]
    }
  ]
}