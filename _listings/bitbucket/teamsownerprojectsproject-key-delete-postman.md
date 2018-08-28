{
  "info": {
    "name": "Bitbucket Delete Teams Owner Projects Project Key",
    "_postman_id": "52a8b3f4-4d53-4f9c-bfee-80bea88eacca",
    "description": "Delete teams owner projects project key",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "6a557cf4-2bf4-4c99-af6f-cac3af3b742d",
          "name": "deleteTeamsOwnerProjectsProjectKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "teams/:owner/projects/:project_key"
              ],
              "variable": [
                {
                  "id": "owner",
                  "value": "owner",
                  "type": "string"
                },
                {
                  "id": "project_key",
                  "value": "project_key",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete teams owner projects project key"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a5f91a7-7f5b-4586-abc4-377d084140e4"
            }
          ]
        }
      ]
    }
  ]
}