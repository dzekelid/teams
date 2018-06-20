{
  "info": {
    "name": "Bitbucket Get Teams Owner Projects Project Key",
    "_postman_id": "4ec2b361-32d2-49c5-8a11-136754cf9b27",
    "description": "Get teams owner projects project key",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "2f9ce695-e3a6-4707-a5de-b963ae78eb04",
          "name": "getTeamsOwnerProjectsProjectKey",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get teams owner projects project key"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40ab9f63-ceb2-4d83-9ba3-ecb823971b4c"
            }
          ]
        }
      ]
    }
  ]
}