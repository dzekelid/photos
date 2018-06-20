{
  "info": {
    "name": "Flickr Stats Get Photostream Domains",
    "_postman_id": "c3a7654b-03b8-49bf-9857-36bd39691653",
    "description": "Get a list of referring domains for a photostream.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Stats",
      "item": [
        {
          "id": "99d4c03a-72ae-411b-a441-5c1c00dac14f",
          "name": "getRestMethodFlickr.stats.getcollectiondomains",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getCollectionDomains?api_key=%7B%7D&collection_id=%7B%7D&date=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of referring domains for a collection"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2d3dc74-4a25-4e14-bbf6-59d0eb752028"
            }
          ]
        },
        {
          "id": "8dcdfa78-7874-4dbd-a7ce-e57fe2ad1d91",
          "name": "getRestMethodFlickr.stats.getphotodomains",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getPhotoDomains?api_key=%7B%7D&date=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of referring domains for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "670de817-3cf1-442a-9ce6-8847fca1e1e7"
            }
          ]
        },
        {
          "id": "59057621-f2d6-4342-acbe-0c0522ffa195",
          "name": "getRestMethodFlickr.stats.getphotosetdomains",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getPhotosetDomains?api_key=%7B%7D&date=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&photoset_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of referring domains for a photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d10495b6-8116-4100-b812-748d6de7fe33"
            }
          ]
        },
        {
          "id": "d0d01a3c-8883-4535-86b6-6df739148c87",
          "name": "getRestMethodFlickr.stats.getphotostreamdomains",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getPhotostreamDomains?api_key=%7B%7D&date=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of referring domains for a photostream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab45f66c-c444-46e9-bddb-88f2f6ee1e4e"
            }
          ]
        }
      ]
    }
  ]
}