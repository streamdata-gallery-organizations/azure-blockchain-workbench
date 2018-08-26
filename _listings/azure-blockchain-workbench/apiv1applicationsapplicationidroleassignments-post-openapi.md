---
swagger: "2.0"
x-collection-name: Azure Blockchain Workbench
x-complete: 0
info:
  title: Azure Blockchain Workbench Post Applications Roleassignments
  description: |-
    Creates a user-to-role mapping in the specified blockchain application. This method can only be performed by
                 users who are Workbench administrators.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/applications:
    get:
      summary: Get Applications
      description: |-
        Lists all blockchain applications to which a user has access in Workbench. Users who are Workbench administrators get
                     all blockchain applications. Non-Workbench administrators get all blockchain applications for which they have at least one
                     associated application role or an associated smart contract instance role.
      operationId: ApplicationsGet
      x-api-path-slug: apiv1applications-get
      parameters:
      - in: query
        name: enabled
        description: A Boolean for whether to filter the result set to only enabled
          applications
      - in: query
        name: skip
        description: The number of entries to skip in the result set
      - in: query
        name: sortBy
        description: The field to sort
      - in: query
        name: top
        description: The maximum number of entries to return in the result set
      responses:
        200:
          description: OK
      tags:
      - Applications
    post:
      summary: Post Applications
      description: |-
        Creates a new blockchain application. This method can only be performed by users who are
                     Workbench administrators.
      operationId: ApplicationsPost
      x-api-path-slug: apiv1applications-post
      parameters:
      - in: formData
        name: appFile
        description: Upload Application File
      responses:
        200:
          description: OK
      tags:
      - Applications
  /api/v1/applications/{applicationId}:
    get:
      summary: Get Applications
      description: |-
        Gets the blockchain application matching a specific application ID. Users who are Workbench administrators get
                     the blockchain application. Non-Workbench administrators get the blockchain application if they have at least one associated
                     application role or is associated with a smart contract instance role.
      operationId: ApplicationGet
      x-api-path-slug: apiv1applicationsapplicationid-get
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      responses:
        200:
          description: OK
      tags:
      - Applications
    delete:
      summary: Delete Applications
      description: |-
        Deletes the specified blockchain application. This method can only be performed by users who are
                     Workbench administrators. NOTE: Currently not implemented.
      operationId: ApplicationDelete
      x-api-path-slug: apiv1applicationsapplicationid-delete
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      responses:
        200:
          description: OK
      tags:
      - Applications
  /api/v1/applications/{applicationId}/enable:
    patch:
      summary: Patch Applications Enable
      description: |-
        Enables the specified blockchain application. This method can only be performed by users who are
                     Workbench administrators.
      operationId: ApplicationEnable
      x-api-path-slug: apiv1applicationsapplicationidenable-patch
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Enable
  /api/v1/applications/{applicationId}/disable:
    patch:
      summary: Patch Applications Disable
      description: |-
        Disables the specified blockchain application. This method can only be performed by users who are
                     Workbench administrators.
      operationId: ApplicationDisable
      x-api-path-slug: apiv1applicationsapplicationiddisable-patch
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Disable
  /api/v1/applications/{applicationId}/roleAssignments:
    get:
      summary: Get Applications Roleassignments
      description: |-
        List all role assignments of the specified blockchain application. Users who are Workbench administrators
                     get all role assignments. Non-Workbench administrators get all their role assignments. Roles are specified
                     in the Workbench application configuration and can be retrieved from GET /applications/{applicationID}.
                     Also, user information can be retrieved from GET /users/{userID}.
      operationId: RoleAssignmentsGet
      x-api-path-slug: apiv1applicationsapplicationidroleassignments-get
      parameters:
      - in: path
        name: applicationId
        description: The id of the configuration
      - in: query
        name: applicationRoleId
        description: The id of the application role
      - in: query
        name: skip
        description: The number of entries to skip in the result set
      - in: query
        name: sortBy
        description: The field to sort
      - in: query
        name: top
        description: The maximum number of entries to return in the result set
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Roleassignments
    post:
      summary: Post Applications Roleassignments
      description: |-
        Creates a user-to-role mapping in the specified blockchain application. This method can only be performed by
                     users who are Workbench administrators.
      operationId: RoleAssignmentsPost
      x-api-path-slug: apiv1applicationsapplicationidroleassignments-post
      parameters:
      - in: path
        name: applicationId
        description: The id of the configuration
      - in: body
        name: roleAssignment
        description: New user-to-role mapping
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Roleassignments
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