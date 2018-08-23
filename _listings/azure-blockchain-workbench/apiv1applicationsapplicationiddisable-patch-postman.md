{
  "info": {
    "name": "Azure Blockchain Workbench Patch Applications Disable",
    "_postman_id": "5a57bf7b-5e50-47f6-9d9b-e5e74dbefa89",
    "description": "Disables the specified blockchain application. This method can only be performed by users who are\n             Workbench administrators.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Applications",
      "item": [
        {
          "id": "6a9b35b0-60b7-4b0e-8f41-ee4f729785e4",
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
              "id": "90018149-8362-4425-a1b2-408e0f7fab88"
            }
          ]
        },
        {
          "id": "7e56f645-adc8-427e-9d63-51a4a7aca1be",
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
              "id": "cc552ca1-c4da-4393-a237-05488fe155b9"
            }
          ]
        },
        {
          "id": "a651ad59-4d86-4b3d-84d0-64a7a94ab68d",
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
              "id": "580c62b3-526f-4bfd-86cc-05baa34985ff"
            }
          ]
        },
        {
          "id": "25075d5f-38b2-423b-a626-98e46cc8d90b",
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
              "id": "ecaed7ef-9a6e-403d-b478-f271721d3cc4"
            }
          ]
        },
        {
          "id": "e94473b5-e8ae-4e84-95a3-fccf2b465742",
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
              "id": "ffa867ea-127f-4d24-8161-5477d0c55fb5"
            }
          ]
        },
        {
          "id": "0f9ec7e3-320e-4f0b-ac63-7b764e466390",
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
              "id": "d205e2e0-c589-48ac-a369-726e3d6ee030"
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