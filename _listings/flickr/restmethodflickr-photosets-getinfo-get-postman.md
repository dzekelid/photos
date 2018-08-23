{
  "info": {
    "name": "Flickr Photosets Get Info",
    "_postman_id": "a2ab28bd-b0c9-400d-bf32-7dbbd2d3e732",
    "description": "Gets information about a photoset.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "9400b278-e5c5-43d2-9a39-98e8c1979251",
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
              "id": "f73ba5f0-0058-4da4-8bf1-9b2918dcc1fb"
            }
          ]
        }
      ]
    },
    {
      "name": "Galleries",
      "item": [
        {
          "id": "8e5983d4-e791-4150-b77f-0e5d83dc581c",
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
              "id": "e182325e-4982-4183-976e-bc0f0429927b"
            }
          ]
        },
        {
          "id": "d1e89057-22bb-4924-a736-99e26f9ec38f",
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
              "id": "710dab06-1236-41dd-977b-13a29f3f3f0a"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "c67520c6-e598-4c38-9b38-1cea8014d102",
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
              "id": "33684758-8e09-4fb5-8b9c-4d81a7d8a260"
            }
          ]
        }
      ]
    },
    {
      "name": "Panda",
      "item": [
        {
          "id": "6b0ea4e7-43d6-42e5-8e98-4c493d30fb78",
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
              "id": "94ffb62e-3f5f-41cf-a5cd-e54ebfc82c38"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "75640055-1c7b-4357-9184-849d1ac9f035",
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
              "id": "f2d52d77-a63a-4c56-8acc-a89deceaaedb"
            }
          ]
        },
        {
          "id": "80834ef2-3497-4f23-84ee-c39dd2c11998",
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
              "id": "5c9272aa-4f65-4184-9881-5a55b83cb65e"
            }
          ]
        },
        {
          "id": "90d156c9-1302-4de8-9b0e-b82d821d4e59",
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
              "id": "da2c470a-e2a8-44a0-b758-a28244a2f3a7"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "c4f45664-864a-4339-856f-f62615d6af34",
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
              "id": "776c4a43-77c4-4889-a1ca-bcf928879696"
            }
          ]
        },
        {
          "id": "789330af-6447-4821-8c90-a7ed5e1d16cb",
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
              "id": "477a56ff-74f1-43eb-bd50-4a23432e626f"
            }
          ]
        },
        {
          "id": "c71c772c-d1fe-4829-ad90-822b2cdab739",
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
              "id": "b7441ee9-2f03-4fa6-99a0-6eccbf610ce2"
            }
          ]
        },
        {
          "id": "cb264bc5-c678-4636-847a-76f1d5619f32",
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
              "id": "8a6f2fbb-f80a-45f1-84c8-0838be4323ef"
            }
          ]
        },
        {
          "id": "425013a6-5fed-4184-b3b6-8aa53e06f05c",
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
              "id": "8a4c69aa-0d3c-4a07-952b-84ac63efe9f3"
            }
          ]
        },
        {
          "id": "a6824e17-b622-461a-b31a-f8a049cea7a2",
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
              "id": "4f85cd4f-7234-4a4f-a6da-28410a964352"
            }
          ]
        },
        {
          "id": "55d692b3-35ff-458a-87c5-e60235f3fa18",
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
              "id": "5dbf7197-2655-4bb5-9cc2-083f7bbc4b0d"
            }
          ]
        },
        {
          "id": "4ae01311-e6a7-45a3-9482-222db4d5ba46",
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
              "id": "34fd7f00-d9d6-415d-84c3-5e3e76c627ba"
            }
          ]
        },
        {
          "id": "63391a11-3c45-4f39-8d60-3d78b4bd4edd",
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
              "id": "a3a1faf1-77dd-4171-b213-dd6dc42329bb"
            }
          ]
        },
        {
          "id": "92295ceb-00b0-4d38-b75a-0bae346d1924",
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
              "id": "ad8d34c9-ad64-4c9a-8b2a-71ec16572199"
            }
          ]
        },
        {
          "id": "c2173256-29db-454f-8972-f13c1cd75d18",
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
              "id": "0b57f8eb-c2df-413b-96bc-fb00adb09bf9"
            }
          ]
        },
        {
          "id": "94174ecb-48b1-4b5c-b62e-b6e8c2f5b8b3",
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
              "id": "87e2c140-b95a-458f-9d7f-a77764a42e47"
            }
          ]
        },
        {
          "id": "ebfe5786-6935-4826-9dad-ac45363919a0",
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
              "id": "38019999-9989-4682-8773-40cfc1890220"
            }
          ]
        },
        {
          "id": "3204d37c-9c86-4b54-b2e8-1833cf5a1680",
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
              "id": "7c4ee815-d536-4409-9e4a-cd957f8914fc"
            }
          ]
        },
        {
          "id": "3f59ee69-83a6-40a3-889a-45e19d4fdb03",
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
              "id": "12f521f4-1515-4d4d-8c29-2bb63940ae62"
            }
          ]
        },
        {
          "id": "10a1089a-8363-464c-98ee-021101708cce",
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
              "id": "520ca728-922c-4359-af07-0c655dfb1a70"
            }
          ]
        },
        {
          "id": "461bba9b-e8af-4d6d-afc2-0c389aa57ea2",
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
              "id": "0439cc0d-8226-41ac-94ef-1985a3d9516e"
            }
          ]
        },
        {
          "id": "e9cd6023-c908-4071-90c3-a78c5bd591f5",
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
              "id": "8abf7348-6ba3-483f-8181-134009e4435b"
            }
          ]
        },
        {
          "id": "0953d42f-71dd-491f-b42d-b02aa5715e37",
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
              "id": "401d4d58-e513-46c1-9aec-6398985fcbbd"
            }
          ]
        },
        {
          "id": "26d454b9-35a6-4b01-8847-6c3d626d9fe1",
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
              "id": "a311298d-7bef-4972-9bf3-4bd7097d1006"
            }
          ]
        },
        {
          "id": "629d3e4e-2059-4fd1-baf6-058c8368cb77",
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
              "id": "48dab268-38f4-4b49-9e3d-2eb71be1406d"
            }
          ]
        },
        {
          "id": "23ee80ad-d4c9-4a70-8c82-858aeb446f91",
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
              "id": "340804a5-4883-4a36-aa16-83eb71186ca3"
            }
          ]
        },
        {
          "id": "dc63289e-5115-4ca4-98c4-c5c98e1e4126",
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
              "id": "becf9d55-6909-43bf-a973-2cea2424ad3a"
            }
          ]
        },
        {
          "id": "1a56fca1-c2d3-49c9-a401-08781c1cd808",
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
              "id": "27be0831-88da-4d8a-9a6e-5a6557d0ebe2"
            }
          ]
        },
        {
          "id": "848c7ccb-45a7-4d0b-8cd3-bf79a81bc022",
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
              "id": "86a24bb5-5e47-4fb5-8c66-c5db6862c940"
            }
          ]
        },
        {
          "id": "718abe69-7b4f-47ec-9893-50036263e7f6",
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
              "id": "30b84d9a-7368-4fcc-a33a-1509e333a7df"
            }
          ]
        },
        {
          "id": "a6daca57-9c2d-4385-8d89-cae8eaf9d1d2",
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
              "id": "81081f21-df2d-4d0b-96c8-4a77b70b18ce"
            }
          ]
        },
        {
          "id": "fd8328b4-c11e-4b34-af26-85987c263c27",
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
              "id": "1b7f3078-bb7e-4bbc-8e88-0028a33098ed"
            }
          ]
        },
        {
          "id": "a9c0cf13-308c-4b4c-8084-d8baf94feb1c",
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
              "id": "ede3e6dd-bb5e-49e3-ba6b-c2f34860553e"
            }
          ]
        },
        {
          "id": "02762d11-f387-4ef0-a743-627d10633c4b",
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
              "id": "362333fe-c10e-4309-921a-11a634bf55c4"
            }
          ]
        },
        {
          "id": "62a959f6-b891-483a-8beb-1331f7dae5e8",
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
              "id": "5d11456e-71e0-465d-9d8c-95a97e1a5b66"
            }
          ]
        },
        {
          "id": "ec953f12-4af6-4bc1-99be-6121dd4bc6a3",
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
              "id": "b3821249-1ad0-4121-b58a-3bf1a6292ac8"
            }
          ]
        },
        {
          "id": "223cedc9-a7bf-43b9-99ac-491cd98f5835",
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
              "id": "242dffc5-7bb7-4eda-8c50-8b9b73996c5f"
            }
          ]
        },
        {
          "id": "73eb6f8d-cf9d-4e55-abf2-a6bd11c2caec",
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
              "id": "720b4107-95b7-4930-89ce-5e75cad4217b"
            }
          ]
        },
        {
          "id": "054a89c5-db57-48f5-8585-e4a132acf1e1",
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
              "id": "14142816-dcbd-42bd-87bb-71b9a307e27d"
            }
          ]
        },
        {
          "id": "d19325de-b6dd-4d9c-804e-204582c53128",
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
              "id": "fd8ccca8-8219-402f-99bf-9c017efb6f14"
            }
          ]
        },
        {
          "id": "491fb983-e866-4721-9731-fb24aafc3268",
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
              "id": "ebf87a2e-0d84-46ac-87a7-e635ce19bc82"
            }
          ]
        },
        {
          "id": "b4684163-ec7f-4c88-8a81-184433710e18",
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
              "id": "d5ae144e-7750-4135-af4e-026e3d5e1fc4"
            }
          ]
        },
        {
          "id": "e1072ff9-c763-4264-8615-a4f013a4870f",
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
              "id": "9c4de77d-0a32-4b85-bd08-be17feae95e4"
            }
          ]
        },
        {
          "id": "7b1c2978-851b-4123-82f3-0fb80899c6b5",
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
              "id": "c00a7272-5e12-411a-8ae2-767805a1d380"
            }
          ]
        },
        {
          "id": "d32a8418-fbf2-41ad-9ff4-7282b9d7a578",
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
              "id": "7e436bea-8d5a-4316-83b8-253f1c52d059"
            }
          ]
        },
        {
          "id": "6b3df387-31be-4acf-8be5-dfd4e0b7da9b",
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
              "id": "ad8bdde5-7f27-45d8-bd97-e5c6433a5a94"
            }
          ]
        },
        {
          "id": "b776b75e-ae86-449a-abb2-ca19480bf2a2",
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
              "id": "e21b8358-1a6a-4362-b1ce-2a85a12edc51"
            }
          ]
        },
        {
          "id": "7a764192-0f91-42c2-9eb6-cc2be41ff8c0",
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
              "id": "f5499337-6730-435a-97af-47caf0d04e40"
            }
          ]
        },
        {
          "id": "87fe5c14-d57c-4329-a3f9-ec5e45dbfcfa",
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
              "id": "4eef4ac2-5865-4c3f-8461-f92c0ea5b4af"
            }
          ]
        },
        {
          "id": "5b89bfbd-1edb-412a-9300-9847315be790",
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
              "id": "cf52c752-8fd5-4e00-aebf-0a10f6d61c7a"
            }
          ]
        },
        {
          "id": "1104c90c-2931-4bfb-9388-ebe28ae638b1",
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
              "id": "49072a74-ffa9-42ab-b6e1-94d54fbb2043"
            }
          ]
        },
        {
          "id": "61515618-c23d-40d9-95a8-cabaec8806a1",
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
              "id": "630d0fa0-a505-4785-921a-3ed2de8f453e"
            }
          ]
        },
        {
          "id": "ed6c4566-9175-47de-bee3-8681011b33e7",
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
              "id": "a532b9f9-b13b-4574-85a6-d66463de70c6"
            }
          ]
        },
        {
          "id": "79859af5-8d2a-4d5e-94d5-751572c98f9d",
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
              "id": "713c4b68-523b-4d1d-91ab-6a4d29fde52c"
            }
          ]
        },
        {
          "id": "982f4a8a-d556-447e-a361-8cdb7dfd9a7b",
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
              "id": "753c3cf7-6788-4ce0-ad3f-5fb019d98ca6"
            }
          ]
        },
        {
          "id": "f163b5bc-8501-4aaa-b489-fb68583fa067",
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
              "id": "1060c4f2-1188-422a-8075-c046c61e060c"
            }
          ]
        }
      ]
    },
    {
      "name": "Photosets",
      "item": [
        {
          "id": "16bf1e41-c874-410d-8ebc-70f3f1d0043c",
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
              "id": "d57449b2-b1b2-4eb8-a4b8-0de8d4b527a5"
            }
          ]
        },
        {
          "id": "9c47e7fa-5fc6-4937-8420-4dd7c566f675",
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
              "id": "5eb2b498-dbbd-47bd-87b8-364e4608d6a8"
            }
          ]
        },
        {
          "id": "0704ae55-6619-41f8-a7c6-60772d3456b1",
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
              "id": "07d7bcbf-1900-4451-a475-711bd12af654"
            }
          ]
        },
        {
          "id": "973279ce-209f-4653-ba94-9e27abd6a694",
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
              "id": "5225f5ad-bf46-4efb-b3f8-a868ba451a81"
            }
          ]
        },
        {
          "id": "926bddf5-317e-42cd-8eb8-dc38ff9d8b42",
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
              "id": "c717e234-973f-43d7-8c15-bdd2145df66b"
            }
          ]
        },
        {
          "id": "ff5870d4-0385-48f8-8ee3-8c75e81708db",
          "name": "getRestMethodFlickr.photosets.getcontext",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.getContext?api_key=%7B%7D&format=%7B%7D&photoset_id=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns next and previous photos for a photo in a set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8b15ac0-009e-47b9-ae96-42ec1e5fe246"
            }
          ]
        },
        {
          "id": "4efa4963-3aa0-4d3b-95f0-0eeede2f389d",
          "name": "getRestMethodFlickr.photosets.getinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.getInfo?api_key=%7B%7D&format=%7B%7D&photoset_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5440a38f-7ed1-471a-9275-5846e7acae75"
            }
          ]
        }
      ]
    }
  ]
}