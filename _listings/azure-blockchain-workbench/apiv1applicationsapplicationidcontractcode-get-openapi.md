---
swagger: "2.0"
x-collection-name: Azure Blockchain Workbench
x-complete: 0
info:
  title: Azure Blockchain Workbench Get Applications Contract Code
  description: |-
    List all blockchain smart contract implementations of the specified blockchain application.
                 Users who are Workbench administrators get all smart contract implementations. Non-Workbench administrators get all
                 smart contract implementations for which they have at least one associated application role or is associated with a
                 smart contract instance role.
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
  /api/v1/applications/{applicationId}/roleAssignments/{roleAssignmentId}:
    get:
      summary: Get Applications Roleassignments Roleassignmentid
      description: |-
        Get a role assignment of the specified blockchain application matching a specific user role assignment ID.
                     Users who are Workbench administrators get the role assignment. Non-Workbench administrators get the role assignment
                     if they are associated in the application.
      operationId: RoleAssignmentGet
      x-api-path-slug: apiv1applicationsapplicationidroleassignmentsroleassignmentid-get
      parameters:
      - in: path
        name: applicationId
        description: The id of the configuration
      - in: path
        name: roleAssignmentId
        description: The id of the role assignment
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Roleassignments
      - Roleassignmentid
    put:
      summary: Put Applications Roleassignments Roleassignmentid
      description: Updates the specified role assignment. This method can only be
        performed by users who are Workbench administrators.
      operationId: RoleAssignmentPut
      x-api-path-slug: apiv1applicationsapplicationidroleassignmentsroleassignmentid-put
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      - in: body
        name: roleAssignment
        description: New user-to-role mapping parameters
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: roleAssignmentId
        description: The id of the user-to-role mapping
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Roleassignments
      - Roleassignmentid
    delete:
      summary: Delete Applications Roleassignments Roleassignmentid
      description: |-
        Deletes the specified role assignment. This method can only be performed by users who are
                     Workbench administrators.
      operationId: RoleAssignmentDelete
      x-api-path-slug: apiv1applicationsapplicationidroleassignmentsroleassignmentid-delete
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      - in: path
        name: roleAssignmentId
        description: The id of the role assignment
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Roleassignments
      - Roleassignmentid
  /api/v1/applications/{applicationId}/workflows:
    get:
      summary: Get Applications Workflows
      description: |-
        List all workflows of the specified blockchain application. Users who are Workbench administrators get all
                     workflows. Non-Workbench administrators get all workflows for which they have at least one associated application role
                     or are associated with a smart contract instance role.
      operationId: WorkflowsGet
      x-api-path-slug: apiv1applicationsapplicationidworkflows-get
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      - in: query
        name: skip
        description: The number of items to skip before returning
      - in: query
        name: top
        description: The maximum number of items to return
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Workflows
  /api/v1/applications/workflows/{workflowId}:
    get:
      summary: Get Applications Workflows
      description: |-
        Get a workflow matching a specific workflow ID.
                     Users who are Workbench administrators get the workflow. Non-Workbench administrators get the workflow if they
                     have at least one associated application role or is associated with a smart contract instance role.
      operationId: WorkflowGet
      x-api-path-slug: apiv1applicationsworkflowsworkflowid-get
      parameters:
      - in: path
        name: workflowId
        description: The id of the workflow
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Workflows
  /api/v1/applications/{applicationId}/contractCode:
    get:
      summary: Get Applications Contract Code
      description: |-
        List all blockchain smart contract implementations of the specified blockchain application.
                     Users who are Workbench administrators get all smart contract implementations. Non-Workbench administrators get all
                     smart contract implementations for which they have at least one associated application role or is associated with a
                     smart contract instance role.
      operationId: ContractCodesGet
      x-api-path-slug: apiv1applicationsapplicationidcontractcode-get
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      - in: query
        name: ledgerId
        description: The index of the chain type
      - in: query
        name: skip
        description: The number of items to skip before returning
      - in: query
        name: top
        description: The maximum number of items to return
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Contract
      - Code
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