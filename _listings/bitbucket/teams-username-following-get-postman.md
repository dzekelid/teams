{
  "info": {
    "name": "Bitbucket Get Teams Username Following",
    "_postman_id": "4f61a7b4-7d9d-4320-a26b-09271231cea8",
    "description": "Returns the list of accounts this team is following.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "30be0a55-bea3-4d0b-8768-104c76db8226",
          "name": "getTeamsUsernameFollowing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "teams/:username/following"
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
            "description": "Returns the list of accounts this team is following"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eec36bd1-fd1b-4c0d-bf59-01fc6c57f83c"
            }
          ]
        }
      ]
    }
  ]
}