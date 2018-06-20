{
  "info": {
    "name": "Bitbucket Get Teams Username Pipelines Config Variables",
    "_postman_id": "1474c944-4f96-414c-8d6d-883675821f56",
    "description": "Get teams username pipelines config variables",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "08d06f99-ac87-41a8-bfd2-8d620683466e",
          "name": "getTeamsUsernamePipelinesConfigVariables",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "teams/:username/pipelines_config/variables/"
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get teams username pipelines config variables"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a8b0cd4-8afc-4c08-8898-f1c00f07cf4d"
            }
          ]
        }
      ]
    }
  ]
}