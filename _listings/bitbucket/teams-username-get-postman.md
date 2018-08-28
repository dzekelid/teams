{
  "info": {
    "name": "Bitbucket Get Teams Username",
    "_postman_id": "f355e2eb-dcec-49d3-977c-b6bbacc20c11",
    "description": "Gets the public information associated with a team.\n\nIf the team's profile is private, `location`, `website` and\n`created_on` elements are omitted.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "d1d5cce2-6a98-4267-aa11-db2409dd53af",
          "name": "getTeamsUsername",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "teams/:username"
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the public information associated with a team"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6302eb96-c8cf-46b5-90a5-cdd7a0f498f3"
            }
          ]
        }
      ]
    }
  ]
}