{
  "info": {
    "name": "Microsoft Graph API List Children Of A Drive Item",
    "_postman_id": "392083f0-1ce3-4065-a7d8-5134b0c5052e",
    "description": "List children of a driveItem Return a collection of DriveItems in the children relationship of a DriveItem.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "d7deb684-21f9-4185-ba31-32780dae1439",
          "name": "ListChildrenOfADriveItem",
          "request": {
            "url": "http://graph.microsoft.com/me/drive/root/children",
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
              "id": "ec6df253-ae6c-4ce4-b9fe-9574fe8d48d8"
            }
          ]
        }
      ]
    }
  ]
}