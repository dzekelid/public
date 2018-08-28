{
  "info": {
    "name": "Azure Virtual Network API Public IPAddresses Get",
    "_postman_id": "b62faec7-1fdc-41c6-91b2-1532fd7a9808",
    "description": "Gets the specified public IP address in a specified resource group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Public IP Address",
      "item": [
        {
          "id": "7a833b75-b4ac-4446-a1c6-e961ef95b862",
          "name": "PublicIPAddresses_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Network/publicIPAddresses/:publicIpAddressName"
              ],
              "query": [
                {
                  "key": "$expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "publicIpAddressName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the specified public IP address in a specified resource group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae0caf47-d417-44bf-a4e8-6f1d47eae821"
            }
          ]
        },
        {
          "id": "a098e621-ef68-47c1-ae41-7067678a6d4a",
          "name": "PublicIPAddresses_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Network/publicIPAddresses/:publicIpAddressName"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "publicIpAddressName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified public IP address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a523863-a83b-4669-b80c-27d150aec530"
            }
          ]
        }
      ]
    }
  ]
}