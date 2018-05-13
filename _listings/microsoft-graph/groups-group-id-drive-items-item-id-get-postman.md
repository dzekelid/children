{
  "info": {
    "name": "Microsoft Graph API List Children Of A Drive Item",
    "_postman_id": "5b207de3-0dac-4453-9940-f6bab264dd8d",
    "description": "List children of a driveItem Return a collection of DriveItems in the children relationship of a DriveItem.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "0080881e-96c1-469d-bbe7-079e0656e684",
          "name": "ListChildrenOfADriveItem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:group-id/drive/items/:item-id"
              ],
              "variable": [
                {
                  "id": "group-id",
                  "value": "group-id",
                  "type": "string"
                },
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
              "code": 200,
              "name": "Response_200",
              "id": "74009e87-ae5a-4824-9d0d-7949f38ce9c6"
            }
          ]
        }
      ]
    }
  ]
}