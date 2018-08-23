{
  "info": {
    "name": "500px Post Photos Comments",
    "_postman_id": "6a8cf16e-9f14-46e7-896d-65b56ddfe924",
    "description": "Creates a new comment for the photo.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blogs",
      "item": [
        {
          "id": "e40781b9-48c3-48ff-b1a1-6c149fb7d85e",
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
              "id": "17088763-7ab6-4421-b4eb-3c7e4d78a0b3"
            }
          ]
        },
        {
          "id": "bb26bf21-bac1-4c80-92aa-7c9ff63ab3f2",
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
              "id": "b4cb7a21-098c-4207-86f4-2f81cb15371c"
            }
          ]
        },
        {
          "id": "c5045ae8-6c4c-464b-b3d3-adcd4f683762",
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
              "id": "d28b7a30-c266-49c5-b8c0-dfbd90c214cf"
            }
          ]
        },
        {
          "id": "2791a89c-5cd9-44be-947b-c533380eb778",
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
              "id": "6e2842f9-0df5-4a83-97ba-e0f8d5771f5b"
            }
          ]
        },
        {
          "id": "a53d8e67-7319-46a9-bd33-f011ae5ba902",
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
              "id": "898677fc-4e17-4597-8360-22310ee2e28a"
            }
          ]
        },
        {
          "id": "204c52c7-4b71-4c52-9d10-66b55f3e7400",
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
              "id": "4126a28f-5029-4123-9bf7-f2bb1ce06c87"
            }
          ]
        },
        {
          "id": "48c36eec-963d-4b85-a01e-27e88fe2e92c",
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
              "id": "6fc6e3a0-731b-4a6f-a4fa-e88554b93400"
            }
          ]
        }
      ]
    },
    {
      "name": "Collections",
      "item": [
        {
          "id": "417aa56e-0d6e-4512-bb43-19fbabb928dc",
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
              "id": "f854da96-53ce-4172-a9d2-6bc1baf30c92"
            }
          ]
        },
        {
          "id": "7a876924-99dc-43f0-b243-c4f9f00776dd",
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
              "id": "a4767569-de5d-4c4a-9652-e0f5aa5b6666"
            }
          ]
        },
        {
          "id": "e7ec081c-6f6a-4fd0-93b5-5190f448a01a",
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
              "id": "573973da-757a-4c86-ba60-9635a3f01f0f"
            }
          ]
        },
        {
          "id": "0a701347-33fe-47b5-8952-ecbb111d98b4",
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
              "id": "8f43ac51-e43c-40b1-abbd-bae5f2298d4f"
            }
          ]
        },
        {
          "id": "f3034f38-c49c-4bb2-8dcf-065d7ffccb9c",
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
              "id": "796ac86a-71c7-49c6-99bc-516a97f296bb"
            }
          ]
        }
      ]
    },
    {
      "name": "Comments",
      "item": [
        {
          "id": "d62c9c47-de28-419e-b3bb-3c4db9647c7d",
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
              "id": "600d5507-30f4-4809-9ea1-19fbd5696601"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "76827b00-9282-43fb-a4f1-a3e024111627",
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
              "id": "775e1271-80d8-4b49-b039-e0a4518f0286"
            }
          ]
        },
        {
          "id": "e267bea6-897e-42ca-9bc3-68957c8d49b6",
          "name": "postPhotos",
          "request": {
            "url": "http://api.500px.com/v1/photos?aperture=%7B%7D&camera=%7B%7D&category=%7B%7D&description=%7B%7D&focal_length=%7B%7D&iso=%7B%7D&latitude=%7B%7D&lens=%7B%7D&longitude=%7B%7D&name=%7B%7D&privacy=%7B%7D&shutter_speed=%7B%7D&tags=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new photo on behalf of the user, and receive an upload key in exchange."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce0e0e27-7592-4d01-a988-2cdf68ec48a8"
            }
          ]
        },
        {
          "id": "416a25ef-5acb-4701-8c86-5b17e5d7ec85",
          "name": "getPhotos",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id?comments=%7B%7D&comments_page=%7B%7D&image_size=%7B%7D&tags=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns detailed information of a single photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28d052d7-481d-4da2-9edd-2993a0f1a16b"
            }
          ]
        },
        {
          "id": "aef71575-3297-4595-bcb4-04d4a7640a85",
          "name": "putPhotos",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id?add_tags: Comma-separated list of tags to add to this photos existing tags.=%7B%7D&aperture: Aperture value value for the photo, internally stored as string.=%7B%7D&camera: Make and model of the camera used to take this photo.=%7B%7D&category: Integer number of the category of the photo. See category mapping for exact values.=%7B%7D&crop: A hash containing keys x, x2, y, y2 and representing coordinates within which the thumbnail must be cropped. The crop is made using the top left corner as the origin. The points must be given relative to image size 4, an image of at most 900px=%7B%7D&description: Text description of the photo, up to 65535 characters in length.=%7B%7D&focal_length: Focal length value for the photo, internally stored as string.=%7B%7D&iso: Integer ISO value for the photo.=%7B%7D&latitude: Latitude of the location this photo was taken at represented by a decimal number.=%7B%7D&lens: Information about the lens used to take this photo.=%7B%7D&license_type: Integer number of the license type chosen for this photo. See license type mapping for exact values.=%7B%7D&longitude: Longitude of the location this photo was taken at represented by a decimal number.=%7B%7D&name: Title of the photo, up to 255 characters in length.=%7B%7D&nsfw: Boolean value indicating that the photo may contain not-safe-for-work content or content not suitable for minors.=%7B%7D&privacy: Integer value indicating that the photo should be shown (0) or hidden (1) on the users profile.=%7B%7D&remove_tags: Comma-separated list of tags to remove from this photos existing tags.=%7B%7D&shutter_speed: Shutter speed value for the photo, internally stored as string.=%7B%7D&tags: Comma-separated list of tags applicable to this photo.=%7B%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Allows the client application to update user-editable information on a photo.nnnResource URLnnhttps://api.500px.com/v1/photos/:idnnnnAuthenticationnnRequired; OAuth. The client application must use the OAuth access token issued for the owner of the photo to access this resouce.nnnParametersnnThe application must provide the ID of the photo to update in the URL of the request. The following parameters are recognized when included in the query string or POST body:nnnnname: Title of the photo, up to 255 characters in length.nndescription: Text description of the photo, up to 65535 characters in length.nncategory: Integer number of the category of the photo. See category mapping for exact values.nntags: Comma-separated list of tags applicable to this photo.nnadd_tags: Comma-separated list of tags to add to this photos existing tags.nnremove_tags: Comma-separated list of tags to remove from this photos existing tags.nnshutter_speed: Shutter speed value for the photo, internally stored as string.nnfocal_length: Focal length value for the photo, internally stored as string.nnaperture: Aperture value value for the photo, internally stored as string.nniso: Integer ISO value for the photo.nncamera: Make and model of the camera used to take this photo.nnlens: Information about the lens used to take this photo.nnlatitude: Latitude of the location this photo was taken at represented by a decimal number.nnlongitude: Longitude of the location this photo was taken at represented by a decimal number.nnnsfw: Boolean value indicating that the photo may contain not-safe-for-work content or content not suitable for minors.nnlicense_type: Integer number of the license type chosen for this photo. See license type mapping for exact values.nnprivacy: Integer value indicating that the photo should be shown (0) or hidden (1) on the users profile.nncrop: A hash containing keys x, x2, y, y2 and representing coordinates within which the thumbnail must be cropped. The crop is made using the top left corner as the origin. The points must be given relative to image size 4, an image of at most 900px on the larger side. The client application may skip this if the user does not wish to change photo thumbnail.nnnnImplementation detailsnnA parameter missing from the request will not be updated.  A parameter set to an empty string or null value will be interpreted as the user wishing to reset the value of the field to its default value.nnYou can use the add_tags and remove_tags parameters to manupulate a photos tags without having to send the complete list of tags in the request.nnnReturn formatnnA JSON object containing key photo, where photo is a Photo object in full format.nnnErrorsnnAll known errors cause the resource to return HTTP error code header together with a JSON array containing at least status and error keys describing the source of error.nnnn401: Invalid OAuth request: The request was refused because the OAuth signature is incorrect.nn404: Photo with ID not found: The photo ID provided is not known to the system.nn404: Photo with ID has been deleted: The photo has been deleted and can not be edited.nn404: Photo with ID belongs to a deactivated user: The photo belongs to a user that is no longer active and can not be edited.nn400: Bad photo category: An unrecognized photo category value has been provided.nn400: Bad license type: An unrecognized license type value has been provided."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d7b123aa-989f-41f3-9cef-afd9936a47e6"
            }
          ]
        },
        {
          "id": "a49bc37e-0990-49a6-adea-842dfa762004",
          "name": "deletePhotos",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id?id (required)=%7B%7D",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the photo from the Users library."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02a1439f-9484-41a8-a9df-83126a5ca141"
            }
          ]
        },
        {
          "id": "de9623de-fbc2-4436-97e7-03c0de7cffb5",
          "name": "getPhotosComments",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/comments?id (required)=%7B%7D&nested - Include this parameter to return the comments in nested format.=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a listing of twenty comments for the photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e8a5cc8-4e6d-4d76-b367-8e510a32f68f"
            }
          ]
        },
        {
          "id": "ce1e31e0-08da-40f0-bf15-aa5892744d1b",
          "name": "postPhotosComments",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/comments?body (required)=%7B%7D&id (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new comment for the photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b33150bc-ec50-4c23-a564-bd194c21d40a"
            }
          ]
        },
        {
          "id": "1df9a2ad-de56-4a6b-9cb1-e07ba7abe490",
          "name": "postPhotosFavorite",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/favorite?id (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds the photo to users list of favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b928728-afd6-4992-a82f-b83f1e0cd7b0"
            }
          ]
        },
        {
          "id": "29fa727f-63fe-4fb0-b2c6-11dbabc39a25",
          "name": "deletePhotosFavorite",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/favorite?id (required)=%7B%7D",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the photo to users list of favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31e2b029-c935-446c-9563-37466eb1ede8"
            }
          ]
        },
        {
          "id": "5c773a59-e862-4853-bd28-8b15bc36a140",
          "name": "getPhotosFavorites",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/favorites?page=%7B%7D&rpp=%7B%7D",
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
              "id": "56791cf6-2659-48e1-ba56-347571342157"
            }
          ]
        },
        {
          "id": "e14ac5af-63a7-4e80-b351-db48cdf1e8b6",
          "name": "postPhotosReport",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/report?id (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Allows to report a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c02c914a-e54f-4e44-976b-6822a786df3d"
            }
          ]
        },
        {
          "id": "54b1cfbc-75d3-4d29-a0ce-7c3a5f6bd402",
          "name": "postPhotosTags",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/tags?id (required)=%7B%7D&tags (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds tags to the photo. Accepts one or multiple coma separated tags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a523a97-216b-4ffd-ba88-f948bcf3f6ab"
            }
          ]
        },
        {
          "id": "cd3f88dc-5cc6-47f1-b8b8-641a72be166c",
          "name": "deletePhotosTags",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/tags?id (required)=%7B%7D&tags (required)=%7B%7D",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes tags from the photo. Accepts one or multiple coma separated tags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84748ea7-6a85-4be1-ac43-9bba64fb5fd4"
            }
          ]
        },
        {
          "id": "950574fa-e34f-4846-a759-942f43c62aaf",
          "name": "postPhotosVote",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/vote?id (required)=%7B%7D&vote (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Allows the user to vote for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0639d38c-b07b-4646-883c-db6bdfb3f3a4"
            }
          ]
        },
        {
          "id": "a4ca6377-c4b8-4671-be7f-6efd24d91b7a",
          "name": "getPhotosVotes",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/votes?page=%7B%7D&rpp=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all users that had liked this photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4d4a93c-f78f-4f9c-81c7-b74fb689b45d"
            }
          ]
        },
        {
          "id": "b98b816d-d93d-4b44-8b1c-320bc283c39e",
          "name": "getPhotosSearch",
          "request": {
            "url": "http://api.500px.com/v1/photos/search?comments_count u2014u00a0Sort by the number of comments, most commented first.=%7B%7D&created_at=%7B%7D&exclude=%7B%7D&favorites_count=%7B%7D&geo=%7B%7D&highest_rating=%7B%7D&image_size=%7B%7D&license_type -- Restrict the results to one or more license types.  Multiple types can be separated with a comma: license_type=1,4.=%7B%7D&only=%7B%7D&page=%7B%7D&rating=%7B%7D&rpp=%7B%7D&sort u2014u00a0Sort photos in the specified order. The following values are recognized:nnnn_score=%7B%7D&tag=%7B%7D&tags=%7B%7D&taken_at u2014u00a0Sort by the original date of the image extracted from metadata, most recent first (might not be available for all images).=%7B%7D&term=%7B%7D&times_viewed u2014u00a0Sort by the number of views, most viewed first.=%7B%7D&votes_count u2013 Sort by the number of votes, most voted on first.=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a listing of twenty (up to one hundred) photos from search results for a specified tag, keyword, or location."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9191fa17-23bb-43fb-843c-3f2fded65d43"
            }
          ]
        },
        {
          "id": "67c7fa13-435f-459e-b34c-5806de8c2d40",
          "name": "postPhotosUpload",
          "request": {
            "url": "http://api.500px.com/v1/photos/upload?aperture=%7B%7D&camera=%7B%7D&category=%7B%7D&description=%7B%7D&file=%7B%7D&file (required)  - Photo filename in JPG/JPEG, passed along with multipart/form-data.=%7B%7D&focal_length=%7B%7D&iso=%7B%7D&latitude=%7B%7D&lens=%7B%7D&longitude=%7B%7D&name=%7B%7D&privacy=%7B%7D&shutter_speed=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "This is a new photo upload endpoint. It is currently in beta.nCreate a new photo on behalf of the user and upload a file.nfile parameter is passed in multipart/form-data, other parameters are passed as query parametrs or multipart/form-data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a9f10c1-d71a-47b7-86fd-07957d7e0816"
            }
          ]
        },
        {
          "id": "f837caf9-461b-4025-a9c8-b0b162b5798c",
          "name": "getPhotos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id"
              ],
              "query": [
                {
                  "key": "comments",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "comments_page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "image_size",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tags",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns detailed information of a single photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2008f9e9-eaea-40a4-883d-b3fabdecab59"
            }
          ]
        },
        {
          "id": "8d40b58d-f8b6-452c-aadc-3337a3d0e308",
          "name": "putPhotos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id"
              ],
              "query": [
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ebee7e6-8d9d-41ce-b9b2-8b854c8f1e00"
            }
          ]
        },
        {
          "id": "32b4c306-0c48-4151-bc60-9d25808d07d2",
          "name": "deletePhotos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id"
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
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the photo from the User's library."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e73c305-3f52-4265-a84c-2e79a0df7523"
            }
          ]
        },
        {
          "id": "4969dc22-c621-4851-b418-8c01a7c7c632",
          "name": "getPhotosComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id/comments"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a listing of twenty comments for the photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67e4e0f3-82cb-469f-a405-2899f15f0eb0"
            }
          ]
        },
        {
          "id": "f3c5d7ac-de17-4052-aced-547136abb728",
          "name": "postPhotosComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id/comments"
              ],
              "query": [
                {
                  "key": "body",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new comment for the photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d50199b-cb43-4902-afe9-7fdd9fff17b9"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "80ac7bae-1bad-4134-ba36-818022f15cfe",
          "name": "postUpload",
          "request": {
            "url": "http://api.500px.com/v1/upload?access_key=%7B%7D&consumer_key=%7B%7D&file=%7B%7D&photo_id=%7B%7D&upload_key=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Allows an application to upload the photo file.nnNote that this endpoint is at the upload.500px.com domain, not the api.500px.com domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b425d1d-ad7b-4e94-b9a6-ff2febac698f"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "631078b4-cd73-4317-93b2-4ae60efdb944",
          "name": "getUsers",
          "request": {
            "url": "http://api.500px.com/v1/users",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the profile information for the current user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a6b4833-62a1-4849-836a-6e414cf63383"
            }
          ]
        },
        {
          "id": "4617b317-657c-44d4-96ec-b2d353e8fef1",
          "name": "getUsersFollowers",
          "request": {
            "url": "http://api.500px.com/v1/users/:id/followers?id (required)=%7B%7D&page=%7B%7D&rpp=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of users who follow the specified user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d48e5bb0-4156-47a6-853a-3175ec4d42f5"
            }
          ]
        },
        {
          "id": "e2bc8880-0305-4ece-8bab-21a02dbfe8fb",
          "name": "getUsersFriends",
          "request": {
            "url": "http://api.500px.com/v1/users/:id/friends?id (required)=%7B%7D&page=%7B%7D&rpp=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of friends for the specified user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a816a39-7679-4c6c-91b5-aec70fe8f5ec"
            }
          ]
        },
        {
          "id": "a35212ea-c332-40a5-9fd1-927472412591",
          "name": "postUsersFriends",
          "request": {
            "url": "http://api.500px.com/v1/users/:id/friends?id (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add the user to the list of followers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0cbaa28a-5fd3-4b2b-beca-a7a55226502f"
            }
          ]
        },
        {
          "id": "1ff1d1e9-04aa-4076-8adb-1aa8202ebd56",
          "name": "deleteUsersFriends",
          "request": {
            "url": "http://api.500px.com/v1/users/:id/friends?id (required)=%7B%7D",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the user from the list of followers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f63f3ee-29e7-4336-af0c-1f63aa2b5b19"
            }
          ]
        },
        {
          "id": "e674f838-6f27-445e-8cb8-b3368db1713b",
          "name": "getUsersSearch",
          "request": {
            "url": "http://api.500px.com/v1/users/search?page=%7B%7D&rpp=%7B%7D&term=%7B%7D&term (required)=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return listing of ten (up to one hundred) users from search results for a specified search term."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f0a47d5-a91d-409d-8fb4-f8fc70402a3b"
            }
          ]
        },
        {
          "id": "bdebd605-63da-4de2-9baf-d69f99761f14",
          "name": "getUsersShow",
          "request": {
            "url": "http://api.500px.com/v1/users/show?email=%7B%7D&id=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the profile information for a specified user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6cf2a2e4-6bc2-48b8-940d-49881e8a22a7"
            }
          ]
        }
      ]
    }
  ]
}