{
  "info": {
    "name": "Bitbucket Get Teams Username Followers",
    "_postman_id": "5e3656f3-7b56-44f2-bc16-aa3fa1e83b63",
    "description": "Returns the list of accounts that are following this team.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "6283b67b-f83d-472a-89e5-c07ec1360ab9",
          "name": "getTeamsUsernameFollowers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "teams/:username/followers"
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
            "description": "Returns the list of accounts that are following this team"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e225349d-9270-4cae-96cc-f22df22f857f"
            }
          ]
        }
      ]
    }
  ]
}