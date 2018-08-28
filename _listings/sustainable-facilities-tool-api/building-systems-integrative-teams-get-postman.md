{
  "info": {
    "name": "Sustainable Facilities Tool API Building System Integrative Teams",
    "_postman_id": "8a2af696-345a-41a4-9b26-40b6dc97f9e6",
    "description": "Returns all building system integrative teams.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "9cf8626a-c749-45a5-b8dd-339e4bced881",
          "name": "returnBuildingSystemIntegrativeTeams",
          "request": {
            "url": "http://api.data.gov/sftool/v1/building-systems/integrative-teams",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all building system integrative teams"
          },
          "response": [
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "[\r\n  {\r\n    \"id\": 196,\r\n    \"name\": \"name\"\r\n  }\r\n]",
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "fc718eb0-c6be-4c99-a39c-a92f8dac0a93"
            }
          ]
        }
      ]
    }
  ]
}