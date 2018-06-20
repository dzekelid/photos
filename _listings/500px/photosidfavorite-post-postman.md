{
  "info": {
    "name": "500px Post Photos Favorite",
    "_postman_id": "23711e9b-1890-4db3-b03f-2a5661344216",
    "description": "Adds the photo to user's list of favorites.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blogs",
      "item": [
        {
          "id": "574ede0e-9dd5-459a-91f1-fc35cfb82c58",
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
              "id": "014b7a5c-fc6f-450f-9699-61ad58eae2c9"
            }
          ]
        },
        {
          "id": "4cebd938-1837-4b36-8f84-b11b856c2849",
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
              "id": "eacd0963-3edd-4a6e-b72b-dd9093ceebf7"
            }
          ]
        },
        {
          "id": "f2df3f99-9060-4273-b120-5252ad32fa1f",
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
              "id": "21407058-edc7-4a58-a21f-2abe5031e94d"
            }
          ]
        },
        {
          "id": "77a47d3a-63a2-46e6-a864-3544315ec6b2",
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
              "id": "7389e591-d839-4231-ac03-172c1fc45e5c"
            }
          ]
        },
        {
          "id": "c3d250d2-4766-4d9d-a41c-01ff1e4c5837",
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
              "id": "8a8f3b84-fd1f-4ce4-bbc3-2f0c1f9107e1"
            }
          ]
        },
        {
          "id": "d095bdeb-01f2-428d-84bb-3dc6320f724a",
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
              "id": "2f2c2844-0e1a-40b2-b0c6-cf0c80449713"
            }
          ]
        },
        {
          "id": "168f6fce-6792-4042-847c-c64404a89b67",
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
              "id": "c6f34f02-a41b-44ef-8fda-a94f17e66da3"
            }
          ]
        }
      ]
    },
    {
      "name": "Collections",
      "item": [
        {
          "id": "2d03bd28-80d1-41e9-9e2a-1e2493223c48",
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
              "id": "f37e424e-2262-457a-8cb5-58900e3eb6f6"
            }
          ]
        },
        {
          "id": "ddcea9e6-3f4e-4d4b-9d4e-be64ab974689",
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
              "id": "5d3a3f74-d3b6-429d-90bb-22666bcd1cec"
            }
          ]
        },
        {
          "id": "3884002f-aa0a-4c48-a4d6-5d670a3d312a",
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
              "id": "4b7ac3d9-389b-404a-b02c-f20bb0f40745"
            }
          ]
        },
        {
          "id": "6a558d19-8d78-4387-86da-687044e5abc3",
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
              "id": "1dfdebb0-8a46-4ce9-8b4b-3379f4e39b4b"
            }
          ]
        },
        {
          "id": "0d13016d-ba16-48e6-8c3a-c6a39c6b281c",
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
              "id": "6dc6ffdf-a930-4cc2-a679-565ba22ae2e4"
            }
          ]
        }
      ]
    },
    {
      "name": "Comments",
      "item": [
        {
          "id": "d367bda5-da76-4114-98a5-13be5c828ec0",
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
              "id": "369938e4-dad5-430f-a47c-9cb7ad751d61"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "e7afc701-729b-4314-94f2-f5803d02fb25",
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
              "id": "53ec7115-66ae-4627-8a63-44de7d376829"
            }
          ]
        },
        {
          "id": "216e93a5-e4af-41ef-94c3-01a3d8560f75",
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
              "id": "e0a2061e-1cb0-42f5-a8d7-a5d454367fdd"
            }
          ]
        },
        {
          "id": "c3906df6-898d-4aa8-bc08-e4e4d9cb7c9b",
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
              "id": "7d5bb100-1533-4dd6-99eb-1c00ea9fd3e8"
            }
          ]
        },
        {
          "id": "1998f06e-cc24-4bfb-b9c7-e01f03db0d9a",
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
              "id": "5df8abb7-9c60-451d-984b-ee27a30e5b9e"
            }
          ]
        },
        {
          "id": "3e16cb3c-e6be-4570-99f7-d05a8c5bdc18",
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
              "id": "8867a3c7-1d73-4c64-af5f-d3d2cac850d0"
            }
          ]
        },
        {
          "id": "fe76a66d-62f0-44ec-be13-a35879571b00",
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
              "id": "e012e0d3-c17f-43c7-8818-f40a729f6075"
            }
          ]
        },
        {
          "id": "9cea57bb-92cd-48ac-a59d-91a60b531950",
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
              "id": "ffe752de-8dad-4747-8e41-9ac600968a83"
            }
          ]
        },
        {
          "id": "72831232-fded-4451-b401-bc29ec6e75b9",
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
              "id": "27f46682-8d5a-48a4-bee3-e9c419b02625"
            }
          ]
        },
        {
          "id": "a376ca60-e7b5-4760-9447-f7f5067c0424",
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
              "id": "0a6cbf1a-bd83-4286-ae39-27b05ded62e5"
            }
          ]
        },
        {
          "id": "44e08833-36b6-4d60-a3d8-fd73d1a4afd2",
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
              "id": "01022414-16e1-4720-a59d-b89c0cdf2d6f"
            }
          ]
        },
        {
          "id": "257908ea-98c8-434b-84a4-c3861facac11",
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
              "id": "c3d3d22f-c7d7-416e-8e4e-aee027d49e9c"
            }
          ]
        },
        {
          "id": "f7efe0f7-40b2-4747-b199-bdcfda28acd1",
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
              "id": "8053254d-97db-4592-b651-9c4f10476991"
            }
          ]
        },
        {
          "id": "d5dd5e95-f3d3-4793-a319-5fd1dad44924",
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
              "id": "8d7b16f7-2536-4a02-9c9a-39050691756a"
            }
          ]
        },
        {
          "id": "9af2382d-50c7-4751-a012-8726660fd5e5",
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
              "id": "19b3640f-c219-4b50-9c1b-c95453e5bf6b"
            }
          ]
        },
        {
          "id": "7d90d9de-b5fa-4da3-a98a-d9c59267034e",
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
              "id": "d9fea364-8ef8-4ff4-a517-f53539ba1997"
            }
          ]
        },
        {
          "id": "69041854-235d-4270-b469-fabe8182f95f",
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
              "id": "556fdc10-95a1-44b5-b12f-d0feea7941d1"
            }
          ]
        },
        {
          "id": "9bfd888a-21c9-4326-b1ab-d15256ed6503",
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
              "id": "25cfcdf9-da0e-4e79-a65c-e56a2cb0e30a"
            }
          ]
        },
        {
          "id": "3b1fe6e4-e24f-4119-9cec-fdb425f9c4ab",
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
              "id": "3bb3715a-8c3c-43d7-82eb-5f894445d935"
            }
          ]
        },
        {
          "id": "513ae951-49b2-4cb2-b72b-301ace014611",
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
              "id": "0c14b7a1-6b57-45a0-930f-e41e3a40982c"
            }
          ]
        },
        {
          "id": "816979fc-a390-44a8-a92e-0c86166e8c71",
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
              "id": "e3effb41-29ac-4867-8c65-b25e774a1ae7"
            }
          ]
        },
        {
          "id": "a7423fa4-2c09-443e-83e8-4e451c11ab30",
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
              "id": "f1b1cd81-9aa9-40d1-a760-8d8ec7596237"
            }
          ]
        },
        {
          "id": "9c694b72-6287-49a0-9331-672251a68943",
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
              "id": "ef8c0e73-f2ad-46df-b005-6e5f34c218ac"
            }
          ]
        },
        {
          "id": "5f8867ed-6879-4906-8f42-a598ea7bf320",
          "name": "getPhotosFavorite",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id/favorite"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "rpp",
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
            "description": "Deletes the photo from User's favorite list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ad4f4fa-fb72-49a1-8a23-ce89e4c9e34d"
            }
          ]
        },
        {
          "id": "c4e2e849-9bf1-4a28-82c3-d1a77070752a",
          "name": "postPhotosFavorite",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id/favorite"
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
            "description": "Adds the photo to user's list of favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e4111123-3ef2-4e45-ab3a-cdd6a6048745"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "d8ef9204-120c-4276-bc6a-1f1b074b0c1d",
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
              "id": "e07d52d2-d768-4e06-9672-e21eb475edb1"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "7406c4af-c420-45e4-ad6a-3ca814510505",
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
              "id": "74b35417-f02b-46c0-8662-066ef3eb7365"
            }
          ]
        },
        {
          "id": "64799ce6-682f-459f-8b12-6e4f889ca924",
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
              "id": "63723281-63aa-40bc-ad7e-6f85878726f5"
            }
          ]
        },
        {
          "id": "beb2d5dd-d303-4b04-aefe-055c7fa20e34",
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
              "id": "e0a7abba-8acb-4b59-97db-76cca42970c1"
            }
          ]
        },
        {
          "id": "d8c631a5-6def-494f-86af-a63fee38236b",
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
              "id": "65a04e1f-e1eb-4a86-9fa5-0813c4e59ac3"
            }
          ]
        },
        {
          "id": "950d7f55-6e61-4598-b596-2ff0b38f42cf",
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
              "id": "c11b91fd-05c1-40ae-9937-f9666dab793a"
            }
          ]
        },
        {
          "id": "a746cd99-15eb-435e-b040-660183c29550",
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
              "id": "506ba754-d149-45ce-ba2d-63fe2630b9ea"
            }
          ]
        },
        {
          "id": "6f94f13b-a152-466b-bbeb-d51382719972",
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
              "id": "b1e717ff-b864-41cb-b81e-ae8a381a5b7c"
            }
          ]
        }
      ]
    }
  ]
}