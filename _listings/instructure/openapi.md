swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Utility APIs
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/quizzes/quiz_id/submissions/{id}/complete:
    post:
      summary: Complete the quiz submission (turn it in).
      description: Complete the quiz submission (turn it in)..
      operationId: complete-the-quiz-submission-turn-it-in
      x-api-path-slug: coursescourse-idquizzesquiz-idsubmissionsidcomplete-post
      parameters:
      - in: query
        name: access_code
        description: Access code for the Quiz, if any
      - in: query
        name: attempt
        description: The attempt number of the quiz submission that should be completed
      - in: query
        name: validation_token
        description: The unique validation token you received when this Quiz Submission
          wasncreated
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Submissions
      - Id
      - Complete