---
{
  "authentication": "required", 
  "description": "Return details on an individual file within a release.  This doesnot actually return the contents of the file, just the associatedmetadata.", 
  "example_request": "GET /api/0/projects/the-interstellar-jurisdiction/pump-station/releases/88dc638c8ccb84e5b7c750da882232aa1b394ac1/files/2/ HTTP/1.1\nHost: sentry.io\nAuthorization: Bearer {base64-encoded-key-here}", 
  "example_response": "HTTP/1.1\nContent-Length: 219\nX-XSS-Protection: 1; mode=block\nContent-Language: en\nX-Content-Type-Options: nosniff\nVary: Accept-Language, Cookie\nAllow: GET, PUT, DELETE, HEAD, OPTIONS\nX-Frame-Options: deny\nContent-Type: application/json\n\n{\n  \"dateCreated\": \"2018-09-10T20:37:01.131Z\", \n  \"dist\": null, \n  \"headers\": {\n    \"Content-Type\": \"text/plain; encoding=utf-8\"\n  }, \n  \"id\": \"2\", \n  \"name\": \"/demo/readme.txt\", \n  \"sha1\": \"2ef7bde608ce5404e97d5f042f95f89f1c232871\", \n  \"size\": 12\n}", 
  "method": "GET", 
  "parameters": null, 
  "path_parameters": [
    {
      "description": "the slug of the organization the release belongs to.", 
      "name": "organization_slug", 
      "type": "string"
    }, 
    {
      "description": "the slug of the project to retrieve the file of.", 
      "name": "project_slug", 
      "type": "string"
    }, 
    {
      "description": "the version identifier of the release.", 
      "name": "version", 
      "type": "string"
    }, 
    {
      "description": "the ID of the file to retrieve.", 
      "name": "file_id", 
      "type": "string"
    }
  ], 
  "query_parameters": null, 
  "sidebar_order": 19, 
  "title": "Releases"
}
---