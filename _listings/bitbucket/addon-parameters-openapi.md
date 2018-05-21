---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Parameters Add On
  description: Parameters addon
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /addon:
    delete:
      summary: Delete Add On
      description: Delete addon
      operationId: deleteAddon
      x-api-path-slug: addon-delete
      responses:
        200:
          description: OK
      tags:
      - Addon
    parameters:
      summary: Parameters Add On
      description: Parameters addon
      operationId: parametersAddon
      x-api-path-slug: addon-parameters
      responses:
        200:
          description: OK
      tags:
      - Addon
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---