swagger: "2.0"
x-collection-name: VMWare
x-complete: 1
info:
  title: vRealize Operations 6
  description: todo-add-description
  version: 1.0.0
host: example.com
basePath: /suite-api/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/resources/{osResourceId}/relationships/children:
    post:
      summary: Add Child Resource to a Resource
      description: "This operation adds a child resource to a resource.  \n\nAPI documentation
        states that POST is additive while PUT is destructive (i.e. overwites existing
        relationships).\n\nJSON body includes an array of child objects to add.  \n\nThe
        call does not provide a lot of detail for failure, but it seems\nthat if you
        have an invalid UUID for a child or the child is already related\nthen it
        will fail with 400.\n\n204 is a successful call."
      operationId: ApiResourcesRelationshipsChildrenByOsResourceIdPost
      x-api-path-slug: apiresourcesosresourceidrelationshipschildren-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: osResourceId
      responses:
        200:
          description: OK
      tags:
      - Resources
      - OsResourceId
      - Relationships
      - Children