{
  "info": {
    "name": "Bitbucket Update Teams Username Hooks U",
    "_postman_id": "898d49c2-3446-4e76-a1c9-f98f4a7d5c77",
    "description": "Updates the specified webhook subscription.\n\nThe following properties can be mutated:\n\n* `description`\n* `url`\n* `active`\n* `events`",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "a328bcd1-1f7c-475e-99ad-a0b70c9a6c36",
          "name": "putTeamsUsernameHooksU",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "teams/:username/hooks/:uid"
              ],
              "variable": [
                {
                  "id": "uid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "username",
                  "value": "username",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the specified webhook subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c6f6219-2438-4ec8-83df-2e856a559327"
            }
          ]
        }
      ]
    }
  ]
}