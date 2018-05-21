{
  "info": {
    "name": "Azure Virtual Network API Public IPAddresses Delete",
    "_postman_id": "47cfeda3-f445-4685-8721-af2febc37763",
    "description": "Deletes the specified public IP address.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Public IP Address",
      "item": [
        {
          "id": "ca657d8c-feff-4a59-8d63-7ddf9711a3bf",
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
              "id": "e7adbcc6-27aa-4c3f-a364-ac928fb4307e"
            }
          ]
        }
      ]
    }
  ]
}