{
  "info": {
    "name": "GIGANDCROWD Get Art Photo Photoid Thumb",
    "_postman_id": "76c3db90-ee58-47f0-9614-9f80338cfb0d",
    "description": "Get art photo photoid thumb.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Admin",
      "item": [
        {
          "id": "fb048f6e-5d0e-4817-ab35-a9cd8e1dddda",
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
              "id": "7e98fa63-cf6a-4067-9c6d-17656e6766b8"
            }
          ]
        },
        {
          "id": "55b3dcd3-6517-42cb-980e-2eccfebd0868",
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
              "id": "453126a2-7cd9-492a-9575-3c2deb2ade33"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "bc7a57a5-7a06-4bf3-93c7-a26f19a588eb",
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
              "id": "cc9da3ba-bfb6-4ccb-961f-5878ebbae6b1"
            }
          ]
        },
        {
          "id": "6cb42843-e17a-49e1-8a20-d4b3cc78a129",
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
              "id": "e7673ee6-1740-4f44-848a-cf392df4bde2"
            }
          ]
        },
        {
          "id": "e1971656-2469-4868-a3fe-6a697eed4244",
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
              "id": "a9290d2a-a122-4549-a4d0-de6da88d5a55"
            }
          ]
        }
      ]
    },
    {
      "name": "Art",
      "item": [
        {
          "id": "6d1a703e-dafa-4825-bd9a-7b59523b461c",
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
              "id": "0e69ac47-c269-478a-bf30-7de21eaba204"
            }
          ]
        },
        {
          "id": "5d8eee8a-330f-486e-a5dd-c02477d40fb2",
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
              "id": "7de1ca9b-da00-4519-bfbf-71f8a9160fa4"
            }
          ]
        },
        {
          "id": "06331bf7-9072-483f-b8b5-a70da5105d2e",
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
              "id": "4844aa76-612a-4a30-9243-d6859c5faf12"
            }
          ]
        },
        {
          "id": "2c06c798-37dd-40b5-9331-347dd4130d36",
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
              "id": "05cfb9b4-a391-4a52-a5bf-e5ba0d05b597"
            }
          ]
        }
      ]
    }
  ]
}