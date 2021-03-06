swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /privileges:
    get:
      summary: Get the privileges information
      description: Get the privileges information
      operationId: getPrivilegeUsingGET
      x-api-path-slug: privileges-get
      responses:
        200:
          description: OK
      tags:
      - Privileges
    post:
      summary: Save the privileges information
      description: Save the privileges information
      operationId: savePrivilegeUsingPOST
      x-api-path-slug: privileges-post
      parameters:
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Privileges
  /privileges/{uuid}:
    put:
      summary: Update the privileges information
      description: Update the privileges information
      operationId: updatePrivilegeUsingPUT
      x-api-path-slug: privilegesuuid-put
      parameters:
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - Privileges
      - Uuid
    delete:
      summary: Delete the privileges information
      description: Delete the privileges information
      operationId: deletePrivilegeUsingDELETE
      x-api-path-slug: privilegesuuid-delete
      parameters:
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - Privileges
      - Uuid