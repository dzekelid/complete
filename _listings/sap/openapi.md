swagger: "2.0"
x-collection-name: SAP
x-complete: 1
info:
  title: SAP Translation Hub
  description: to-provide-users-of-software-in-a-global-market-with-texts-in-their-own-language-translations-are-required--sap-translation-hub-enables-you-to-draw-on-saps-translation-experience-across-multiple-products-and-languages-to-propose-translations-for-short-texts-
  contact:
    name: SAP Translation Hub team
    email: translationhub@sap.com
  version: 1.0.0
host: sandbox.api.sap.com
basePath: /translationhub/api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /collaborationRooms/{collaborationRoomId}/complete:
    post:
      summary: Completes a collaboration
      description: |-
        Sets a collaboration as completed
        - The login user must be a collaboration lead for the customer.
        - If there's already a supplier in the collaboration room, the collaboration must already or still be in process.
        - If there's already a completed collaboration with the same additive manufacturing supplier, part ID, and customer, this operation fails.
      operationId: sets-a-collaboration-as-completed-the-login-user-must-be-a-collaboration-lead-for-the-customer-if-th
      x-api-path-slug: collaborationroomscollaborationroomidcomplete-post
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Completes
      - Collaboration