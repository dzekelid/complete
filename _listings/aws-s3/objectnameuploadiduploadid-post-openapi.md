---
swagger: "2.0"
x-collection-name: AWS S3
x-complete: 0
info:
  title: AWS S3 Complete Multipart Upload
  version: 1.0.0
  description: This operation completes a multipart upload by assembling previously
    uploaded parts
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ObjectName?uploadId=UploadId:
    post:
      summary: Complete Multipart Upload
      description: This operation completes a multipart upload by assembling previously
        uploaded parts
      operationId: complete-multipart-upload
      x-api-path-slug: objectnameuploadiduploadid-post
      responses:
        200:
          description: OK
      tags:
      - Complete
      - Multipart
      - Upload
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