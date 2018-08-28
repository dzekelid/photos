{
  "info": {
    "name": "GIGANDCROWD Post Admin Place Placeid Photos",
    "_postman_id": "fcee046e-6d2e-411f-863b-0e0e742db845",
    "description": "Post admin place placeid photos.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Admin",
      "item": [
        {
          "id": "41d4d6b1-2aa1-47df-8a44-ff6a23edac93",
          "name": "postApiV1AdminPlacePlacePhotos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/admin/place/:placeId/photos"
              ],
              "query": [
                {
                  "key": "file",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "placeId",
                  "value": "placeId",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Post admin place placeid photos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8c459c1-8a97-4cc4-bccf-6cb5ab875c5f"
            }
          ]
        }
      ]
    }
  ]
}