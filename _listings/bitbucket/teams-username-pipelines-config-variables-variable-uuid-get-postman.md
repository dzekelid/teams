{
  "info": {
    "name": "Bitbucket Get Teams Username Pipelines Config Variables Variable Uu",
    "_postman_id": "7e176c20-ff47-41cb-b7ee-a5aed3d99350",
    "description": "Get teams username pipelines config variables variable uu",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "7fb79d50-ce03-40e9-90f5-453e208c74a2",
          "name": "getTeamsUsernamePipelinesConfigVariablesVariableUu",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "teams/:username/pipelines_config/variables/:variable_uuid"
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variable_uuid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get teams username pipelines config variables variable uu"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "054163f9-fe4b-46e5-b870-02b12966b01d"
            }
          ]
        }
      ]
    }
  ]
}