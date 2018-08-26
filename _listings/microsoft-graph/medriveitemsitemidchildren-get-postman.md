{
  "info": {
    "name": "Microsoft Graph API List Children Of A Drive Item",
    "_postman_id": "6222757f-0b65-4e4d-9d97-cb53f13ec388",
    "description": "List children of a driveItem Return a collection of DriveItems in the children relationship of a DriveItem.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "f2d95963-5c65-4f84-8ce3-ed1932080196",
          "name": "ListChildrenOfADriveItem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/drive/items/:item-id/children"
              ],
              "variable": [
                {
                  "id": "item-id",
                  "value": "item-id",
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
              "id": "8f12f261-e503-444c-a658-413788ab7ae0"
            }
          ]
        }
      ]
    }
  ]
}