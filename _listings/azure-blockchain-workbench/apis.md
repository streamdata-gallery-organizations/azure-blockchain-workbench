---
name: Azure Blockchain Workbench
x-slug: azure-blockchain-workbench
description: Azure Blockchain Workbench helps organizations build rich, integrated
  multi-party blockchain applications quickly and easily. Azure Blockchain Workbench
  REST API provides developers and information workers a way to integrate to blockchain
  applications. For example, a developer can use the REST API to enable IoT devices
  to send data to a blockchain application. Or, an information worker can use the
  REST API and Power BI to create visualization of blockchain data.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
x-kinRank: "7"
x-alexaRank: ""
tags: Azure Blockchain Workbench
created: "2018-08-29"
modified: "2018-08-29"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Blockchain Workbench REST API - Get Applications
  x-api-slug: apiv1applications-get
  description: |-
    Lists all blockchain applications to which a user has access in Workbench. Users who are Workbench administrators get
                 all blockchain applications. Non-Workbench administrators get all blockchain applications for which they have at least one
                 associated application role or an associated smart contract instance role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applications-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applications-get-openapi.md
- name: Azure Blockchain Workbench REST API - Post Applications
  x-api-slug: apiv1applications-post
  description: |-
    Creates a new blockchain application. This method can only be performed by users who are
                 Workbench administrators.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applications-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applications-post-openapi.md
- name: Azure Blockchain Workbench REST API - Get Applications
  x-api-slug: apiv1applicationsapplicationid-get
  description: |-
    Gets the blockchain application matching a specific application ID. Users who are Workbench administrators get
                 the blockchain application. Non-Workbench administrators get the blockchain application if they have at least one associated
                 application role or is associated with a smart contract instance role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationsapplicationid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationsapplicationid-get-openapi.md
- name: Azure Blockchain Workbench REST API - Delete Applications
  x-api-slug: apiv1applicationsapplicationid-delete
  description: |-
    Deletes the specified blockchain application. This method can only be performed by users who are
                 Workbench administrators. NOTE: Currently not implemented.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationsapplicationid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationsapplicationid-delete-openapi.md
- name: Azure Blockchain Workbench REST API - Patch Applications Enable
  x-api-slug: apiv1applicationsapplicationidenable-patch
  description: |-
    Enables the specified blockchain application. This method can only be performed by users who are
                 Workbench administrators.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationsapplicationidenable-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationsapplicationidenable-patch-openapi.md
- name: Azure Blockchain Workbench REST API - Patch Applications Disable
  x-api-slug: apiv1applicationsapplicationiddisable-patch
  description: |-
    Disables the specified blockchain application. This method can only be performed by users who are
                 Workbench administrators.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationsapplicationiddisable-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationsapplicationiddisable-patch-openapi.md
- name: Azure Blockchain Workbench REST API - Get Applications Roleassignments
  x-api-slug: apiv1applicationsapplicationidroleassignments-get
  description: |-
    List all role assignments of the specified blockchain application. Users who are Workbench administrators
                 get all role assignments. Non-Workbench administrators get all their role assignments. Roles are specified
                 in the Workbench application configuration and can be retrieved from GET /applications/{applicationID}.
                 Also, user information can be retrieved from GET /users/{userID}.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationsapplicationidroleassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationsapplicationidroleassignments-get-openapi.md
- name: Azure Blockchain Workbench REST API - Post Applications Roleassignments
  x-api-slug: apiv1applicationsapplicationidroleassignments-post
  description: |-
    Creates a user-to-role mapping in the specified blockchain application. This method can only be performed by
                 users who are Workbench administrators.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationsapplicationidroleassignments-post-openapi.md
- name: Azure Blockchain Workbench REST API - Get Applications Roleassignments Roleassignmentid
  x-api-slug: apiv1applicationsapplicationidroleassignmentsroleassignmentid-get
  description: |-
    Get a role assignment of the specified blockchain application matching a specific user role assignment ID.
                 Users who are Workbench administrators get the role assignment. Non-Workbench administrators get the role assignment
                 if they are associated in the application.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationsapplicationidroleassignmentsroleassignmentid-get-openapi.md
- name: Azure Blockchain Workbench REST API - Put Applications Roleassignments Roleassignmentid
  x-api-slug: apiv1applicationsapplicationidroleassignmentsroleassignmentid-put
  description: Updates the specified role assignment. This method can only be performed
    by users who are Workbench administrators.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationsapplicationidroleassignmentsroleassignmentid-put-openapi.md
- name: Azure Blockchain Workbench REST API - Delete Applications Roleassignments
    Roleassignmentid
  x-api-slug: apiv1applicationsapplicationidroleassignmentsroleassignmentid-delete
  description: |-
    Deletes the specified role assignment. This method can only be performed by users who are
                 Workbench administrators.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationsapplicationidroleassignmentsroleassignmentid-delete-openapi.md
