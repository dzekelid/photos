{
  "info": {
    "name": "Flickr Photos Get With Geo Data",
    "_postman_id": "2eb321ef-af81-42b9-ae36-4332a36423a7",
    "description": "Returns a list of your geo-tagged photos.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Photos",
      "item": [
        {
          "id": "3c746bf9-f39a-42c0-b6fc-eff3c74ea914",
          "name": "getRestMethodFlickr.photos.getwithgeodata",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getWithGeoData?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&media=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&privacy_filter=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of your geo-tagged photos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64e67080-ea44-4e79-ac27-29ce662ad097"
            }
          ]
        }
      ]
    }
  ]
}