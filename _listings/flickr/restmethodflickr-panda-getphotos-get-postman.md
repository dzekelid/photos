{
  "info": {
    "name": "Flickr Panda Get Photos",
    "_postman_id": "c939b8c8-c419-45f5-9290-2309bb347f43",
    "description": "Ask the Flickr Pandas for a list of recent public (and \"safe\") photos. More information about the pandas can be found on the dev blog.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "d1d9165d-842c-4c58-bfd9-230216fc1cf9",
          "name": "getRestMethodFlickr.activity.userphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.activity.userPhotos?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&timeframe=%7B%7D",
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
              "id": "17625d3b-b4ab-450a-829d-9be1580400c9"
            }
          ]
        }
      ]
    },
    {
      "name": "Galleries",
      "item": [
        {
          "id": "d14e9c85-2eb6-41ab-b7ed-6302e10796bc",
          "name": "postRestMethodFlickr.galleries.editphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.galleries.editPhotos?api_key=%7B%7D&gallery_id=%7B%7D&photo_ids=%7B%7D&primary_photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Modify the photos in a gallery. Use this method to add, remove and re-order photos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7cef356-f4b8-479e-8f34-7acd145966ea"
            }
          ]
        },
        {
          "id": "59b1c798-e3ad-4686-a7d1-30737da77bd0",
          "name": "getRestMethodFlickr.galleries.getphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.galleries.getPhotos?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&gallery_id=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return the list of photos for a gallery."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d83aebb1-494b-4569-a089-e689c5ce9f43"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "d3c11f4c-23f0-4e18-87a3-08c43aa864fa",
          "name": "getRestMethodFlickr.groups.pools.getphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.pools.getPhotos?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&tags=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of pool photos for a given group, based on the permissions of the group and the user logged in (if any)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6cbb681-9772-4f70-b756-c877a8cac2fc"
            }
          ]
        }
      ]
    },
    {
      "name": "Panda",
      "item": [
        {
          "id": "870ba04b-4d4c-42c9-a396-7920850f2155",
          "name": "getRestMethodFlickr.panda.getphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.panda.getPhotos?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&page=%7B%7D&panda_name=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Ask the Flickr Pandas for a list of recent public (and \"safe\") photos. More information about the pandas can be found on the dev blog."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92efbf8c-a13a-4460-a561-92ddb9ab242f"
            }
          ]
        }
      ]
    }
  ]
}