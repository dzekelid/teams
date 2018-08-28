{
  "info": {
    "name": "Bitbucket Get Teams Username Repositories",
    "_postman_id": "e63e0d8a-3c87-43e0-8c11-c770917cda08",
    "description": "All repositories owned by a user/team. This includes private\nrepositories, but filtered down to the ones that the calling user has\naccess to.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "fb731f34-1c79-4212-9a4d-39a3a2e083da",
          "name": "getTeamsUsernameRepositories",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "teams/:username/repositories"
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
            "description": "All repositories owned by a user/team"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08713ea0-488f-4c54-a5bb-e4ec9e467170"
            }
          ]
        }
      ]
    }
  ]
}