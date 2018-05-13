{
  "info": {
    "name": "Microsoft Graph API List Children Of A Drive Item",
    "_postman_id": "c6908d80-bead-4990-929d-2fde34dccb0c",
    "description": "List children of a driveItem Return a collection of DriveItems in the children relationship of a DriveItem.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "4de37c2f-7411-4ca4-9620-cbe34abf377f",
          "name": "ListChildrenOfADriveItem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "drives/:drive-id/items/:item-id/children"
              ],
              "variable": [
                {
                  "id": "drive-id",
                  "value": "drive-id",
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
              "status": "Successful Response",
              "code": 200,
              "name": "Response_200",
              "id": "d4daf04e-04b6-467f-bb96-db97890e7773"
            }
          ]
        }
      ]
    }
  ]
}