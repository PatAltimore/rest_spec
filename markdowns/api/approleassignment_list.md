# List AppRoleAssignment

Retrieve a list of approleassignment objects.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /users/<objectId>/appRoleAssignments
GET /drive/root/createdByUser/appRoleAssignments
GET /drive/root/lastModifiedByUser/appRoleAssignments
```
### Optional query parameters
|Name|Value|Description|
|:---------------|:--------|:-------|
|$orderby|string|Comma-separated list of properties that are used to sort the order of items in the response collection.|

### Request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| X-Sample-Header  | string  | Sample HTTP header. Update accordingly or remove if not needed|

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns a `200 OK` response code and collection of [AppRoleAssignment](../resources/approleassignment.md) objects in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_approleassignments"
}-->
```http
GET /users/<objectId>
```
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.approleassignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 467

{
  "value": [
    {
      "creationTimestamp": "datetime-value",
      "id": "id-value",
      "principalDisplayName": "principalDisplayName-value",
      "principalId": "principalId-value",
      "principalType": "principalType-value",
      "resourceDisplayName": "resourceDisplayName-value",
      "resourceId": "resourceId-value",
      "objectType": "objectType-value",
      "objectId": "objectId-value",
      "deletionTimestamp": "datetime-value"
    }
  ]
}
```

<!-- uuid: 1ec6c637-d5ce-4c7c-8510-60a02b97903c
2015-10-25 13:14:09 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List AppRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->