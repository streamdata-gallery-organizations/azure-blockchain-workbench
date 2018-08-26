{
  "info": {
    "name": "Azure Blockchain Workbench Post Applications",
    "_postman_id": "d1659b30-f24a-4083-be6e-5206884d4b8e",
    "description": "Creates a new blockchain application. This method can only be performed by users who are\n             Workbench administrators.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Applications",
      "item": [
        {
          "id": "30824b49-1c05-4101-be0c-4f99eba9a027",
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
              "id": "840feb56-a233-47ff-923b-e69efa5967da"
            }
          ]
        },
        {
          "id": "0db8830e-0aec-4430-97f1-7094e3bbadb3",
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
              "id": "3a2f25a9-0a7d-4413-8581-c85c54d6263f"
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