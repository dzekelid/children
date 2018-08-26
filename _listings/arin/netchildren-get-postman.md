{
  "info": {
    "name": "Network API List Children",
    "_postman_id": "abfc2979-b8a5-46b7-ace5-2221ca53efa8",
    "description": "lists the child networks of a given network.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Networks",
      "item": [
        {
          "id": "b6c0f08d-e36a-4d34-b296-052d1b7603c7",
          "name": "nets",
          "request": {
            "url": "http://example.com/api/nets?handle=handle&name=name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Networks"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97d5f994-5278-4be3-8acb-33336fc273cf"
            }
          ]
        }
      ]
    },
    {
      "name": "POCs",
      "item": [
        {
          "id": "4b748dec-d34f-40b3-8529-d1e06f9b6627",
          "name": "netsPocs",
          "request": {
            "url": "http://example.com/api/net/pocs",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "lists the POCs associated with a given network."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a5ac926-c344-4bfa-a0b2-12bc0533209c"
            }
          ]
        }
      ]
    },
    {
      "name": "Parent",
      "item": [
        {
          "id": "f69f3dae-d4ab-40c2-aa4f-d5f4681d5df6",
          "name": "netParent",
          "request": {
            "url": "http://example.com/api/net/parent",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "lists the parent network of a given network."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74b5d17b-bcbb-4300-bf6c-8900f8f5152f"
            }
          ]
        }
      ]
    },
    {
      "name": "Children",
      "item": [
        {
          "id": "2218d203-867a-4e94-aa9c-d98b5609ecbc",
          "name": "netChildren",
          "request": {
            "url": "http://example.com/api/net/children",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "lists the child networks of a given network."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7080ce16-b48e-4616-bf3a-4c7117b93c1a"
            }
          ]
        }
      ]
    }
  ]
}