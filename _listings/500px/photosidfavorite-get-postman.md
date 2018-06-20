{
  "info": {
    "name": "500px Get Photos Favorite",
    "_postman_id": "f31c38cd-9897-4e0d-9f47-e710f0013ef3",
    "description": "Deletes the photo from User's favorite list.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blogs",
      "item": [
        {
          "id": "f88898cc-676a-459b-9dc7-c5401b626ef3",
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
              "id": "8beed322-2a0a-433e-a1a5-59d2c632599a"
            }
          ]
        },
        {
          "id": "dcf84feb-77de-4a09-b058-658c39993d07",
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
              "id": "07da31ec-0dfb-4ce1-8240-21fe74d99d48"
            }
          ]
        },
        {
          "id": "58395961-3978-4bd2-9441-9c7acc5d4f6d",
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
              "id": "8749b118-b9a1-4603-b2d1-9900130a9b5e"
            }
          ]
        },
        {
          "id": "60f9f69a-4e46-4eb5-bf2b-cf398d2ed33c",
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
              "id": "63e47f19-b53c-42a0-8fce-c4bb5f93808b"
            }
          ]
        },
        {
          "id": "d8b62917-bbbe-4db7-ae70-6add298b6118",
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
              "id": "9ade2c9f-6d56-433a-8e60-967bb8cabd9e"
            }
          ]
        },
        {
          "id": "7ccf5726-549b-4bc2-9c09-9a84864b94fe",
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
              "id": "a7a07185-aa09-42b3-9181-9f5085b2235f"
            }
          ]
        },
        {
          "id": "669a35e6-3767-4b75-b34d-1d83bd3984f7",
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
              "id": "1e780b15-393b-41b6-bb4a-ea6d365ba812"
            }
          ]
        }
      ]
    },
    {
      "name": "Collections",
      "item": [
        {
          "id": "14d2310b-1645-4b2f-a621-a82c55759381",
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
              "id": "291cf9f0-cffb-4587-b32c-a9e8de7047a5"
            }
          ]
        },
        {
          "id": "30f6c693-f690-484d-9780-ba5a0a8187ad",
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
              "id": "af5894f1-7109-4f95-85ff-a8c97ae60569"
            }
          ]
        },
        {
          "id": "1a5247bf-d702-4cd1-801f-ef95dfc20212",
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
              "id": "f577dcff-dbd6-48b0-b5a7-299851743174"
            }
          ]
        },
        {
          "id": "fe2c082e-07ae-4e41-b992-716573ef6e40",
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
              "id": "deb4de25-b96e-46fa-8d08-6720a8b389ce"
            }
          ]
        },
        {
          "id": "5c080f4f-e9dd-46a1-b4ba-327528e18fcd",
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
              "id": "e8123f10-2f50-4a7a-8f0a-e83873cbcdd3"
            }
          ]
        }
      ]
    },
    {
      "name": "Comments",
      "item": [
        {
          "id": "081d242a-9e55-4c82-af27-2024ece26243",
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
              "id": "33a03f3c-66bf-46e3-ab29-d69724bd04fe"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "de4dedb8-06cf-4782-8881-901985197315",
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
              "id": "f4b143b9-7339-4414-a8e1-53a19499603d"
            }
          ]
        },
        {
          "id": "0aa2bf95-c629-4587-a872-80e399a8ca03",
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
              "id": "7ec8cf22-ef49-4648-869a-5b34b4e80d2b"
            }
          ]
        },
        {
          "id": "04d72349-7f2f-409d-8894-ac225894587a",
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
              "id": "8550ad80-5ddc-49cd-b397-3a8f050cede0"
            }
          ]
        },
        {
          "id": "a51e29f3-a650-4aab-9890-9bc74d4f4bbd",
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
              "id": "ce4c0eb6-1e61-4781-9436-6faf11fd156a"
            }
          ]
        },
        {
          "id": "0b8652d7-60b4-404c-8a0b-d3edb9bdbf8f",
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
              "id": "30a63b4d-3fc2-463e-b671-07d2eaf7f720"
            }
          ]
        },
        {
          "id": "9d3a94e1-0811-4b6e-847d-73935e8db8e7",
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
              "id": "69ed1a54-07eb-4fe9-8725-f60e8413b495"
            }
          ]
        },
        {
          "id": "2abfe323-024d-42d7-ba68-eff6b49c678e",
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
              "id": "c438c8b7-cadb-432a-b306-17f17e5eb2b7"
            }
          ]
        },
        {
          "id": "55847016-f5a9-413e-8222-0b179773fd99",
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
              "id": "952b73ff-13e1-4530-a251-a28132e5dc1f"
            }
          ]
        },
        {
          "id": "bcb49ded-4482-4de3-835b-6a7d00c2d365",
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
              "id": "0790112c-d5bc-44b9-ba87-6bbea2ba3295"
            }
          ]
        },
        {
          "id": "d911dc25-d280-45fa-9858-37f8c82ee32a",
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
              "id": "e5b53781-eb20-4eb5-a7f6-69570db16705"
            }
          ]
        },
        {
          "id": "de356ffb-6678-41d3-99a9-a7882049452c",
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
              "id": "0a196c9f-bdc4-4c79-8fd3-c24a44eedbc2"
            }
          ]
        },
        {
          "id": "a5c51981-b9e8-42bf-bf1b-5b6c29d4add2",
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
              "id": "df48e6b3-cf5a-4b8e-9a12-cab427f5538d"
            }
          ]
        },
        {
          "id": "05da4f8f-ee28-4afe-a00f-3572aede9347",
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
              "id": "623fcca1-0400-49c3-83f9-7d8e4bac82f1"
            }
          ]
        },
        {
          "id": "8ed6fcb1-436e-4a6f-9e1e-d65680c14e9b",
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
              "id": "06820509-a448-4d5f-b58d-809a7bf99eec"
            }
          ]
        },
        {
          "id": "d3a41a4c-594b-4e12-9bf0-bc3fdf340acf",
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
              "id": "48a617c9-98fb-4db2-83c0-5756ddee01a3"
            }
          ]
        },
        {
          "id": "e694aec5-1b29-4744-8400-3262e72ca3a5",
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
              "id": "4345ab7f-99fc-4c73-89f2-34891966c926"
            }
          ]
        },
        {
          "id": "6bba355d-ea6a-4fa3-9455-8339a97b0fc6",
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
              "id": "7630d108-9118-442e-b6b6-c8dcb8a61632"
            }
          ]
        },
        {
          "id": "21749ce9-7729-4c82-a481-d157bf1191e8",
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
              "id": "e5d047de-3d07-4e9c-9e90-1fa9697ac88a"
            }
          ]
        },
        {
          "id": "840dbf38-774e-4dd0-91df-5ba070b3de69",
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
              "id": "3f269b58-82e9-4866-b77f-df8d448e5ad7"
            }
          ]
        },
        {
          "id": "9cf1e33a-54f1-4c76-a15a-126f1239bc7b",
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
              "id": "ea8d42c4-85c9-4842-b271-c1c2247156d1"
            }
          ]
        },
        {
          "id": "83d4f529-25c8-413c-a6c4-c00cbfabc8f6",
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
              "id": "e92edecf-ef46-4234-8447-d84d89d4645d"
            }
          ]
        },
        {
          "id": "ff0ca117-53fa-4b2c-9a22-2541765adc84",
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
              "id": "03286ab3-6458-44d6-b1b7-f1637e421a2d"
            }
          ]
        },
        {
          "id": "8f17d037-db33-4672-9b46-41a305341f4b",
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
              "id": "92b469f5-f31d-4184-8f32-5cc69d9e191e"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "6e52a112-d3dc-4325-9b52-2140975960b8",
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
              "id": "1e96df75-c103-4932-97d9-b3a209c1d105"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "ea92ff1f-0a25-46a4-b9f0-c337ccf633f1",
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
              "id": "99e90c7a-2e32-4209-b1b8-f3cdd8fa14b4"
            }
          ]
        },
        {
          "id": "9e5d49a9-4cf0-495c-886b-6350594f9c62",
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
              "id": "1685eef9-ce52-4313-80c7-80d009c52e5d"
            }
          ]
        },
        {
          "id": "dfbf11aa-5d0b-4143-925d-29a171cbab3e",
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
              "id": "332d2753-c959-4fc2-a98a-da3e176dc2bf"
            }
          ]
        },
        {
          "id": "c8ce11b3-a7a3-4a78-bd25-4d2643ec63eb",
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
              "id": "ca046b73-82a4-41e3-bbb3-0b5643e2b05c"
            }
          ]
        },
        {
          "id": "49b2be6d-1f24-4cc3-833d-474f0e47b33e",
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
              "id": "01951f54-60fd-4259-a458-7172167a3c70"
            }
          ]
        },
        {
          "id": "7d56cc97-aa68-4882-913b-39458366a145",
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
              "id": "318323a3-f5c8-4897-8b36-ed0c769dd4aa"
            }
          ]
        },
        {
          "id": "f73a5b72-5f1f-4716-90d9-a4cfa695b3d2",
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
              "id": "9f8fc9a1-c951-4b4a-a2b6-042b87ab4947"
            }
          ]
        }
      ]
    }
  ]
}