{
  "info": {
    "name": "Flickr Get Photo Exif",
    "_postman_id": "ca9463ee-5815-4193-a2ac-55bfd6e497c5",
    "description": "Retrieves a list of EXIF/TIFF/GPS tags for a given photo. The calling user must have permission to view the photo.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "photos",
      "item": [
        {
          "id": "42f4fbe9-bc4a-4da9-b6a6-f55233965006",
          "name": "getPhotoExifByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photos.getExif?api_key=%7B%7D&photo_id=%7B%7D&secret=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a list of EXIF/TIFF/GPS tags for a given photo"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7d52497-5214-4aed-ae97-785700971741"
            }
          ]
        }
      ]
    }
  ]
}