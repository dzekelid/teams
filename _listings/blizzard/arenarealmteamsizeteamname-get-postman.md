{
  "info": {
    "name": "World of Warcraft Get Arena Realm Teamsize Teamname",
    "_postman_id": "693d4cb6-0803-47c1-8cc2-6eaae60206e7",
    "description": "Provides detailed arena team information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Character",
      "item": [
        {
          "id": "7f559064-fb58-484c-9ee5-d133994953aa",
          "name": "getCharacterRealmCharactername",
          "request": {
            "url": {
              "protocol": "http",
              "host": "us.battle.net",
              "path": [
                "api",
                "wow",
                "character/:realm/:characterName"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "characterName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "realm",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches a single character at a time through an HTTP GET request to a URL describing the character profile resource. By default, a basic dataset will be returned and with each request and zero or more additional fields can be retrieved. The core dataset returned includes the character's realm, name, level, last modified timestamp, thumbnail, race id, achievement points value, gender id and class id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "223538e9-65f8-41b9-b7d9-6c77f1883409"
            }
          ]
        }
      ]
    },
    {
      "name": "Guild",
      "item": [
        {
          "id": "d7a66885-ebde-4bfa-b217-fac2eb3908ba",
          "name": "getGuildRealmGuildname",
          "request": {
            "url": {
              "protocol": "http",
              "host": "us.battle.net",
              "path": [
                "api",
                "wow",
                "guild/:realm/:guildName"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "guildName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "realm",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches a single guild at a time through an HTTP GET request to a url describing the guild profile resource. By default, a basic dataset will be returned and with each request and zero or more additional fields can be retrieved. The core dataset returned includes the guild's name, level, faction and achievement points."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8959a08b-c922-4597-9f2e-6ea14d41ab41"
            }
          ]
        }
      ]
    },
    {
      "name": "Realm",
      "item": [
        {
          "id": "92fde3b6-4f9b-467c-84d0-ba267331ffea",
          "name": "getRealmStatus",
          "request": {
            "url": "http://us.battle.net/api/wow/realm/status",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves realms status information. This information is limited to whether or not the realm is up, the type and state of the realm and the current population."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "212ef5a4-130b-45c8-9ae5-c0a970a2715e"
            }
          ]
        }
      ]
    },
    {
      "name": "Auction",
      "item": [
        {
          "id": "cfede538-e024-4100-95e4-b2678c28cda7",
          "name": "getAuctionDataRealm",
          "request": {
            "url": {
              "protocol": "http",
              "host": "us.battle.net",
              "path": [
                "api",
                "wow",
                "auction/data/:realm"
              ],
              "variable": [
                {
                  "id": "realm",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides a per-realm list of recently generated auction house data dumps. The current auctions data is represented as JSON structures containing auction data for the tree auctions houses available on each realm."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4ead29e-5a3d-45e4-a21b-fafef81e0e76"
            }
          ]
        }
      ]
    },
    {
      "name": "Item",
      "item": [
        {
          "id": "330eb4a8-6993-4546-ac60-e18596261980",
          "name": "getItemItem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "us.battle.net",
              "path": [
                "api",
                "wow",
                "item/:itemId"
              ],
              "variable": [
                {
                  "id": "itemId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides detailed item information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "136df157-fbdf-4a20-a954-d0e9f235ae7d"
            }
          ]
        }
      ]
    },
    {
      "name": "Arena",
      "item": [
        {
          "id": "0799bef8-6aa8-498d-bd33-3aff16a5e186",
          "name": "getArenaRealmTeamsizeTeamname",
          "request": {
            "url": {
              "protocol": "http",
              "host": "us.battle.net",
              "path": [
                "api",
                "wow",
                "arena/:realm/:teamSize/:teamName"
              ],
              "variable": [
                {
                  "id": "realm",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "teamName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "teamSize",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides detailed arena team information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2aa0bd3a-8b15-429b-8a6b-10c7684548a2"
            }
          ]
        }
      ]
    }
  ]
}