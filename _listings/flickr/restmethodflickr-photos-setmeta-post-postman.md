{
  "info": {
    "name": "Flickr Photos Set Meta",
    "_postman_id": "f02d41ab-5ec4-4867-ae3f-5b88d271c886",
    "description": "Set the meta information for a photo.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "b07a2cba-3b5a-431c-ae8b-41913e4a8b7d",
          "name": "getRestMethodFlickr.activity.usercomments",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.activity.userComments?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of recent activity on photos commented on by the calling user. Do not poll this method more than once an hour."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49ce674e-cfa9-43be-8322-62abaa943f3a"
            }
          ]
        }
      ]
    },
    {
      "name": "Galleries",
      "item": [
        {
          "id": "8152be69-dcb4-440e-916c-435775bf0db2",
          "name": "postRestMethodFlickr.galleries.editmeta",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.galleries.editMeta?api_key=%7B%7D&description=%7B%7D&gallery_id=%7B%7D&title=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Modify the metadata for a gallery."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3128c067-bcf7-476e-b655-9a4cea658be9"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "fa9226c1-78a2-4710-a71e-6032a55029e8",
          "name": "getRestMethodFlickr.groups.members.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.members.getList?api_key=%7B%7D&format=%7B%7D&group_id=%7B%7D&membertypes=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of the members of a group. The call must be signed on behalf of a Flickr member, and the ability to see the group membership will be determined by the Flickr member's group privileges."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c45f70d-b34f-4338-9c75-a5b7cdfad22e"
            }
          ]
        }
      ]
    },
    {
      "name": "Machinetags",
      "item": [
        {
          "id": "f01ce629-f139-4bc6-8e8e-e2b1832ee8bc",
          "name": "getRestMethodFlickr.machinetags.getnamespaces",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.machinetags.getNamespaces?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&predicate=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of unique namespaces, optionally limited by a given predicate, in alphabetical order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5bb27f1-3a70-4373-88b2-4eeed75c4ada"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "e051c822-c4a3-43cc-89ce-81d47c345c63",
          "name": "getRestMethodFlickr.people.findbyusername",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.people.findByUsername?api_key=%7B%7D&format=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a user's NSID, given their username."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c44e920-593e-4025-bc6a-eaf62311965c"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "c75b6275-ccbf-4f24-9a6f-6d8ff7f43c73",
          "name": "postRestMethodFlickr.photos.setmeta",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.setMeta?api_key=%7B%7D&description=%7B%7D&photo_id=%7B%7D&title=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set the meta information for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8185273-74ea-4b63-af70-5d96c2a55e4b"
            }
          ]
        }
      ]
    }
  ]
}