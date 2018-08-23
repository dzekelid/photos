{
  "info": {
    "name": "Flickr Photos Get Contacts Photos",
    "_postman_id": "2316ff40-9c86-45c8-a33e-39bbae09fc8d",
    "description": "Fetch a list of recent photos from the calling users' contacts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Contacts",
      "item": [
        {
          "id": "db8df095-99b9-44e8-9387-70cfa4e68c10",
          "name": "getRestMethodFlickr.contacts.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.contacts.getList?api_key=%7B%7D&filter=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of contacts for the calling user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85a969bb-1110-4eb8-a7b7-dcbf4219e3a7"
            }
          ]
        },
        {
          "id": "5d96c0b9-7383-4caf-9f4a-1ec8fff4114a",
          "name": "getRestMethodFlickr.contacts.getlistrecentlyuploaded",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.contacts.getListRecentlyUploaded?api_key=%7B%7D&date_lastupload=%7B%7D&filter=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of contacts for a user who have recently uploaded photos along with the total count of photos uploaded. This method is still considered experimental. We don't plan for it to change or to go away but so long as this notice is present you should write your code accordingly."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9865901a-ad4e-4999-8533-d1ad9052cf41"
            }
          ]
        },
        {
          "id": "32cd1955-fa79-4660-af3d-a80b241b0fd7",
          "name": "getRestMethodFlickr.contacts.getpubliclist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.contacts.getPublicList?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the contact list for a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1af9683f-72ca-49e6-9a23-5bae9899f921"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "f960f1e6-81c8-41cc-ad98-6a1313c5828a",
          "name": "getRestMethodFlickr.photos.getcontactsphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getContactsPhotos?api_key=%7B%7D&count=%7B%7D&extras=%7B%7D&format=%7B%7D&include_self=%7B%7D&just_friends=%7B%7D&single_photo=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch a list of recent photos from the calling users' contacts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f03dbe6-c78a-46ac-b64d-682725d3de54"
            }
          ]
        }
      ]
    }
  ]
}