---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Confluence Cloud API Get content children
  description: "Returns a map of the direct children of a piece of content. A piece
    of content \nhas different types of child content, depending on its type. These
    are \nthe default parent-child content type relationships:\n\n- `page`: child
    content is `page`, `comment`, `attachment`\n- `blogpost`: child content is `comment`,
    `attachment`\n- `attachment`: child content is `comment`\n- `comment`: child content
    is `attachment`\n\nApps can override these default relationships. Apps can also
    introduce \nnew content types that create new parent-child content relationships.\n\nNote,
    the map will always include all child content types that are valid \nfor the content.
    However, if the content has no instances of a child content \ntype, the map will
    contain an empty array for that child content type.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: 'View' permission for the space, \nand permission to view the content
    if it is a page."
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /content/{id}/child:
    get:
      summary: Get content children
      description: "Returns a map of the direct children of a piece of content. A
        piece of content \nhas different types of child content, depending on its
        type. These are \nthe default parent-child content type relationships:\n\n-
        `page`: child content is `page`, `comment`, `attachment`\n- `blogpost`: child
        content is `comment`, `attachment`\n- `attachment`: child content is `comment`\n-
        `comment`: child content is `attachment`\n\nApps can override these default
        relationships. Apps can also introduce \nnew content types that create new
        parent-child content relationships.\n\nNote, the map will always include all
        child content types that are valid \nfor the content. However, if the content
        has no instances of a child content \ntype, the map will contain an empty
        array for that child content type.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: 'View' permission for the space, \nand permission to view the
        content if it is a page."
      operationId: com.atlassian.confluence.plugins.restapi.resources.ChildContentResource.getContentChildren_get
      x-api-path-slug: contentidchild-get
      parameters:
      - in: query
        name: expand
        description: A multi-value parameter indicating which properties of the children
          to expand, where:- `attachment` returns all attachments for the content
      - in: path
        name: id
        description: The ID of the content to be queried for its children
      - in: query
        name: parentVersion
        description: The version of the parent content to retrieve children for
      responses:
        200:
          description: OK
      tags:
      - Content
      - Children
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