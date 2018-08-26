{
  "info": {
    "name": "Azure Blockchain Workbench Get Applications",
    "_postman_id": "28988e4d-1c19-4d3f-b7cf-a7d2447984d9",
    "description": "Lists all blockchain applications to which a user has access in Workbench. Users who are Workbench administrators get\n             all blockchain applications. Non-Workbench administrators get all blockchain applications for which they have at least one\n             associated application role or an associated smart contract instance role.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Applications",
      "item": [
        {
          "id": "8cc2d083-026b-4611-a8fd-ab7257a20fa8",
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
              "id": "f2f4230b-5d3f-47d8-a969-f9014467d68a"
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