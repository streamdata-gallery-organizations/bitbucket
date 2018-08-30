{
  "info": {
    "name": "Bitbucket Get Hook Events Subject Type",
    "_postman_id": "f255b112-0682-4ea6-a8e6-91a5253bbf09",
    "description": "Returns a paginated list of all valid webhook events for the\nspecified entity.\n\nThis is public data that does not require any scopes or authentication.\n\nExample:\n\nNOTE: The following example is a truncated response object for the `team` `subject_type`.\nWe return the same structure for the other `subject_type` objects.\n\n```\n$ curl https://api.bitbucket.org/2.0/hook_events/team\n{\n    \"page\": 1,\n    \"pagelen\": 30,\n    \"size\": 21,\n    \"values\": [\n        {\n            \"category\": \"Repository\",\n            \"description\": \"Whenever a repository push occurs\",\n            \"event\": \"repo:push\",\n            \"label\": \"Push\"\n        },\n        {\n            \"category\": \"Repository\",\n            \"description\": \"Whenever a repository fork occurs\",\n            \"event\": \"repo:fork\",\n            \"label\": \"Fork\"\n        },\n        ...\n        {\n            \"category\": \"Repository\",\n            \"description\": \"Whenever a repository import occurs\",\n            \"event\": \"repo:imported\",\n            \"label\": \"Import\"\n        }\n    ]\n}\n```",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "hook",
      "item": [
        {
          "id": "cce66600-8ea1-4c3d-a6f2-32ef5d147082",
          "name": "getHookEventsSubjectType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "hook_events/:subject_type"
              ],
              "variable": [
                {
                  "id": "subject_type",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a paginated list of all valid webhook events for the\nspecified entity"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d150648f-db3b-4189-9bef-ed3b8d02f445"
            }
          ]
        }
      ]
    }
  ]
}