{
  "info": {
    "name": "Bitbucket Delete Teams Username Hooks U",
    "_postman_id": "13b3a98a-9921-4ac7-81c5-fef298b9cdfc",
    "description": "Deletes the specified webhook subscription from the given team\naccount.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "cddfb6c2-b4da-4cf7-895d-d1d43ead70c2",
          "name": "deleteTeamsUsernameHooksU",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified webhook subscription from the given team\naccount"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "482414ee-21c4-4f03-aa4f-aada9076e48d"
            }
          ]
        }
      ]
    }
  ]
}