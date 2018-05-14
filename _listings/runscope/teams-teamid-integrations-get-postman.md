{
  "info": {
    "name": "Runscope Get Teams Integrations",
    "_postman_id": "35bd2f75-0f64-40c5-b46d-86bae92b7ec6",
    "description": "Team integrations list",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "d5f83c39-f422-47e1-9344-ac2c069e691a",
          "name": "teams.teamId.integrations.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.runscope.com",
              "path": [
                "teams/:teamId/integrations"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "teamId",
                  "value": "teamId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Team integrations list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46fdd436-f167-410a-9564-13c1602ac8ee"
            }
          ]
        }
      ]
    }
  ]
}