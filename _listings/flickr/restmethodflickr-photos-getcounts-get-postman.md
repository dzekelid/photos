{
  "info": {
    "name": "Flickr Photos Get Counts",
    "_postman_id": "0daedd23-ddbc-47f6-825a-444564abcc8e",
    "description": "Returns next and previous photos for a photo in a photostream.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Photos",
      "item": [
        {
          "id": "ee910749-32f5-4d7b-ab4c-90ca6a6f3387",
          "name": "getRestMethodFlickr.photos.getcounts",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getCounts?api_key=%7B%7D&dates=%7B%7D&format=%7B%7D&taken_dates=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns next and previous photos for a photo in a photostream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e390105-ab65-4da6-b799-d6b82a848fb2"
            }
          ]
        }
      ]
    }
  ]
}