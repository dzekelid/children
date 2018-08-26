---
swagger: "2.0"
x-collection-name: Rat Genome Database
x-complete: 1
info:
  title: Rat Genome Database
  description: the-rgd-rest-api-provides-programmatic-access-to-information-and-annotation-stored-in-the-rat-genome-database
  termsOfService: http://rgd.mcw.edu/wg/citing-rgd
  contact:
    name: Rat Genome Database
    url: http://rgd.mcw.edu
    email: RGD.Data2@mcw.edu
  version: "1.1"
host: rest.rgd.mcw.edu
basePath: /rgdws
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /annotations/count/{accId}/{includeChildren}:
    get:
      summary: Returns annotation count for ontology accession ID
      description: ""
      operationId: getAnnotationCountByAccIdUsingGET
      x-api-path-slug: annotationscountaccidincludechildren-get
      parameters:
      - in: path
        name: accId
        description: Ontology term accession ID
      - in: path
        name: includeChildren
        description: 'true: return annotations for the term and children, false: return
          annotations for the term only'
      responses:
        200:
          description: OK
      tags:
      - ""
  /annotations/count/{accId}/{speciesTypeKey}/{includeChildren}:
    get:
      summary: Returns annotation count for ontology accession ID and speicies
      description: ""
      operationId: getAnnotationCountByAccIdAndSpeciesUsingGET
      x-api-path-slug: annotationscountaccidspeciestypekeyincludechildren-get
      parameters:
      - in: path
        name: accId
        description: Ontology term accession ID
      - in: path
        name: includeChildren
        description: 'true: return annotations for the term and children, false: return
          annotations for the term only'
      - in: path
        name: speciesTypeKey
        description: A list of species type keys can be found using the lookup service
      responses:
        200:
          description: OK
      tags:
      - ""
  /annotations/count/{accId}/{speciesTypeKey}/{includeChildren}/{objectType}:
    get:
      summary: Returns annotation count for ontology accession ID and object type
      description: ""
      operationId: getAnnotationCountByAccIdAndObjectTypeUsingGET
      x-api-path-slug: annotationscountaccidspeciestypekeyincludechildrenobjecttype-get
      parameters:
      - in: path
        name: accId
        description: Ontology term accession ID
      - in: path
        name: includeChildren
        description: 'true: return annotations for the term and children, false: return
          annotations for the term only'
      - in: path
        name: objectType
        description: A list of object types can be found using the lookup service
      - in: path
        name: speciesTypeKey
        description: A list of species type keys can be found using the lookup service
      responses:
        200:
          description: OK
      tags:
      - ""
  /annotations/{accId}/{speciesTypeKey}/{includeChildren}:
    get:
      summary: Returns a list annotations for an ontology term or a term and it's
        children
      description: ""
      operationId: getAnnotationsUsingGET
      x-api-path-slug: annotationsaccidspeciestypekeyincludechildren-get
      parameters:
      - in: path
        name: accId
        description: Ontology term accession ID
      - in: path
        name: includeChildren
        description: 'true: return annotations for the term and children, false: return
          annotations for the term only'
      - in: path
        name: speciesTypeKey
        description: A list of species type keys can be found using the lookup service
      responses:
        200:
          description: OK
      tags:
      - ""
---