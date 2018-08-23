{
  "info": {
    "name": "GIGANDCROWD Post Art Photo Type",
    "_postman_id": "4cd2fd7b-7a2d-4496-9ace-0a8784e95501",
    "description": "Post art photo type.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Admin",
      "item": [
        {
          "id": "04250daa-6b6e-4dc9-b480-109e30fb6ae6",
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
              "id": "ec2a224f-1264-473d-93c4-3dff952256c6"
            }
          ]
        },
        {
          "id": "17f0ca52-5444-403c-bdbd-b6cffd5b7def",
          "name": "deleteApiV1AdminPlacePlacePhotoPhoto",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/admin/place/:placeId/photo/:photoId"
              ],
              "variable": [
                {
                  "id": "photoId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "placeId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
            "description": "Delete admin place placeid photo photoid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "580ac796-0672-4e5f-a775-4049ffbb94b4"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "82cdcfca-a88a-44ae-8150-c49546293ede",
          "name": "postApiV1EventEventPhotos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/event/:eventId/photos"
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
                  "id": "eventId",
                  "value": "eventId",
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
            "description": "Post event eventid photos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6b3d4e0-7408-40ed-929d-e0756f24a403"
            }
          ]
        }
      ]
    },
    {
      "name": "Art",
      "item": [
        {
          "id": "9b6b9e78-4dbc-4ec6-b1f3-852bf0147b62",
          "name": "getApiV1ArtPhotoPhoto",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/art/photo/:photoId"
              ],
              "variable": [
                {
                  "id": "photoId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
            "description": "Get art photo photoid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8f4ca03-ee56-4156-bf00-e0d2e017ff8f"
            }
          ]
        },
        {
          "id": "f65f9f95-480e-4768-94b0-5ed7254f7be7",
          "name": "getApiV1ArtPhotoPhotoThumb",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/art/photo/:photoId/thumb"
              ],
              "variable": [
                {
                  "id": "photoId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
            "description": "Get art photo photoid thumb."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb292671-75a1-4816-bc70-ec239b8b1457"
            }
          ]
        },
        {
          "id": "f4ade114-b9cb-4c64-bb31-0696d8d2224f",
          "name": "postApiV1ArtPhotoType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/art/photo/:type"
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
                  "id": "type",
                  "value": "type",
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
            "description": "Post art photo type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df6a5904-fc9e-49e7-8c88-2bf73c3bfbea"
            }
          ]
        }
      ]
    }
  ]
}