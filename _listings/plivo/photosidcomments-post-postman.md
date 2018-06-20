{
  "info": {
    "name": "Codenvy Account API Post Photos Comments",
    "_postman_id": "7ed8462c-8ab4-4123-b829-79beac8c23fc",
    "description": "Creates a new comment for the photo.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blogs",
      "item": [
        {
          "id": "4832e3c7-c58a-4962-b20b-e89f0ab6ab21",
          "name": "creates-a-comment-for-the-story",
          "request": {
            "url": "http:///account/https://codenvy.com/api/blogs/:id/comments?body (required)=%7B%7D&id (required)=%7B%7D",
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
              "id": "24752c56-2107-4c19-95e8-af891cbef51f"
            }
          ]
        }
      ]
    },
    {
      "name": "Comments",
      "item": [
        {
          "id": "c8d73ee1-5c33-4145-9444-8e50b1b01fab",
          "name": "creates-a-reply-to-an-existing-comment-comments-can-only-be-nested-one-level-deep-you-cannot-reply-t",
          "request": {
            "url": "http:///account/https://codenvy.com/api/comments/:id/comments?body (required)=%7B%7D",
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
              "id": "e69d8c20-00d4-44c1-8443-4e1d4cf0ae1a"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "a3c07eb5-eaa8-44de-b74d-dd46c5fe8341",
          "name": "creates-a-new-comment-for-the-photo",
          "request": {
            "url": "http:///account/https://codenvy.com/api/photos/:id/comments?body (required)=%7B%7D&id (required)=%7B%7D",
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
              "id": "fcda5935-904f-46ea-b567-18205c0a0134"
            }
          ]
        }
      ]
    }
  ]
}