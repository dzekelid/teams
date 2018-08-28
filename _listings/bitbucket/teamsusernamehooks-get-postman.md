{
  "info": {
    "name": "Bitbucket Get Teams Username Hooks",
    "_postman_id": "feb25bd2-85b4-4676-80ab-11fb85adc8dd",
    "description": "Returns a paginated list of webhooks installed on this team.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "f76593ac-40d0-4812-b8fe-5034c5e0f7aa",
          "name": "getTeamsUsernameHooks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "teams/:username/hooks"
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "username",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a paginated list of webhooks installed on this team"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57ab0c1d-6ab8-4a06-b5d3-7439079923c2"
            }
          ]
        }
      ]
    }
  ]
}