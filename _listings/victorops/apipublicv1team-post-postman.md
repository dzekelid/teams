{
  "info": {
    "name": "Victor Ops Add a team",
    "_postman_id": "53c17468-2e95-4a40-9f4a-3654c97a5d48",
    "description": "Add a team to your organization.\n\nThis API may be called a maximum of 15 times per minute.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Alerts",
      "item": [
        {
          "id": "81de378a-f430-47c8-9097-29894714a4cf",
          "name": "api_public.v1.alerts.uuid.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/alerts/:uuid"
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
                  "id": "uuid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the details of an alert that was sent VictorOps by you.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63686573-2e92-4a83-b905-ea88dc256258"
            }
          ]
        }
      ]
    },
    {
      "name": "Incidents",
      "item": [
        {
          "id": "f6a41764-8f39-442f-90a9-585aeab5b6dd",
          "name": "api_public.v1.incidents.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of the currently open, acknowledged and recently resolved incidents.\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9cccca7e-219a-4a9c-a36e-3959d3647db0"
            }
          ]
        },
        {
          "id": "8116faf9-5e96-4aa3-a78f-8b4a488e580a",
          "name": "api_public.v1.incidents.post",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents?No Name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new incident.\n\nThis call replicates the function of our\nmanual incident creation process.\nMonitoring tools and custom integrations\nshould be configured using our\nREST Endpoint.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff656239-7317-455a-99ca-27c6d30036a3"
            }
          ]
        },
        {
          "id": "a52b7537-9cc0-4542-9b18-6537a5fe254c",
          "name": "api_public.v1.incidents.ack.patch",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/ack?No Name=%7B%7D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75445fef-faa2-48a2-bc5e-9f612f73b06e"
            }
          ]
        },
        {
          "id": "9b020f30-d4ee-4472-947e-e27a29d234e8",
          "name": "api_public.v1.incidents.byUser.ack.patch",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/byUser/ack?No Name=%7B%7D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc7e5a70-f089-4c7d-bf6a-0b2b0d70ffcf"
            }
          ]
        },
        {
          "id": "15c7a98c-bcaf-41a0-9b50-c5ab1249bb2c",
          "name": "api_public.v1.incidents.byUser.resolve.patch",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/byUser/resolve?No Name=%7B%7D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74bc924a-7fe3-482d-8e0f-5bf7d5f02023"
            }
          ]
        },
        {
          "id": "62a8a8f1-7f87-43a3-a0c9-ff1d10b5fad5",
          "name": "api_public.v1.incidents.reroute.post",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/reroute?No Name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Reroute one or more incidents to one or more users and/or escalation policies"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2725ae37-a024-45f6-8ccf-d77cc4fa35b4"
            }
          ]
        },
        {
          "id": "3c2baa17-915e-426c-a58e-e9f831296aa5",
          "name": "api_public.v1.incidents.resolve.patch",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/resolve?No Name=%7B%7D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe9f89da-d2da-4564-aa6d-c1e979037f93"
            }
          ]
        }
      ]
    },
    {
      "name": "Oncall",
      "item": [
        {
          "id": "c15ef65d-8b9d-473b-a1ed-38bc8ec5574d",
          "name": "api_public.v1.oncall.current.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/oncall/current?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all on-call uesrs/teams for your organization.\n\nThis API may be called a maximum of 1 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46bc5bf8-8881-46c7-9674-1bb3ec880b79"
            }
          ]
        }
      ]
    },
    {
      "name": "Org",
      "item": [
        {
          "id": "eb137c32-a0f6-4d33-999f-c8245b6274c0",
          "name": "api_public.v1.org.routing_keys.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/org/routing-keys?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a list of routing keys and associated teams.\nThis API may be called a maximum of once a minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06bc1ba9-83cc-4b25-ad06-82aa5236a62f"
            }
          ]
        }
      ]
    },
    {
      "name": "Policies",
      "item": [
        {
          "id": "217a4c49-63a0-4d5b-b5f1-e961e7058f75",
          "name": "api_public.v1.policies.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/policies?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a list of escalation policy information.\nThis API may be called a maximum of once a minute"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61dee737-8881-43e9-9905-c7768f925e06"
            }
          ]
        },
        {
          "id": "fd67fbd2-618a-40b7-afc8-bf130ae449c1",
          "name": "api_public.v1.policies.types.contacts.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/policies/types/contacts?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the available contact types\n\ndescription: \"Email Address\", type: \"email\"\ndescription: \"Phone Number\", type: \"phone\"\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "505d757f-da4c-4ef3-905c-c58079350075"
            }
          ]
        },
        {
          "id": "06371983-0945-4b1c-abe3-f0aecf03c0de",
          "name": "api_public.v1.policies.types.notifications.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/policies/types/notifications?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the available notification types\n\ndescription: \"Send a push notification to all my devices\", type: \"push\"\ndescription: \"Send an email to an email address\", type: \"email\"\ndescription: \"Send an SMS to a phone number\", type: \"sms\"\ndescription: \"Make a phone call to a phone number\", type: \"phone\"\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3c854cd-8f7a-4fff-b7ff-edaf0826dc3f"
            }
          ]
        },
        {
          "id": "e40246ff-d734-4f10-b983-2fddf97a56f9",
          "name": "api_public.v1.policies.types.timeouts.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/policies/types/timeouts?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the available timeout values\n\ndescription: \"If still unacked after 1 minute\", type: 1\ndescription: \"If still unacked after 5 minutes\", type: 5\ndescription: \"If still unacked after 10 minutes\", type: 10\ndescription: \"If still unacked after 15 minutes\", type: 15\ndescription: \"If still unacked after 20 minutes\", type: 20\ndescription: \"If still unacked after 25 minutes\", type: 25\ndescription: \"If still unacked after 30 minutes\", type: 30\ndescription: \"If still unacked after 45 minutes\", type: 45\ndescription: \"If still unacked after 60 minutes\", type: 60\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73d648b7-6b4b-4a26-bfd0-d177326d8fc7"
            }
          ]
        },
        {
          "id": "827ac13b-a473-4495-960e-c2cf32543bdb",
          "name": "api_public.v1.policies.policy.oncall.user.patch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/policies/:policy/oncall/user"
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
                  "id": "policy",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "Replaces a currently on-call user in the escalation policy with another.  In many cases, the policy slug\nwill match the slug of the team that contains it.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f33587eb-2ea9-4288-89ad-51c2cae5388c"
            }
          ]
        }
      ]
    },
    {
      "name": "Profile",
      "item": [
        {
          "id": "4448b882-32c9-422e-b13f-271db44c66ad",
          "name": "api_public.v1.profile.username.policies.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies"
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
            "description": "Get all the paging policy steps for the user on the org associated with the API key\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dccabc42-400a-453b-8fd8-3cc2117abc56"
            }
          ]
        },
        {
          "id": "9176d61f-7b6c-4799-bbe5-72bba8efc5c1",
          "name": "api_public.v1.profile.username.policies.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "257ba354-2908-489d-be05-9358d6944f19"
            }
          ]
        },
        {
          "id": "71e730a3-696d-4ce5-84f5-4dfcaa3269fb",
          "name": "api_public.v1.profile.username.policies.step.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies/:step"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "step",
                  "value": "step",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a8e904b-f75d-4c18-b89f-39380aa2353e"
            }
          ]
        },
        {
          "id": "cf1b1874-98e5-4845-bccb-4af9319f490b",
          "name": "api_public.v1.profile.username.policies.step.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies/:step"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "step",
                  "value": "step",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6727ab16-c8ff-44fe-b95e-4b2f1fa9cbf3"
            }
          ]
        },
        {
          "id": "55e148ed-3786-483d-8829-8bd3a850e15c",
          "name": "api_public.v1.profile.username.policies.step.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies/:step"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "step",
                  "value": "step",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a rule for a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "442fa1dd-b444-4a22-ba46-7523072fc16d"
            }
          ]
        },
        {
          "id": "d088a140-c5ff-408e-ac48-5cd1c5e6c05e",
          "name": "api_public.v1.profile.username.policies.step.rule.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies/:step/:rule"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "step",
                  "value": "step",
                  "type": "string"
                },
                {
                  "id": "rule",
                  "value": "rule",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a rule from a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf06eec2-7657-4ed6-b65c-1dea82444549"
            }
          ]
        },
        {
          "id": "9c66c66f-d173-4567-96f6-4ddca56fd166",
          "name": "api_public.v1.profile.username.policies.step.rule.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies/:step/:rule"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "step",
                  "value": "step",
                  "type": "string"
                },
                {
                  "id": "rule",
                  "value": "rule",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a rule for a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24fb2f43-498b-4c6c-b5f5-8352c47dc60c"
            }
          ]
        },
        {
          "id": "8df10ccc-35b4-4de3-84a8-620622678d54",
          "name": "api_public.v1.profile.username.policies.step.rule.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies/:step/:rule"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "step",
                  "value": "step",
                  "type": "string"
                },
                {
                  "id": "rule",
                  "value": "rule",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a rule from a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ff18e46-3609-46be-a26a-bac9bff2c65d"
            }
          ]
        }
      ]
    },
    {
      "name": "Team",
      "item": [
        {
          "id": "86cb1939-e253-446b-aaac-1c77db48fcaa",
          "name": "api_public.v1.team.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/team?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of teams for your organization.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6e16b07-0484-41d7-a1d7-ca381aaf89b6"
            }
          ]
        },
        {
          "id": "3cd9d2d3-6904-4c89-9103-b11886851a6e",
          "name": "api_public.v1.team.post",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/team?No Name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a team to your organization.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "223cf35d-6c62-47ad-81ae-d12b58db8620"
            }
          ]
        }
      ]
    }
  ]
}