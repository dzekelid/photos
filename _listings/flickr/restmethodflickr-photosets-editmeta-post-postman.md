{
  "info": {
    "name": "Flickr Photosets Edit Meta",
    "_postman_id": "f5758ba1-428b-46ef-b6a4-8edb0e7ef378",
    "description": "Modify the meta-data for a photoset.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "8c982ea1-2728-4444-9a32-bf2835317f2c",
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
              "id": "a1697cfb-e6dc-4d90-a91c-b98bdae54f84"
            }
          ]
        }
      ]
    },
    {
      "name": "Galleries",
      "item": [
        {
          "id": "e46192b3-9d99-40c9-8fb1-cd2111d02060",
          "name": "postRestMethodFlickr.galleries.editmeta",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.galleries.editMeta?api_key=%7B%7D&description=%7B%7D&gallery_id=%7B%7D&title=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Modify the metadata for a gallery."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c120ecf-70d9-499d-9942-ae46cfff5fe0"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "a72f6c9c-080c-42e7-bd2a-6c085e189d3b",
          "name": "getRestMethodFlickr.groups.members.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.members.getList?api_key=%7B%7D&format=%7B%7D&group_id=%7B%7D&membertypes=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of the members of a group. The call must be signed on behalf of a Flickr member, and the ability to see the group membership will be determined by the Flickr member's group privileges."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1379195-dbe8-46bb-8292-8fb7ec9e3d2e"
            }
          ]
        }
      ]
    },
    {
      "name": "Machinetags",
      "item": [
        {
          "id": "e63bc0bf-ebcd-413d-92ba-5ee770f033d1",
          "name": "getRestMethodFlickr.machinetags.getnamespaces",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.machinetags.getNamespaces?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&predicate=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of unique namespaces, optionally limited by a given predicate, in alphabetical order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d06098f-1581-4471-9295-026a316f76af"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "26b1e765-5f0a-4985-9b33-971d5062a138",
          "name": "getRestMethodFlickr.people.findbyusername",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.people.findByUsername?api_key=%7B%7D&format=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a user's NSID, given their username."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6a6151e-e316-4d2a-8440-6366b9168f2f"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "1616f335-9600-429c-a693-89b78733d214",
          "name": "postRestMethodFlickr.photos.setmeta",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.setMeta?api_key=%7B%7D&description=%7B%7D&photo_id=%7B%7D&title=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set the meta information for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42af8861-950f-419f-96f8-797588692cd2"
            }
          ]
        },
        {
          "id": "2156d4b6-3255-4d51-9ed3-5280cd4c90f7",
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
              "id": "7e3aaaa3-3c93-4560-b85c-67b41e9d398d"
            }
          ]
        },
        {
          "id": "9bf8912e-629d-4c91-9086-61f84d8fa6e7",
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
              "id": "b4f089cd-3d23-4b5e-af8b-f25bab98e055"
            }
          ]
        },
        {
          "id": "864fd78f-1917-4963-b1c7-bb0293080af0",
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
              "id": "87cb76cf-0aef-4f7c-b64d-9f53cf77349f"
            }
          ]
        },
        {
          "id": "25948ccb-fd22-4953-b37b-8c4d9759072a",
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
              "id": "3f671cf2-ad32-4964-bcf6-a6e044341245"
            }
          ]
        },
        {
          "id": "c10e7645-5a49-44be-acd3-c37a0b90681d",
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
              "id": "6b2f1977-392c-4803-9123-59d795fde007"
            }
          ]
        }
      ]
    },
    {
      "name": "Photosets",
      "item": [
        {
          "id": "997286a5-6667-485e-a730-938ca33797c2",
          "name": "postRestMethodFlickr.photosets.editmeta",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.editMeta?api_key=%7B%7D&description=%7B%7D&photoset_id=%7B%7D&title=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Modify the meta-data for a photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ba7f0ea-d0dd-4c40-ab3a-76faf3590f46"
            }
          ]
        }
      ]
    }
  ]
}