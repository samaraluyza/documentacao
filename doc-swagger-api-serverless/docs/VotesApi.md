# ApiServerlessDeEnquetes.VotesApi

All URIs are relative to *https://rp6w0qdem1.execute-api.us-east-1.amazonaws.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addVotes**](VotesApi.md#addVotes) | **POST** /votes | Adiciona voto em uma enquete

<a name="addVotes"></a>
# **addVotes**
> PoolItem addVotes()

Adiciona voto em uma enquete

Adiciona voto em uma enquete

### Example
```javascript
import {ApiServerlessDeEnquetes} from 'api_serverless_de_enquetes';

let apiInstance = new ApiServerlessDeEnquetes.VotesApi();
apiInstance.addVotes((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PoolItem**](PoolItem.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

