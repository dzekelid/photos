{
  "info": {
    "name": "500px Get Photos",
    "_postman_id": "fd04c477-4408-442b-b4b0-4235e83e7422",
    "description": "Returns a listing of twenty (up to one hundred) photos for a specified photo stream.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blogs",
      "item": [
        {
          "id": "bd395b5a-3985-4fb5-8d45-175729c42f5f",
          "name": "getBlogs",
          "request": {
            "url": "http://api.500px.com/v1/blogs/?feature=%7B%7D&feature (required)=%7B%7D&page=%7B%7D&rpp=%7B%7D&user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a listing of five recent stories (maximum 100 per page)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd9d21f0-2ccd-420f-90e8-c802d50d5fab"
            }
          ]
        },
        {
          "id": "1174549d-8952-458b-963b-77940b74d6ad",
          "name": "postBlogs",
          "request": {
            "url": "http://api.500px.com/v1/blogs/?body (required)=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&photo_ids=%7B%7D&tags=%7B%7D&title (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Story."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fcae9725-6d26-4309-86e0-1692af32483b"
            }
          ]
        },
        {
          "id": "be43d468-5fad-4b3d-ab65-e9b2d5d23d5b",
          "name": "getBlogs",
          "request": {
            "url": "http://api.500px.com/v1/blogs/:id?id (required) - Return information for the specific story.=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns detailed information of a single story."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42aa490b-c4f0-48b8-93f2-3e1ae12cb780"
            }
          ]
        },
        {
          "id": "1ad6fdc3-1e24-4cdb-9936-edfa4ab8ca13",
          "name": "putBlogs",
          "request": {
            "url": "http://api.500px.com/v1/blogs/:id?body=%7B%7D&id (required)=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&photo_ids=%7B%7D&tags=%7B%7D&title=%7B%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the Story."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "992ebc93-283a-4457-b50b-5549c30efc6a"
            }
          ]
        },
        {
          "id": "0bd8308b-da37-4287-9196-a2b29b67e6e6",
          "name": "deleteBlogs",
          "request": {
            "url": "http://api.500px.com/v1/blogs/:id?id (required)=%7B%7D",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the story."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11005bb9-9098-44e5-bcb3-8ebc5df57327"
            }
          ]
        },
        {
          "id": "b4fd7698-c917-4664-9ee6-264059bd6c55",
          "name": "getBlogsComments",
          "request": {
            "url": "http://api.500px.com/v1/blogs/:id/comments?id (required)=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a listing of twenty comments for a specific Story."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70d80887-cd12-4aae-8a06-e8bff717be3c"
            }
          ]
        },
        {
          "id": "42b476e2-c5d9-462c-9658-9fde6ff4b989",
          "name": "postBlogsComments",
          "request": {
            "url": "http://api.500px.com/v1/blogs/:id/comments?body (required)=%7B%7D&id (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a comment for the Story."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10baf46b-47f8-4c38-9f25-f447e42c8ec5"
            }
          ]
        }
      ]
    },
    {
      "name": "Collections",
      "item": [
        {
          "id": "555dae51-66ca-4394-92ae-fd3932e6dc82",
          "name": "getCollections",
          "request": {
            "url": "http://api.500px.com/v1/collections?photos_per_collection_limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a listing of all Users collections and sets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0a999a9-b426-4546-8069-4c043362b801"
            }
          ]
        },
        {
          "id": "86c67527-3094-412c-9bcd-fa0e9892226c",
          "name": "postCollections",
          "request": {
            "url": "http://api.500px.com/v1/collections?kind=%7B%7D&path=%7B%7D&path (required)=%7B%7D&photo_ids=%7B%7D&position=%7B%7D&title=%7B%7D&title (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates new a collection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81a8c580-7759-4920-aaae-4822a1bf05dd"
            }
          ]
        },
        {
          "id": "840b0530-2e48-4c45-b95f-ef7ac1c6ec52",
          "name": "getCollections",
          "request": {
            "url": "http://api.500px.com/v1/collections/:id?image_size - Numerical size of the image to link to, 1 being the smallest and 4 being the largest. Multiple image sizes may be specified as image_size[]=2&amp;image_size[]=4.=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a collection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d2b9e06-cd2c-4fd1-a785-d844761947b7"
            }
          ]
        },
        {
          "id": "d964f1ac-91de-4eff-8c02-58281e14e718",
          "name": "putCollections",
          "request": {
            "url": "http://api.500px.com/v1/collections/:id?id (required)=%7B%7D&kind=%7B%7D&path=%7B%7D&photo_ids=%7B%7D&position=%7B%7D&title=%7B%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates collection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0684b7bc-9167-486b-8d40-9e26ce03e781"
            }
          ]
        },
        {
          "id": "5716c2e6-e18b-4e4e-b2bf-5f97ec723b52",
          "name": "deleteCollections",
          "request": {
            "url": "http://api.500px.com/v1/collections/:id?Forkn      n      n        69=%7B%7D&Starn  nn    n      281=%7B%7D",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes collection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "add74922-539d-4b47-a675-2894c46d8197"
            }
          ]
        }
      ]
    },
    {
      "name": "Comments",
      "item": [
        {
          "id": "bb386ac6-35ac-4657-a04a-ff13b715c6ce",
          "name": "postCommentsComments",
          "request": {
            "url": "http://api.500px.com/v1/comments/:id/comments?body (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a reply to an existing comment. Comments can only be nested one level deep, you cannot reply to a reply of a comment. If a comment has a non-null parent_id value then it cannot be replied to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f217cf89-1bc1-4fd1-b32c-908a82f1661b"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "8b33aa39-f043-4c0a-8541-622f6a204388",
          "name": "getPhotos",
          "request": {
            "url": "http://api.500px.com/v1/photos?exclude=%7B%7D&feature=%7B%7D&image_size=%7B%7D&include_states=%7B%7D&include_store=%7B%7D&only=%7B%7D&page=%7B%7D&rpp=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D&tags=%7B%7D&username=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a listing of twenty (up to one hundred) photos for a specified photo stream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a4b7e3b-4b7a-4ec9-a20d-aed3534e2246"
            }
          ]
        }
      ]
    }
  ]
}