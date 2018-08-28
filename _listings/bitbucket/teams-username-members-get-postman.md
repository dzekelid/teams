{
  "info": {
    "name": "Bitbucket Get Teams Username Members",
    "_postman_id": "86464684-eb82-48cf-b61d-3692fa5b0a9b",
    "description": "All members of a team.\n\nReturns all members of the specified team. Any member of any of the\nteam's groups is considered a member of the team. This includes users\nin groups that may not actually have access to any of the team's\nrepositories.\n\nNote that members using the \"private profile\" feature are not included.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "3f736ec9-6150-42c1-8ff9-bd4c2ea89d8d",
          "name": "getTeamsUsernameMembers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "teams/:username/members"
              ],
              "variable": [
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
            "description": "All members of a team"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8d4a25d-636b-4163-b266-e14369382e31"
            }
          ]
        }
      ]
    }
  ]
}