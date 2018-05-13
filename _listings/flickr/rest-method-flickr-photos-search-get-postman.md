{
  "info": {
    "name": "Flickr Photo Search",
    "_postman_id": "95f06009-4506-43c8-bf0b-ef449a9844d8",
    "description": "Return a list of photos matching some criteria.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "photos",
      "item": [
        {
          "id": "bd22a489-12d9-4b64-811a-574116b8193b",
          "name": "getMediaBySearch",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photos.search?accuracy=%7B%7D&api_key=%7B%7D&bbox=%7B%7D&contacts=%7B%7D&content_type=%7B%7D&geo_context=%7B%7D&group_id=%7B%7D&has_geo=%7B%7D&in_gallery=%7B%7D&is_commons=%7B%7D&is_getty=%7B%7D&lat=%7B%7D&license=%7B%7D&lon=%7B%7D&machine_tags=%7B%7D&machine_tag_mode=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&media=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&place_id=%7B%7D&privacy_filter=%7B%7D&radius=%7B%7D&radius_units=%7B%7D&safe_search=%7B%7D&sort=%7B%7D&tags=%7B%7D&text=%7B%7D&user_id=%7B%7D&woe_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of photos matching some criteria"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7ff6062-9032-4571-803d-456fb9054d3d"
            }
          ]
        }
      ]
    }
  ]
}