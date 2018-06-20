{
  "info": {
    "name": "Flickr Photos Get Favorites",
    "_postman_id": "17e68cf2-d321-4d77-9782-1eca6f10ccd8",
    "description": "Returns the list of people who have favorited a given photo.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Favorites",
      "item": [
        {
          "id": "566395fe-639f-4dc1-84b0-62e302de544e",
          "name": "getRestMethodFlickr.favorites.add",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.favorites.add?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a photo to a user's favorites list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b214321d-a852-4c36-ab5b-d5c79c0b3782"
            }
          ]
        },
        {
          "id": "ab0c87ae-fca6-4007-87d9-f328ad902548",
          "name": "getRestMethodFlickr.favorites.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.favorites.getList?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&max_fave_date=%7B%7D&min_fave_date=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the user's favorite photos. Only photos which the calling user has permission to see are returned."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8944beab-c20f-4acb-b08b-d70d0014a7e5"
            }
          ]
        },
        {
          "id": "7946f459-79af-4731-9063-54445d5a165f",
          "name": "getRestMethodFlickr.favorites.getpubliclist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.favorites.getPublicList?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&max_fave_date=%7B%7D&min_fave_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of favorite public photos for the given user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "def6132d-f911-47a2-9b96-cd23acda4c15"
            }
          ]
        },
        {
          "id": "3c407c88-de0e-4ed3-a05a-9f41caa5ab13",
          "name": "getRestMethodFlickr.favorites.remove",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.favorites.remove?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a photo to a user's favorites list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27aaac3d-5709-4e0d-a09a-e8584c4fa031"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "79e16c15-5439-456e-b52e-ef6130d5175e",
          "name": "getRestMethodFlickr.photos.getfavorites",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getFavorites?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of people who have favorited a given photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b8e37a0-0c92-4e86-8849-0ea1653f09cf"
            }
          ]
        }
      ]
    }
  ]
}