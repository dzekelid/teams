{
  "info": {
    "name": "Bitbucket Get Teams Owner Projects",
    "_postman_id": "81a45790-527a-474d-9ee2-9dcf197be940",
    "description": "Get teams owner projects",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "cd1c1520-94bc-4298-a557-4b0d5c0e075f",
          "name": "getTeamsOwnerProjects",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "teams/:owner/projects/"
              ],
              "variable": [
                {
                  "id": "owner",
                  "value": "owner",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get teams owner projects"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "912242d2-e490-4bd9-871a-96adca88ac13"
            }
          ]
        }
      ]
    }
  ]
}