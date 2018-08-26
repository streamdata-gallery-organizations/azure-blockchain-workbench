{
  "info": {
    "name": "Azure Blockchain Workbench Patch Applications Enable",
    "_postman_id": "b7280170-9932-44c9-9add-d3bf27c260dc",
    "description": "Enables the specified blockchain application. This method can only be performed by users who are\n             Workbench administrators.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Applications",
      "item": [
        {
          "id": "34fd82e9-05fd-43b3-8078-ae9a7de7301e",
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
              "id": "35f3e756-5075-4237-b430-a3dc6b9b18b3"
            }
          ]
        },
        {
          "id": "dba05005-0c34-4b5b-8763-3036c538c9dc",
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
              "id": "b4e56f21-fdf4-42b2-b488-5609e676cc43"
            }
          ]
        },
        {
          "id": "3df7bb76-4c5c-43ec-855d-5f4710d52f35",
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
              "id": "8f9cdacf-8cf8-41a0-abe0-2b70ecda1166"
            }
          ]
        },
        {
          "id": "4383667f-1e81-43a8-8eca-21fab6b48cb8",
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
              "id": "442e77c2-34c9-4566-8478-9001eea6217b"
            }
          ]
        },
        {
          "id": "c9209acf-7583-4aa5-bd24-34b36fcfcc6d",
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
              "id": "282598e4-82cd-4d22-a0e0-85e39cf127c7"
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