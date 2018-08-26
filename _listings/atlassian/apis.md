---
name: Atlassian
x-slug: atlassian
description: Millions of users globally rely on Atlassian products every day for improving
  software development, project management, collaboration, and code quality.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
x-kinRank: "8"
x-alexaRank: "1656"
tags: Children
created: "2018-08-25"
modified: "2018-08-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/children/master/_listings/atlassian/apis.md
specificationVersion: "0.14"
apis:
- name: The Confluence Cloud REST API - Get content children
  x-api-slug: contentidchild-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/children/master/_listings/atlassian/contentidchild-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/children/master/_listings/atlassian/contentidchild-get-openapi.md
- name: The Confluence Cloud REST API - Get content children by type
  x-api-slug: contentidchildtype-get
  description: "Returns all children of a given type, for a piece of content. \nA
    piece of content has different types of child content, depending on its type:\n\n-
    `page`: child content is `page`, `comment`, `attachment`\n- `blogpost`: child
    content is `comment`, `attachment`\n- `attachment`: child content is `comment`\n-
    `comment`: child content is `attachment`\n\nCustom content types that are provided
    by apps can also be returned.\n\nNote, this method only returns direct children.
    To return children at all \nlevels, use [Get descendants by type](#api-content-id-descendant-type-get).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: 'View' permission for the space, \nand permission to view the content
    if it is a page."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/children/master/_listings/atlassian/contentidchildtype-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/children/master/_listings/atlassian/contentidchildtype-get-openapi.md
x-common:
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/platform/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/confluence/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/software/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/service-desk/swagger.v3.json
- type: x-website
  url: http://atlassian.com/
- type: x-website
  url: http://www.atlassian.com
- type: x-api-gallery
  url: http://att.dev.program.api.gallery.streamdata.io
- type: x-api-stack
  url: http://atlassian.stack.network
- type: x-blog
  url: http://blogs.atlassian.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/atlassian
- type: x-crunchbase
  url: http://www.crunchbase.com/company/atlassian
- type: x-email
  url: copyright@atlassian.com
- type: x-email
  url: trademarks@atlassian.com
- type: x-email
  url: sales@atlassian.com
- type: x-email
  url: ar_enterprise@atlassian.com
- type: x-email
  url: privacy@atlassian.com
- type: x-email
  url: eudatarep@atlassian.com
- type: x-email
  url: experts@atlassian.com
- type: x-email
  url: remittance@atlassian.com
- type: x-email
  url: ap@atlassian.com
- type: x-email
  url: procurement@atlassian.com
- type: x-github
  url: https://github.com/atlassian
- type: x-privacy-policy
  url: https://www.atlassian.com/legal/privacy-policy?_ga=2.188884514.868776184.1519225620-845241124.1519225620
- type: x-twitter
  url: https://twitter.com/atlassian
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---