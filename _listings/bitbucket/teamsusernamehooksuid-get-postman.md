{
  "info": {
    "name": "Bitbucket Get Teams Username Hooks U",
    "_postman_id": "0228230d-1801-4cb7-bf2a-a11b889b3f3b",
    "description": "Returns the webhook with the specified id installed on the given\nteam account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "00d497eb-07e5-4d90-8fe6-6592eaff1ff6",
          "name": "getTeamsUsernameHooksU",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the webhook with the specified id installed on the given\nteam account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1601980-832b-41b1-bc67-26c0429b7929"
            }
          ]
        }
      ]
    }
  ]
}