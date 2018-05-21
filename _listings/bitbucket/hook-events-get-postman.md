{
  "info": {
    "name": "Bitbucket Get Hook Events",
    "_postman_id": "ca4d92ed-611f-4b4d-b839-ca13582419ce",
    "description": "Returns the webhook resource or subject types on which webhooks can\nbe registered.\n\nEach resource/subject type contains an `events` link that returns the\npaginated list of specific events each individual subject type can\nemit.\n\nThis endpoint is publicly accessible and does not require\nauthentication or scopes.\n\nExample:\n\n```\n$ curl https://api.bitbucket.org/2.0/hook_events\n\n{\n    \"repository\": {\n        \"links\": {\n            \"events\": {\n                \"href\": \"https://api.bitbucket.org/2.0/hook_events/repository\"\n            }\n        }\n    },\n    \"team\": {\n        \"links\": {\n            \"events\": {\n                \"href\": \"https://api.bitbucket.org/2.0/hook_events/team\"\n            }\n        }\n    },\n    \"user\": {\n        \"links\": {\n            \"events\": {\n                \"href\": \"https://api.bitbucket.org/2.0/hook_events/user\"\n            }\n        }\n    }\n}\n```",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "hook",
      "item": [
        {
          "id": "1fec18e8-b8e6-44f4-b769-4c158f5ae188",
          "name": "getHookEvents",
          "request": {
            "url": "http://api.bitbucket.org/2.0/hook_events",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the webhook resource or subject types on which webhooks can\nbe registered"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e20d9d3-6730-4556-9c8b-ee03fce8f99e"
            }
          ]
        }
      ]
    }
  ]
}