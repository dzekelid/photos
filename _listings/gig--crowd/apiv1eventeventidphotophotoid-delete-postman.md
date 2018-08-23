{
  "info": {
    "name": "GIGANDCROWD Delete Event Eventid Photo Photoid",
    "_postman_id": "2dd63e32-2224-4f34-86cd-7e44ae66b425",
    "description": "Delete event eventid photo photoid.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Admin",
      "item": [
        {
          "id": "e91d09d7-9074-46f6-a68f-368f9d82ca27",
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
              "id": "0d46b213-8a0c-4a9d-b19b-5faab949a30c"
            }
          ]
        },
        {
          "id": "2702e9c2-f164-45ab-af81-cf8c18d14d0f",
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
              "id": "6cf5a1c8-11c2-4b60-ad49-5321b1b581e5"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "5e936892-1ce2-4c07-8a2c-faf52acf96b8",
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
              "id": "1e5a87b8-3872-4e81-8536-38df75a43ad1"
            }
          ]
        },
        {
          "id": "5cc08b46-ecbe-40e9-af1a-612f190f47aa",
          "name": "postApiV1EventEventPhoto",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/event/:eventId/photo"
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
            "description": "Post event eventid photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "415dd51c-bb8c-4f8d-b25c-9ce6ab658e92"
            }
          ]
        },
        {
          "id": "33903b96-d2ba-4ed5-b72f-0c69e2511df6",
          "name": "deleteApiV1EventEventPhotoPhoto",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/event/:eventId/photo/:photoId"
              ],
              "variable": [
                {
                  "id": "eventId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "photoId",
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
            "description": "Delete event eventid photo photoid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c4a003e-e0f8-482a-8d7e-f1e10fb49789"
            }
          ]
        }
      ]
    },
    {
      "name": "Art",
      "item": [
        {
          "id": "70c41749-c7e1-4057-8a94-953d0f67bdd4",
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
              "id": "afc94ffe-00b2-4326-a660-657ec5dcbef0"
            }
          ]
        },
        {
          "id": "529bdf61-e4ac-4ee5-b2e4-adc532a91fb6",
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
              "id": "41022597-0502-49c7-9945-97af2c24d54a"
            }
          ]
        },
        {
          "id": "7047ab3b-b58b-4caa-80fa-fbd6c8f517e7",
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
              "id": "81f21b97-bf42-4fd7-b913-1928c0317f09"
            }
          ]
        },
        {
          "id": "794d1e6d-d968-4b7e-a9a9-0972122b15ce",
          "name": "deleteApiV1ArtPhoto",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/art/photo/:id"
              ],
              "variable": [
                {
                  "id": "id",
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
            "description": "Delete art photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7185ff6d-6c8d-4195-ab8c-9edbedf98ed5"
            }
          ]
        }
      ]
    }
  ]
}