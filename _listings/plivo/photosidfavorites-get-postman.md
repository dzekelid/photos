{
  "info": {
    "name": "Codenvy Account API Get Photos Favorites",
    "_postman_id": "51128ca5-5b70-43dc-bfc4-9a56040f1cd7",
    "description": "Returns all users that had favorite that photo.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Photos",
      "item": [
        {
          "id": "f9ef76ee-6017-46f6-b44e-f031f04f43ec",
          "name": "returns-all-users-that-had-favorite-that-photo",
          "request": {
            "url": "http:///account/https://codenvy.com/api/photos/:id/favorites?page=%7B%7D&rpp=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all users that had favorite that photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18822151-4ca8-46ee-8414-e6f2aaad9079"
            }
          ]
        }
      ]
    }
  ]
}