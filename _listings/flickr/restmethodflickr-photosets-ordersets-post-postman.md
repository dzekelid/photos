{
  "info": {
    "name": "Flickr Photosets Order Sets",
    "_postman_id": "a920bd03-60a2-4557-8eac-a47c7c14ec6b",
    "description": "Set the order of photosets for the calling user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Photosets",
      "item": [
        {
          "id": "c56b63ae-cb32-49ba-be51-131445e18f0f",
          "name": "postRestMethodFlickr.photosets.ordersets",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.orderSets?api_key=%7B%7D&photoset_ids=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set the order of photosets for the calling user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "651d33a5-af2a-406b-a619-73a927c6c45e"
            }
          ]
        }
      ]
    }
  ]
}