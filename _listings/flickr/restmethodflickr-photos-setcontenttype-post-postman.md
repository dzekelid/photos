{
  "info": {
    "name": "Flickr Photos Set Content Type",
    "_postman_id": "e66357de-d683-47ed-8428-38f4f11d3a74",
    "description": "Set the content type of a photo.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Photos",
      "item": [
        {
          "id": "549355ae-e6f4-4034-bcfc-69197f9618e7",
          "name": "postRestMethodFlickr.photos.setcontenttype",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.setContentType?api_key=%7B%7D&content_type=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set the content type of a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6111e43-ad15-4f26-a78e-f994dd18aa2c"
            }
          ]
        }
      ]
    }
  ]
}