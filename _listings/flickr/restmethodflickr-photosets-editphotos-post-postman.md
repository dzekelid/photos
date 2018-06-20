{
  "info": {
    "name": "Flickr Photosets Edit Photos",
    "_postman_id": "cfd54c5a-e4af-45d7-96d6-539968965943",
    "description": "Modify the photos in a photoset. Use this method to add, remove and re-order photos.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "8f4dbbce-4b48-4445-a937-6f5ab2ffab24",
          "name": "getRestMethodFlickr.activity.userphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.activity.userPhotos?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&timeframe=%7B%7D",
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
              "id": "0e598263-969d-43aa-92e9-7b93b7356f69"
            }
          ]
        }
      ]
    },
    {
      "name": "Galleries",
      "item": [
        {
          "id": "c73439fb-f08e-41fa-98f0-dbee13aea79b",
          "name": "postRestMethodFlickr.galleries.editphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.galleries.editPhotos?api_key=%7B%7D&gallery_id=%7B%7D&photo_ids=%7B%7D&primary_photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Modify the photos in a gallery. Use this method to add, remove and re-order photos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05c6cf48-c4f7-42bb-bc53-f23b4703b06d"
            }
          ]
        },
        {
          "id": "0889d23b-0cfe-4b22-97af-09bad5a11e93",
          "name": "getRestMethodFlickr.galleries.getphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.galleries.getPhotos?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&gallery_id=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return the list of photos for a gallery."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4004cb5a-4c83-4eb6-9ffd-8910a7d5afee"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "b461be85-1936-4368-a960-a089e24b0d81",
          "name": "getRestMethodFlickr.groups.pools.getphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.pools.getPhotos?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&tags=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of pool photos for a given group, based on the permissions of the group and the user logged in (if any)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6311fc69-dca5-44aa-8131-1976467d8727"
            }
          ]
        }
      ]
    },
    {
      "name": "Panda",
      "item": [
        {
          "id": "f05cb9de-1528-4c84-94e3-272dc5eaf941",
          "name": "getRestMethodFlickr.panda.getphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.panda.getPhotos?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&page=%7B%7D&panda_name=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Ask the Flickr Pandas for a list of recent public (and \"safe\") photos. More information about the pandas can be found on the dev blog."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58e6955e-2652-4ea3-8111-d40f43954f00"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "1479590a-fc06-49a8-babf-fce6b50edfae",
          "name": "getRestMethodFlickr.people.getphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.people.getPhotos?api_key=%7B%7D&content_type=%7B%7D&extras=%7B%7D&format=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&privacy_filter=%7B%7D&safe_search=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return photos from the given user's photostream. Only photos visible to the calling user will be returned. This method must be authenticated; to return public photos for a user, use flickr.people.getPublicPhotos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "986f34cb-b210-4625-872b-358953befa00"
            }
          ]
        },
        {
          "id": "e9704acb-7eb2-4da1-bc57-58f9beea42b0",
          "name": "getRestMethodFlickr.people.getphotosof",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.people.getPhotosOf?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&owner_id=%7B%7D&page=%7B%7D&per_page=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of photos containing a particular Flickr member."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5058775e-4fbc-4dea-bc7e-f3bcb855ac4c"
            }
          ]
        },
        {
          "id": "356d1729-b4ca-4664-945f-4ca700369e65",
          "name": "getRestMethodFlickr.people.getpublicphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.people.getPublicPhotos?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&safe_search=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of public photos for the given user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08842c52-2256-482a-9068-1129e1577394"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "aefcdeb4-ae16-40d0-9b41-98dc81c0b8f3",
          "name": "postRestMethodFlickr.photos.addtags",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.addTags?api_key=%7B%7D&photo_id=%7B%7D&tags=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add tags to a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c501af9-8d4c-4327-9899-312a92f31b7c"
            }
          ]
        },
        {
          "id": "430f97c2-8634-4eae-ab74-6f9124fe295c",
          "name": "postRestMethodFlickr.photos.delete",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.delete?api_key=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a photo from Flickr."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae74dc58-e73c-4c8f-81d4-545fa42c7a26"
            }
          ]
        },
        {
          "id": "2402ff4d-3165-4574-923c-24e49ffb65ec",
          "name": "getRestMethodFlickr.photos.getallcontexts",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getAllContexts?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all visible sets and pools the photo belongs to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b4ee828-cc2a-4455-ab21-bf71631af695"
            }
          ]
        },
        {
          "id": "284bf71e-cb64-42b1-930c-82cd1ab61437",
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
              "id": "e76d3bf4-485b-4e3c-b3d9-e2a741b04500"
            }
          ]
        },
        {
          "id": "68e5c968-4ce4-4c68-a4ba-48cee5153850",
          "name": "getRestMethodFlickr.photos.getcontactspublicphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getContactsPublicPhotos?api_key=%7B%7D&count=%7B%7D&extras=%7B%7D&format=%7B%7D&include_self=%7B%7D&just_friends=%7B%7D&single_photo=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch a list of recent public photos from a users' contacts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d331042-302a-4781-93a7-2a90eb61b44a"
            }
          ]
        },
        {
          "id": "7c1a6361-f332-4845-9970-7b97fa9f3dad",
          "name": "getRestMethodFlickr.photos.getcontext",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getContext?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns next and previous photos for a photo in a photostream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1d02222-27e9-46f6-b17d-ea6ca4fd0e85"
            }
          ]
        },
        {
          "id": "1735bceb-9a8c-468b-9c9a-014a0c94cc47",
          "name": "getRestMethodFlickr.photos.getcounts",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getCounts?api_key=%7B%7D&dates=%7B%7D&format=%7B%7D&taken_dates=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns next and previous photos for a photo in a photostream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a66dd9b2-8a65-4a39-93d6-4ab8fd9e6b5f"
            }
          ]
        },
        {
          "id": "4874d91d-0f5a-4d2c-92bc-bcd712f5beed",
          "name": "getRestMethodFlickr.photos.getexif",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getExif?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D&secret=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a list of EXIF/TIFF/GPS tags for a given photo. The calling user must have permission to view the photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea4a68bc-7ac4-433a-82d7-b8c106cdb072"
            }
          ]
        },
        {
          "id": "bdc4ede0-d656-403d-92b8-d4ee4dab343e",
          "name": "getRestMethodFlickr.photos.getfavorites",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getFavorites?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of people who have favorited a given photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fea73fc8-5ebc-4b4d-b540-adb2c70dc4aa"
            }
          ]
        },
        {
          "id": "449052c8-1d6f-46bd-aca9-053f22dbc002",
          "name": "getRestMethodFlickr.photos.getinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getInfo?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D&secret=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a photo. The calling user must have permission to view the photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68a7b239-ec89-429f-ba97-deabcd1949ca"
            }
          ]
        },
        {
          "id": "1c7e0538-357a-42dd-93fd-952f66aada49",
          "name": "getRestMethodFlickr.photos.getnotinset",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getNotInSet?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&media=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&privacy_filter=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of your photos that are not part of any sets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1fa1b682-c203-423b-86a8-c494f1e652c7"
            }
          ]
        },
        {
          "id": "9fbc74b7-db43-4920-b014-f3a24a65781b",
          "name": "getRestMethodFlickr.photos.getperms",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getPerms?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get permissions for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6db09b85-c268-4a94-a1fa-8b53c1a6f771"
            }
          ]
        },
        {
          "id": "79d1000b-f8e9-4fad-b79e-61f034a318e1",
          "name": "getRestMethodFlickr.photos.getrecent",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getRecent?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of people who have favorited a given photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d706b083-b821-48fd-9103-9ba3e07b2f7e"
            }
          ]
        },
        {
          "id": "8508ae99-941a-4aa8-9fc3-32de5e592621",
          "name": "getRestMethodFlickr.photos.getsizes",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getSizes?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the available sizes for a photo. The calling user must have permission to view the photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4fdf94c6-5f8a-4c9f-bc05-eabb01a09292"
            }
          ]
        },
        {
          "id": "e10a10b9-508e-4b17-afc1-690a9ae0f13b",
          "name": "getRestMethodFlickr.photos.getuntagged",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getUntagged?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&media=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&privacy_filter=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of your photos that are not tagged."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "991554ee-b121-4e50-8c7c-14442e2f93ea"
            }
          ]
        },
        {
          "id": "dbce3aab-58e2-44c8-ab35-9fd195cc4114",
          "name": "getRestMethodFlickr.photos.getwithgeodata",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getWithGeoData?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&media=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&privacy_filter=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of your geo-tagged photos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "163d1a44-6182-4fea-848a-e427f2c288a5"
            }
          ]
        },
        {
          "id": "3366344c-c0f5-4522-8f88-4b02d619ec1b",
          "name": "getRestMethodFlickr.photos.getwithoutgeodata",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getWithoutGeoData?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&media=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&privacy_filter=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of your photos which haven't been geo-tagged."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64de1357-fbff-4f6a-9d9b-927b13110c3e"
            }
          ]
        },
        {
          "id": "b2d4354c-15ec-483b-9759-1f91fadeb690",
          "name": "getRestMethodFlickr.photos.getrecentlyupdated",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getRecentlyUpdated?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&min_date=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of your photos that have been recently created or which have been recently modified. Recently modified may mean that the photo's metadata (title, description, tags) may have been changed or a comment has been added (or just modified somehow :-)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "713b968a-5dde-47ec-91fb-b01959343a09"
            }
          ]
        },
        {
          "id": "24d4f203-c3af-4899-b1b8-31dd7a9fb4db",
          "name": "postRestMethodFlickr.photos.removetag",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.removeTag?api_key=%7B%7D&photo_id=%7B%7D&tag_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a tag from a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "060db5c2-ba4f-4f73-8adb-b9252fe41bda"
            }
          ]
        },
        {
          "id": "03d5d1c9-29fe-4c9c-a4d2-d6608d76365c",
          "name": "getRestMethodFlickr.photos.search",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.search?accuracy=%7B%7D&api_key=%7B%7D&contacts=%7B%7D&content_type=%7B%7D&extras=%7B%7D&format=%7B%7D&geo_context=%7B%7D&group_id=%7B%7D&has_geo=%7B%7D&hbox=%7B%7D&is_commons=%7B%7D&is_gallery=%7B%7D&is_getty=%7B%7D&lat=%7B%7D&license=%7B%7D&lon=%7B%7D&machine_tags=%7B%7D&machine_tag_mode=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&media=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&place_id=%7B%7D&privacy_filter=%7B%7D&radius=%7B%7D&radius_units=%7B%7D&safe_search=%7B%7D&sort=%7B%7D&tags=%7B%7D&tag_mode=%7B%7D&text=%7B%7D&user_id=%7B%7D&woe_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of photos matching some criteria. Only photos visible to the calling user will be returned. To return private or semi-private photos, the caller must be authenticated with 'read' permissions, and have permission to view the photos. Unauthenticated calls will only return public photos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "645011c3-f8c5-4902-b2f3-7e49dc85cdf7"
            }
          ]
        },
        {
          "id": "53856eb3-ebb9-4a96-a27f-05bebf758129",
          "name": "postRestMethodFlickr.photos.setcontenttype",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.setContentType?api_key=%7B%7D&content_type=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set the content type of a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f797276-cc39-4599-b757-9fce1da2b175"
            }
          ]
        },
        {
          "id": "99c2a0b5-ba0e-4cd5-92d3-d3559eaa7564",
          "name": "postRestMethodFlickr.photos.setdates",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.setDates?api_key=%7B%7D&date_posted=%7B%7D&date_taken=%7B%7D&date_taken_granularity=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set one or both of the dates for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "098710a9-a734-409f-ac1e-7fe24589debe"
            }
          ]
        },
        {
          "id": "da13601f-7826-4864-944b-a85e46cf6d1a",
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
              "id": "48fc7bec-c17b-41ee-bbb5-de75f4d697e4"
            }
          ]
        },
        {
          "id": "09c48e4a-b08f-4ea7-9722-6c3330ad90e1",
          "name": "postRestMethodFlickr.photos.setperms",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.setPerms?api_key=%7B%7D&format=%7B%7D&is_family=%7B%7D&is_friend=%7B%7D&is_public=%7B%7D&perm_addmeta=%7B%7D&perm_comment=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set permissions for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d14ccdb3-9eb5-45a2-b219-17d1e3535950"
            }
          ]
        },
        {
          "id": "1cba8eb0-a505-48ab-9df9-4a6103f5c05e",
          "name": "postRestMethodFlickr.photos.setsafetylevel",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.setSafetyLevel?api_key=%7B%7D&format=%7B%7D&hidden=%7B%7D&photo_id=%7B%7D&safety_level=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set the safety level of a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44bc789b-4a7a-4437-9621-c3351dfbc969"
            }
          ]
        },
        {
          "id": "5ef4e885-de66-46d2-8f43-8ad4c48a8f6a",
          "name": "postRestMethodFlickr.photos.settags",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.setTags?api_key=%7B%7D&photo_id=%7B%7D&tags=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set the tags for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fec08e5e-38e9-4648-a311-75513ff5f33d"
            }
          ]
        },
        {
          "id": "e7d2aedc-c823-4cf4-9c03-41cd92b9ebf0",
          "name": "postRestMethodFlickr.photos.comments.addcomment",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.comments.addComment?api_key=%7B%7D&comment_text=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add comment to a photo as the currently authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "271c3897-1eb1-42a3-a2f6-912b61097e4c"
            }
          ]
        },
        {
          "id": "066698fd-745a-4a06-8fb9-da48d70f2b79",
          "name": "postRestMethodFlickr.photos.comments.deletecomment",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.comments.deleteComment?api_key=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delete comment as the currently authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61016978-6ba6-4dda-93c2-d2f754afbea8"
            }
          ]
        },
        {
          "id": "6afd2610-4970-44ab-8f54-7a807932edf8",
          "name": "postRestMethodFlickr.photos.comments.editcomment",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.comments.editComment?api_key=%7B%7D&comment_id=%7B%7D&comment_text=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Edit the text of a comment as the currently authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1807f09d-0eb9-40c6-8966-c24d71247345"
            }
          ]
        },
        {
          "id": "e10bd939-5572-45ef-ae46-2e8f290eb947",
          "name": "getRestMethodFlickr.photos.comments.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.comments.getList?api_key=%7B%7D&format=%7B%7D&max_comment_date=%7B%7D&min_comment_date=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the comments for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc4b8690-6a0b-42f8-9ecf-1b7c591e05cd"
            }
          ]
        },
        {
          "id": "b37abf8d-9883-48dd-aa3b-4ca7698c1b84",
          "name": "getRestMethodFlickr.photos.comments.getrecentforcontacts",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.comments.getRecentForContacts?api_key=%7B%7D&contacts_filter=%7B%7D&date_lastcomment=%7B%7D&extras=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return the list of photos belonging to your contacts that have been commented on recently."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8417de4b-2f19-4c4d-ac96-bd0e411e7f27"
            }
          ]
        },
        {
          "id": "17faad37-eeef-480b-85d1-ada43526d7bd",
          "name": "postRestMethodFlickr.photos.geo.batchcorrectlocation",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.geo.batchCorrectLocation?accuracy=%7B%7D&api_key=%7B%7D&lat=%7B%7D&lon=%7B%7D&place_id=%7B%7D&woe_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Correct the places hierarchy for all the photos for a user at a given latitude, longitude and accuracy. Batch corrections are processed in a delayed queue so it may take a few minutes before the changes are reflected in a user's photos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a9ac833-b00f-4464-be7e-9b70d7659160"
            }
          ]
        },
        {
          "id": "5cf2c317-0b83-44a6-b910-5fd62e470bd4",
          "name": "postRestMethodFlickr.photos.geo.correctlocation",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.geo.correctLocation?api_key=%7B%7D&photo_id=%7B%7D&place_id=%7B%7D&woe_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Corrects a photo's location."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d0b10c0-8ff0-484d-91f1-759c8c271cbc"
            }
          ]
        },
        {
          "id": "80aaa275-d4dd-4372-94bb-2a5e1d8dc4f3",
          "name": "getRestMethodFlickr.photos.geo.getlocation",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.geo.getLocation?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the geo data (latitude and longitude and the accuracy level) for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "867fe585-de3d-4f3e-af2e-f55d560a633a"
            }
          ]
        },
        {
          "id": "22b81799-ef49-4808-adb0-8f20e3d6712d",
          "name": "getRestMethodFlickr.photos.geo.getperms",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.geo.getPerms?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get permissions for who may view geo data for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "648948f2-ae46-4160-9eef-704ed243a5b1"
            }
          ]
        },
        {
          "id": "57498d69-ba75-4e84-a7bc-f57c05627cdd",
          "name": "getRestMethodFlickr.photos.geo.photosforlocation",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.geo.photosForLocation?accuracy=%7B%7D&api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&lat=%7B%7D&lon=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of photos for the calling user at a specific latitude, longitude and accuracy"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e06847e6-8b96-4609-8b60-159d04b8b1b1"
            }
          ]
        },
        {
          "id": "466a1c0b-8279-4f42-9e79-99d315e85e75",
          "name": "postRestMethodFlickr.photos.geo.removelocation",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.geo.removeLocation?api_key=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the geo data associated with a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a697230-183c-4a48-89fb-d5409d58bc44"
            }
          ]
        },
        {
          "id": "f1fb8f8f-8f0c-4f41-a19f-fa215a0091cc",
          "name": "postRestMethodFlickr.photos.geo.setcontext",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.geo.setContext?api_key=%7B%7D&context=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Indicate the state of a photo's geotagginess beyond latitude and longitude. Note : photos passed to this method must already be geotagged (using the flickr.photos.geo.setLocation method)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "635aa555-0a84-422a-9393-f7aad2c74024"
            }
          ]
        },
        {
          "id": "0a088ef9-7706-4221-9363-9ec9b02a1ce0",
          "name": "postRestMethodFlickr.photos.geo.setlocation",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.geo.setLocation?accuracy=%7B%7D&api_key=%7B%7D&context=%7B%7D&format=%7B%7D&lat=%7B%7D&lon=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the geo data (latitude and longitude and, optionally, the accuracy level) for a photo. Before users may assign location data to a photo they must define who, by default, may view that information. Users can edit this preference at http://www.flickr.com/account/geo/privacy/. If a user has not set this preference, the API method will return an error."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d4b1cc3-f656-4610-a730-d6ec44fd61b5"
            }
          ]
        },
        {
          "id": "7e8c38f4-7f3d-4209-8a21-d1cd987db4df",
          "name": "getRestMethodFlickr.photos.geo.setperms",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.geo.setPerms?api_key=%7B%7D&is_contact=%7B%7D&is_family=%7B%7D&is_friend=%7B%7D&is_public=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Set the permission for who may view the geo data associated with a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af0271fd-cf29-4c8c-8fe9-720b42b26112"
            }
          ]
        },
        {
          "id": "98b49d30-3730-4fe1-8ef6-dfcf126ce167",
          "name": "getRestMethodFlickr.photos.licenses.getinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.licenses.getInfo?api_key=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches a list of available photo licenses for Flickr."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9bfd4d93-8b07-407d-9ddb-28c7246a9a0e"
            }
          ]
        },
        {
          "id": "31be77ba-2127-4e2d-acc6-9fc79ea03884",
          "name": "postRestMethodFlickr.photos.licenses.setinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.licenses.setInfo?api_key=%7B%7D&license_id=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the license for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a050209-fb0c-416f-b04d-1f670deb62ae"
            }
          ]
        },
        {
          "id": "dbcebd5f-8de9-43be-b5b7-5d0218190101",
          "name": "postRestMethodFlickr.photos.notes.add",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.notes.add?api_key=%7B%7D&format=%7B%7D&note_h=%7B%7D&note_text=%7B%7D&note_w=%7B%7D&note_x=%7B%7D&note_y=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a note to a photo. Coordinates and sizes are in pixels, based on the 500px image size shown on individual photo pages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4280273a-cba7-42a9-a64c-e17d7ff31ba9"
            }
          ]
        },
        {
          "id": "12063227-7ed7-42d1-9f0b-61dd435d84e0",
          "name": "postRestMethodFlickr.photos.notes.delete",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.notes.delete?api_key=%7B%7D&note_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a note from a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa933014-4e28-47a5-b541-52a64304d079"
            }
          ]
        },
        {
          "id": "7853fafe-a1a6-43c5-a853-a2321f1154f7",
          "name": "postRestMethodFlickr.photos.notes.edit",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.notes.edit?api_key=%7B%7D&note_h=%7B%7D&note_id=%7B%7D&note_text=%7B%7D&note_w=%7B%7D&note_x=%7B%7D&note_y=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Edit a note on a photo. Coordinates and sizes are in pixels, based on the 500px image size shown on individual photo pages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a4de276-f752-479b-bb29-a8587e09c258"
            }
          ]
        },
        {
          "id": "941e220b-5e67-4eca-b988-90b7ff2944ca",
          "name": "postRestMethodFlickr.photos.people.add",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.people.add?api_key=%7B%7D&person_h=%7B%7D&person_w=%7B%7D&person_x=%7B%7D&person_y=%7B%7D&photo_id=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a person to a photo. Coordinates and sizes are in pixels, based on the 500px image size shown on individual photo pages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb17e8ef-7405-4e1f-961d-629d6b9ca234"
            }
          ]
        },
        {
          "id": "7268c933-c6a5-48cb-a070-13c421a51063",
          "name": "postRestMethodFlickr.photos.people.delete",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.people.delete?api_key=%7B%7D&photo_id=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a person from a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8febd40-a0ee-4034-980d-f90d67ca1d4c"
            }
          ]
        },
        {
          "id": "ae0a0d15-4a2d-47c0-af0b-747c25acd0d1",
          "name": "postRestMethodFlickr.photos.people.deletecoords",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.people.deleteCoords?api_key=%7B%7D&photo_id=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Remove the bounding box from a person in a photo"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4276b472-18e2-41d2-b0ad-86f36702c1f3"
            }
          ]
        },
        {
          "id": "16ad8492-fadc-4388-b36a-eb2947706eef",
          "name": "postRestMethodFlickr.photos.people.editcoords",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.people.editCoords?api_key=%7B%7D&person_h=%7B%7D&person_w=%7B%7D&person_x=%7B%7D&person_y=%7B%7D&photo_id=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Edit the bounding box of an existing person on a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d9911a3-7e16-4a80-bdb0-39c7c26b84fa"
            }
          ]
        },
        {
          "id": "858abd4c-cabe-451e-bf05-2c8146791ed1",
          "name": "getRestMethodFlickr.photos.people.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.people.getList?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of people in a given photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "535edcf4-e6af-486f-9285-5cec8fb3f984"
            }
          ]
        },
        {
          "id": "79d13299-23f3-4c45-9a1b-d30351a449e5",
          "name": "postRestMethodFlickr.photos.transform.rotate",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.transform.rotate?api_key=%7B%7D&degrees=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Rotate a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c04f23cb-bc28-40f7-aa7c-b3f0eec6e650"
            }
          ]
        },
        {
          "id": "85bdf645-0d5b-4be0-9b45-080626d38a3f",
          "name": "getRestMethodFlickr.photos.upload.checktickets",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.upload.checkTickets?api_key=%7B%7D&format=%7B%7D&tickets=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Checks the status of one or more asynchronous photo upload tickets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39f7155f-2fbf-4d03-bbaa-a312cf18aae7"
            }
          ]
        }
      ]
    },
    {
      "name": "Photosets",
      "item": [
        {
          "id": "8ed3d1e0-025f-4d73-b698-52ff6c78e90c",
          "name": "postRestMethodFlickr.photosets.addphoto",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.addPhoto?api_key=%7B%7D&photoset_id=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a photo to the end of an existing photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c61ec271-f26e-412c-8304-8a0bf9080dbc"
            }
          ]
        },
        {
          "id": "50da16ce-5651-411f-ab8d-8f8337eae8c4",
          "name": "postRestMethodFlickr.photosets.create",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.create?api_key=%7B%7D&description=%7B%7D&format=%7B%7D&primary_photo_id=%7B%7D&title=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new photoset for the calling user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc06b2a2-6c80-4a86-a099-72b098ccc7b0"
            }
          ]
        },
        {
          "id": "12aebeec-64ba-4efc-87f6-a31f37741535",
          "name": "postRestMethodFlickr.photosets.delete",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.delete?api_key=%7B%7D&photoset_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a new photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ffae88d9-4a4a-4474-8bae-1109d921635b"
            }
          ]
        },
        {
          "id": "2fdec478-2adb-4bbb-beca-60364abfd59b",
          "name": "postRestMethodFlickr.photosets.editmeta",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.editMeta?api_key=%7B%7D&description=%7B%7D&photoset_id=%7B%7D&title=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Modify the meta-data for a photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81fc6d79-e4d9-4ef6-b7e5-025eb84d70e1"
            }
          ]
        },
        {
          "id": "86374b90-8b7b-4d92-ad0c-f5837c8a7c65",
          "name": "postRestMethodFlickr.photosets.editphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.editPhotos?api_key=%7B%7D&photoset_id=%7B%7D&photo_ids=%7B%7D&primary_photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Modify the photos in a photoset. Use this method to add, remove and re-order photos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3346888b-1b21-4e48-a368-164bda49640e"
            }
          ]
        }
      ]
    }
  ]
}