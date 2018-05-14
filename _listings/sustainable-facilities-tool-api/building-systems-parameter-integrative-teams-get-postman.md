{
  "info": {
    "name": "Sustainable Facilities Tool API Building System Integrative Team",
    "_postman_id": "40dbd26f-d30b-4fa4-b127-96f3b2e8bd85",
    "description": "Returns a building system integrative team by parameter.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "c4966b87-882c-443b-b0cc-39ec9d20a143",
          "name": "returnBuildingSystemIntegrativeTeams",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.gov",
              "path": [
                "sftool",
                "v1",
                "building-systems/:parameter/integrative-teams"
              ],
              "variable": [
                {
                  "id": "parameter",
                  "value": "parameter",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a building system integrative team by parameter"
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
              "body": "[\r\n  {\r\n    \"id\": 66,\r\n    \"name\": \"name\"\r\n  }\r\n]",
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "42018cad-e5b1-48e2-b30c-a8a39b095d95"
            }
          ]
        }
      ]
    }
  ]
}