{
  "info": {
    "name": "Compute Engine",
    "_postman_id": "9f93b8ba-452b-42e9-a769-c4f2f56ba846",
    "description": "Creates and runs virtual machines on Google Cloud Platform.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "subnetwork",
      "item": [
        {
          "id": "bbfe980e-9b4e-4df8-a9be-36720f5a57ff",
          "name": "compute.subnetworks.aggregatedList",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "compute",
                "v1",
                "projects",
                ":project/aggregated/subnetworks"
              ],
              "query": [
                {
                  "key": "filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "orderBy",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "project",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves an aggregated list of subnetworks"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1d38292-3482-4cf6-8fd7-73a753a8a6e0"
            }
          ]
        }
      ]
    }
  ]
}