{
  "info": {
    "name": "Bitbucket Add Teams Username Hooks",
    "_postman_id": "75a6b52c-b5af-4a3e-ba42-d0c8490b3c01",
    "description": "Creates a new webhook on the specified team.\n\nTeam webhooks are fired for events from all repositories belonging to\nthat team account.\n\nNote that only admins can install webhooks on teams.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "59be5810-be73-425f-877d-4152836ac0e0",
          "name": "postTeamsUsernameHooks",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new webhook on the specified team"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5269cdc9-b2fb-4136-b57c-45aa88d0603f"
            }
          ]
        }
      ]
    }
  ]
}