- name: Azure Blockchain Workbench REST API - Get Applications Workflows
  x-api-slug: apiv1applicationsapplicationidworkflows-get
  description: |-
    List all workflows of the specified blockchain application. Users who are Workbench administrators get all
                 workflows. Non-Workbench administrators get all workflows for which they have at least one associated application role
                 or are associated with a smart contract instance role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationsapplicationidworkflows-get-openapi.md
- name: Azure Blockchain Workbench REST API - Get Applications Workflows
  x-api-slug: apiv1applicationsworkflowsworkflowid-get
  description: |-
    Get a workflow matching a specific workflow ID.
                 Users who are Workbench administrators get the workflow. Non-Workbench administrators get the workflow if they
                 have at least one associated application role or is associated with a smart contract instance role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationsworkflowsworkflowid-get-openapi.md
- name: Azure Blockchain Workbench REST API - Get Applications Contract Code
  x-api-slug: apiv1applicationsapplicationidcontractcode-get
  description: |-
    List all blockchain smart contract implementations of the specified blockchain application.
                 Users who are Workbench administrators get all smart contract implementations. Non-Workbench administrators get all
                 smart contract implementations for which they have at least one associated application role or is associated with a
                 smart contract instance role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationsapplicationidcontractcode-get-openapi.md
- name: Azure Blockchain Workbench REST API - Post Applications Contract Code
  x-api-slug: apiv1applicationsapplicationidcontractcode-post
  description: |-
    Uploads one or more smart contracts (ex. .sol or .zip), representing the implementation of the specified blockchain
                 application. This method can only be performed by users who are Workbench administrators.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationsapplicationidcontractcode-post-openapi.md
- name: Azure Blockchain Workbench REST API - Get Applications Contract Code
  x-api-slug: apiv1applicationscontractcodecontractcodeid-get
  description: |-
    Get the blockchain smart contract implementation matching a specific
                 contract code id. Users who are Workbench administrators get the specified smart contract implementation.
                 Non-Workbench administrators get the smart contract implementation if they have at least one associated application
                 role or is associated with a smart contract instance role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationscontractcodecontractcodeid-get-openapi.md
- name: Azure Blockchain Workbench REST API - Delete Applications Contract Code
  x-api-slug: apiv1applicationscontractcodecontractcodeid-delete
  description: |-
    Deletes the specified blockchain smart contract implementation of a specific blockchain application.
                 This method can only be performed by users who are Workbench administrators.
                 NOTE: not currently implemented
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1applicationscontractcodecontractcodeid-delete-openapi.md
- name: Azure Blockchain Workbench REST API - Get Capabilities
  x-api-slug: apiv1capabilities-get
  description: |-
    List all capabilities the user can perform within Workbench.
                 Checked capabilities include ability to add blockchain applications, add smart contract implementations,
                 add or edit user role assignments, and add new users.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1capabilities-get-openapi.md
- name: Azure Blockchain Workbench REST API - Get Capabilities Can Create Contract
  x-api-slug: apiv1capabilitiescancreatecontractworkflowid-get
  description: Checks if user has capability to create new smart contract instance
    for a specific workflow ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1capabilitiescancreatecontractworkflowid-get-openapi.md
- name: Azure Blockchain Workbench REST API - Post Checkers Check Application
  x-api-slug: apiv1checkerscheckapplication-post
  description: Checks if the supplied application configuration file is valid for
    Workbench.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1checkerscheckapplication-post-openapi.md
- name: Azure Blockchain Workbench REST API - Post Checkers Check Contract Node
  x-api-slug: apiv1checkerscheckcontractcode-post
  description: Check if the application smart contract implementation file is valid
    for Workbench.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1checkerscheckcontractcode-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1checkerscheckcontractcode-post-openapi.md
- name: Azure Blockchain Workbench REST API - Get Ledgers Connections
  x-api-slug: apiv1ledgersconnections-get
  description: Lists the connected blockchain networks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1ledgersconnections-get-openapi.md
- name: Azure Blockchain Workbench REST API - Get Ledgers Connections
  x-api-slug: apiv1ledgersconnectionsconnectionid-get
  description: Gets the connected blockchain network matching a specific connection
    ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1ledgersconnectionsconnectionid-get-openapi.md
- name: Azure Blockchain Workbench REST API - Get Ledgers Connections Blocks
  x-api-slug: apiv1ledgersconnectionsconnectionidblocks-get
  description: Lists the blocks for a connected blockchain network.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1ledgersconnectionsconnectionidblocks-get-openapi.md
- name: Azure Blockchain Workbench REST API - Get Ledgers Connections Blocks Blockid
  x-api-slug: apiv1ledgersconnectionsconnectionidblocksblockid-get
  description: Gets the block matching a specific block ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1ledgersconnectionsconnectionidblocksblockid-get-openapi.md
- name: Azure Blockchain Workbench REST API - Get Ledgers Connections Transactions
  x-api-slug: apiv1ledgersconnectionsconnectionidtransactions-get
  description: Lists the transactions for a connected blockchain network.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1ledgersconnectionsconnectionidtransactions-get-openapi.md
