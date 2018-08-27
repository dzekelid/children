swagger: "2.0"
x-collection-name: ARIN
x-complete: 1
info:
  title: Reverse DNS API
  description: for-managing-reverse-dns-
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: www.arin.net
basePath: /regrws/core/v1
paths:
  /net/children:
    get:
      summary: List Children
      description: lists the child networks of a given network.
      operationId: netChildren
      x-api-path-slug: netchildren-get
      responses:
        200:
          description: OK
      tags:
      - Children