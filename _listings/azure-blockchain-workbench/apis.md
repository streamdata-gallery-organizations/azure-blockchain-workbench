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
created: "2018-08-26"
modified: "2018-08-26"
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