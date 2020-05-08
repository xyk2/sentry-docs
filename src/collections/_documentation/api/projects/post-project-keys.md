---
# This file is automatically generated from the API using `api-docs/generate.py`
# Do not manually this file.
{
  "api_path": "/api/0/projects/{organization_slug}/{project_slug}/keys/", 
  "authentication": "", 
  "description": "Create a new client key bound to a project.  The key's secret and\npublic key are generated by the server.", 
  "example_request": "POST /api/0/projects/the-interstellar-jurisdiction/pump-station/keys/ HTTP/1.1\nHost: sentry.io\nAuthorization: Bearer <token>\nContent-Type: application/json\n\n{\n  \"name\": \"Fabulous Key\"\n}", 
  "example_response": "HTTP/1.1 201 CREATED\nContent-Length: 906\nX-XSS-Protection: 1; mode=block\nContent-Language: en\nX-Content-Type-Options: nosniff\nVary: Accept-Language, Cookie\nAllow: GET, POST, HEAD, OPTIONS\nX-Frame-Options: deny\nContent-Type: application/json\n\n{\n  \"browserSdk\": {\n    \"choices\": [\n      [\n        \"latest\", \n        \"latest\"\n      ], \n      [\n        \"4.x\", \n        \"4.x\"\n      ]\n    ]\n  }, \n  \"browserSdkVersion\": \"4.x\", \n  \"dateCreated\": \"2018-11-06T21:20:07.941Z\", \n  \"dsn\": {\n    \"cdn\": \"https://sentry.io/js-sdk-loader/cec9dfceb0b74c1c9a5e3c135585f364.min.js\", \n    \"csp\": \"https://sentry.io/api/2/csp-report/?sentry_key=cec9dfceb0b74c1c9a5e3c135585f364\", \n    \"minidump\": \"https://sentry.io/api/2/minidump/?sentry_key=cec9dfceb0b74c1c9a5e3c135585f364\", \n    \"public\": \"https://cec9dfceb0b74c1c9a5e3c135585f364@sentry.io/2\", \n    \"secret\": \"https://cec9dfceb0b74c1c9a5e3c135585f364:4f6a592349e249c5906918393766718d@sentry.io/2\", \n    \"security\": \"https://sentry.io/api/2/security/?sentry_key=cec9dfceb0b74c1c9a5e3c135585f364\"\n  }, \n  \"id\": \"cec9dfceb0b74c1c9a5e3c135585f364\", \n  \"isActive\": true, \n  \"label\": \"Fabulous Key\", \n  \"name\": \"Fabulous Key\", \n  \"projectId\": 2, \n  \"public\": \"cec9dfceb0b74c1c9a5e3c135585f364\", \n  \"rateLimit\": null, \n  \"secret\": \"4f6a592349e249c5906918393766718d\"\n}", 
  "method": "POST", 
  "parameters": [
    {
      "description": "the name for the new key.", 
      "name": "name", 
      "type": "string"
    }
  ], 
  "path_parameters": [
    {
      "description": "the slug of the organization the client keys belong to.", 
      "name": "organization_slug", 
      "type": "string"
    }, 
    {
      "description": "the slug of the project the client keys belong to.", 
      "name": "project_slug", 
      "type": "string"
    }
  ], 
  "query_parameters": null, 
  "sidebar_order": 14, 
  "title": "Create a new Client Key", 
  "warning": null
}
---