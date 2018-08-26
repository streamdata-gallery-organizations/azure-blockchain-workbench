{
  "info": {
    "name": "Azure Blockchain Workbench Get Applications Roleassignments",
    "_postman_id": "07815107-e216-4119-aeac-26ce53918507",
    "description": "List all role assignments of the specified blockchain application. Users who are Workbench administrators\n             get all role assignments. Non-Workbench administrators get all their role assignments. Roles are specified\n             in the Workbench application configuration and can be retrieved from GET /applications/{applicationID}.\n             Also, user information can be retrieved from GET /users/{userID}.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Applications",
      "item": [
        {
          "id": "374ec33f-4094-416e-8d5a-b2d74e4c7a44",
          "name": "ApplicationsGet",
          "request": {
            "url": "{{default}}/api/v1/applications?enabled=%7B%7D&skip=%7B%7D&sortBy=%7B%7D&top=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists all blockchain applications to which a user has access in Workbench. Users who are Workbench administrators get\n             all blockchain applications. Non-Workbench administrators get all blockchain applications for which they have at least one\n             associated application role or an associated smart contract instance role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3aa4d1be-775b-458a-9e82-60e32e641660"
            }
          ]
        },
        {
          "id": "2c2cce8c-0c27-46a0-ae82-4ed1095b97d8",
          "name": "ApplicationsPost",
          "request": {
            "url": "{{default}}/api/v1/applications",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "appFile",
                  "value": "{}",
                  "disabled": false,
                  "description": "Upload Application File"
                }
              ]
            },
            "description": "Creates a new blockchain application. This method can only be performed by users who are\n             Workbench administrators."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c15ad3d9-7039-4e2d-8359-25d99f0d4788"
            }
          ]
        },
        {
          "id": "a484b8b4-c8d0-46e8-9d77-16fd80a6aba3",
          "name": "ApplicationGet",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "api/v1/applications/:applicationId"
              ],
              "variable": [
                {
                  "id": "applicationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the blockchain application matching a specific application ID. Users who are Workbench administrators get\n             the blockchain application. Non-Workbench administrators get the blockchain application if they have at least one associated\n             application role or is associated with a smart contract instance role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e52c8607-392a-43a3-8e2a-caec70690df4"
            }
          ]
        },
        {
          "id": "32577538-f7cd-41d9-b5c5-e72aae098d81",
          "name": "ApplicationDelete",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "api/v1/applications/:applicationId"
              ],
              "variable": [
                {
                  "id": "applicationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified blockchain application. This method can only be performed by users who are\n             Workbench administrators. NOTE: Currently not implemented."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0c480fb-5420-46ec-9a00-6f05cbe3d01b"
            }
          ]
        },
        {
          "id": "f8a6919a-a303-4cf0-b63e-e075786abb6d",
          "name": "ApplicationEnable",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "api/v1/applications/:applicationId/enable"
              ],
              "variable": [
                {
                  "id": "applicationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Enables the specified blockchain application. This method can only be performed by users who are\n             Workbench administrators."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34e3068d-fade-4931-9a96-83fd01c4d985"
            }
          ]
        },
        {
          "id": "dcc8551f-10d2-40ee-adaa-cc571ca990e9",
          "name": "ApplicationDisable",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "api/v1/applications/:applicationId/disable"
              ],
              "variable": [
                {
                  "id": "applicationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Disables the specified blockchain application. This method can only be performed by users who are\n             Workbench administrators."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0cfd7c5c-2abd-4f8e-8f5d-7cf2b4fd5180"
            }
          ]
        },
        {
          "id": "3b21675c-f603-40f6-8fbb-40511e0a5002",
          "name": "RoleAssignmentsGet",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "api/v1/applications/:applicationId/roleAssignments"
              ],
              "query": [
                {
                  "key": "applicationRoleId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "skip",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sortBy",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "top",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "applicationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List all role assignments of the specified blockchain application. Users who are Workbench administrators\n             get all role assignments. Non-Workbench administrators get all their role assignments. Roles are specified\n             in the Workbench application configuration and can be retrieved from GET /applications/{applicationID}.\n             Also, user information can be retrieved from GET /users/{userID}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69e6d324-5725-447b-902d-ec83ff689c56"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/"
    }
  ]
}