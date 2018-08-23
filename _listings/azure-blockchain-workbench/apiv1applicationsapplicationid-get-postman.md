{
  "info": {
    "name": "Azure Blockchain Workbench Get Applications",
    "_postman_id": "851c27ce-ee82-4c6b-ac22-8981c637e99f",
    "description": "Gets the blockchain application matching a specific application ID. Users who are Workbench administrators get\n             the blockchain application. Non-Workbench administrators get the blockchain application if they have at least one associated\n             application role or is associated with a smart contract instance role.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Applications",
      "item": [
        {
          "id": "7baf8a3d-c2c5-4772-9b94-bca099e9c86e",
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
              "id": "b9053ad0-80ce-456a-ab9f-644e583331c0"
            }
          ]
        },
        {
          "id": "0340056c-711e-4ad1-a964-cbb1aa357990",
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
              "id": "206b75f4-637c-4ab5-b05a-7eac89f1c3b1"
            }
          ]
        },
        {
          "id": "e102b19b-7d07-47a6-9426-4ccd3f5620ce",
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
              "id": "1a17c4b6-864d-431e-bb15-317c1990aa04"
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