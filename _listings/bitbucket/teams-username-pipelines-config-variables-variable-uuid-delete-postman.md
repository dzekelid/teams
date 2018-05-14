{
  "info": {
    "name": "Bitbucket Delete Teams Username Pipelines Config Variables Variable Uu",
    "_postman_id": "4c4bcf92-1b21-4b82-926c-0d82ae5acc68",
    "description": "Delete teams username pipelines config variables variable uu",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "7af5077a-0290-41d8-8143-0ba92a19c710",
          "name": "deleteTeamsUsernamePipelinesConfigVariablesVariableUu",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete teams username pipelines config variables variable uu"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4fe557b-3479-429a-ac7b-5680d968c0a2"
            }
          ]
        }
      ]
    }
  ]
}