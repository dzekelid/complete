---
swagger: "2.0"
x-collection-name: AWS S3
x-complete: 1
info:
  title: No Title
  version: 1.0.0
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
---