- name: Azure Blockchain Workbench REST API - Get Ledgers Connections Transactions
    Transactionid
  x-api-slug: apiv1ledgersconnectionsconnectionidtransactionstransactionid-get
  description: Gets the transaction matching a specific transaction ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1ledgersconnectionsconnectionidtransactionstransactionid-get-openapi.md
- name: Azure Blockchain Workbench REST API - Get Contracts
  x-api-slug: apiv1contracts-get
  description: |-
    Lists the smart contract instances of the specified workflow. Users who are Workbench administrators get all
                 smart contract instances. Non-Workbench administrators get all smart contract instances for which they have at least
                 one associated application role or is associated with a smart contract instance role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1contracts-get-openapi.md
- name: Azure Blockchain Workbench REST API - Post Contracts
  x-api-slug: apiv1contracts-post
  description: |-
    Creates a new smart contract instance for the specified workflow ID.
                 Users are only able to create a new smart contract instance if the user is associated with an application role,
                 which can initiate a smart contract instance for the workflow.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1contracts-post-openapi.md
- name: Azure Blockchain Workbench REST API - Get Contracts
  x-api-slug: apiv1contractscontractid-get
  description: |-
    Gets the smart contract instance matching a specific contract ID. Users who are Workbench
                 administrators get the smart contract instance. Non-Workbench administrators get the smart contract instance
                 if they have at least one associated application role or is associated with the smart contract instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1contractscontractid-get-openapi.md
- name: Azure Blockchain Workbench REST API - Get Contracts Actions
  x-api-slug: apiv1contractscontractidactions-get
  description: |-
    Lists all actions, which can be taken by the given user and current state of the specified smart contract
                 instance. Users get all applicable actions if the user has an associated application role or is associated with a smart
                 contract instance role for the current state of the specified smart contract instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1contractscontractidactions-get-openapi.md
- name: Azure Blockchain Workbench REST API - Post Contracts Actions
  x-api-slug: apiv1contractscontractidactions-post
  description: |-
    Executes an action for the specified smart contract instance and action ID. Users are only able to execute
                 the action given the current state of the specified smart contract instance and the user's associated application role
                 or smart contract instance role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1contractscontractidactions-post-openapi.md
- name: Azure Blockchain Workbench REST API - Get Contracts Actions
  x-api-slug: apiv1contractscontractidactionsactionid-get
  description: |-
    Gets the action matching the specified action ID. Users get the action if the user can take the action
                 given the current state of the specified smart contract instance and the user's associated application role or smart
                 contract instance role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1contractscontractidactionsactionid-get-openapi.md
- name: Azure Blockchain Workbench REST API - Get Graph Proxy Version Users
  x-api-slug: apiv1graphproxyversionusers-get
  description: |-
    Represents a proxy method to the Azure Active Directory Graph API for users.
                 See https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list for more details.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1graphproxyversionusers-get-openapi.md
- name: Azure Blockchain Workbench REST API - Get Api Health
  x-api-slug: apihealth-get
  description: |-
    Returns the health of the system. See https://docs.microsoft.com/en-us/azure/architecture/patterns/health-endpoint-monitoring
                 for more details.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apihealth-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apihealth-get-openapi.md
- name: Azure Blockchain Workbench REST API - Get Ledgers
  x-api-slug: apiv1ledgers-get
  description: Lists the supported blockchain types, such as Ethereum or Hyperledger
    Fabric.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1ledgers-get-openapi.md
- name: Azure Blockchain Workbench REST API - Get Users
  x-api-slug: apiv1users-get
  description: Lists all users within the connected blockchain consortium.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1users-get-openapi.md
- name: Azure Blockchain Workbench REST API - Post Users
  x-api-slug: apiv1users-post
  description: |-
    Adds a user to the blockchain consortium. This method can only be performed by users who are
                 Workbench administrators.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1users-post-openapi.md
- name: Azure Blockchain Workbench REST API - Get Users Userid
  x-api-slug: apiv1usersuserid-get
  description: Gets the user matching a specific user ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1usersuserid-get-openapi.md
- name: Azure Blockchain Workbench REST API - Delete Users Userid
  x-api-slug: apiv1usersuserid-delete
  description: |-
    Deletes the specified user. This method can only be performed by users who are Workbench administrators.
                 NOTE: Not currently implemented.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1usersuserid-delete-openapi.md
- name: Azure Blockchain Workbench REST API - Get Users Me
  x-api-slug: apiv1usersme-get
  description: Returns the current user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-blockchain-workbench/master/_listings/azure-blockchain-workbench/apiv1usersme-get-openapi.md
x-common:
- type: x-blog
  url: https://azure.microsoft.com/en-us/blog/topics/blockchain/
- type: x-blog-rss
  url: https://azurecomcdn.azureedge.net/en-us/blog/topics/blockchain/feed/
- type: x-openapi
  url: https://raw.githubusercontent.com/Azure-Samples/blockchain/master/blockchain-workbench/rest-api-samples/swagger/swagger.json
- type: x-website
  url: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
- type: x-api-gallery
  url: http://azure.billing.api.api.gallery.streamdata.io
- type: x-api-stack
  url: http://azure.blockchain.workbench.stack.network
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---