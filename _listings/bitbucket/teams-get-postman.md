{
  "info": {
    "name": "Bitbucket Get Teams",
    "_postman_id": "9bcb1b6f-8b1c-4251-a319-3cb631bad130",
    "description": "Returns all the teams that the authenticated user is associated\nwith.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "c081ed9b-7ec9-4ff5-9ae3-3cf028438dce",
          "name": "getTeams",
          "request": {
            "url": "http://api.bitbucket.org/2.0/teams?role=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all the teams that the authenticated user is associated\nwith"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2b648fc-6742-4abc-b86d-6c65e0b0bfbd"
            }
          ]
        }
      ]
    }
  ]
}