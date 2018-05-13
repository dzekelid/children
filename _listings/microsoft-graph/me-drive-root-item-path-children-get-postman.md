{
  "info": {
    "name": "Microsoft Graph API List Children Of A Drive Item",
    "_postman_id": "91081819-569b-4e63-ac81-31921566e345",
    "description": "List children of a driveItem Return a collection of DriveItems in the children relationship of a DriveItem.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "cb4c03b3-d171-42bb-a119-2cfdb644e7c2",
          "name": "ListChildrenOfADriveItem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/drive/root:/:item-path:/children"
              ],
              "variable": [
                {
                  "id": "item-path",
                  "value": "item-path",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "if-none-match",
                "value": "if-none-match",
                "description": "If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an HTTP 304 Not Modified response is returned",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List children of a driveItem Return a collection of DriveItems in the children relationship of a DriveItem"
          },
          "response": [
            {
              "status": "Successful Response",
              "code": 200,
              "name": "Response_200",
              "id": "4b6f7ff8-3f89-4130-99cd-757dc5f9d33a"
            }
          ]
        }
      ]
    }
  ]
}