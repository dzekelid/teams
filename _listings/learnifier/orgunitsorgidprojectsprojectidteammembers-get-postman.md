{
  "info": {
    "name": "Learnifier Project team members",
    "_postman_id": "bc50b602-8641-477f-a912-1d51c5c7b0ec",
    "description": "Returns the project team members. A team member is a ....",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "c0c991b0-1ce7-4ba9-a449-c456b10c4652",
          "name": "orgunits.orgid.projects.projectid.teammembers.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "learnifier.com",
              "path": [
                "orgunits/:orgid/projects/:projectid/teammembers"
              ],
              "variable": [
                {
                  "id": "orgid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the project team members. A team member is a ...."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7681f6b8-91cb-4cb1-9114-8a9ac20ed1da"
            }
          ]
        }
      ]
    }
  ]
}