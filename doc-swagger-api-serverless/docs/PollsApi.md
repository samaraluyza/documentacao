# ApiServerlessDeEnquetes.PollsApi

All URIs are relative to *https://rp6w0qdem1.execute-api.us-east-1.amazonaws.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addPoll**](PollsApi.md#addPoll) | **POST** /polls | Adiciona uma enquete
[**searchPollID**](PollsApi.md#searchPollID) | **GET** /polls/{pollId} | Lista uma enquete específica
[**searchPolls**](PollsApi.md#searchPolls) | **GET** /polls | Lista todas as enquetes

<a name="addPoll"></a>
# **addPoll**
> PoolItem addPoll()

Adiciona uma enquete

Adiciona uma enquete ao banco de dados

### Example
```javascript
import {ApiServerlessDeEnquetes} from 'api_serverless_de_enquetes';

let apiInstance = new ApiServerlessDeEnquetes.PollsApi();
apiInstance.addPoll((error, data, response) => {
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

<a name="searchPollID"></a>
# **searchPollID**
> PoolItem searchPollID(pollId)

Lista uma enquete específica

Lista um enquete específica passando o parâmetro Poll ID 

### Example
```javascript
import {ApiServerlessDeEnquetes} from 'api_serverless_de_enquetes';

let apiInstance = new ApiServerlessDeEnquetes.PollsApi();
let pollId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | Poll ID

apiInstance.searchPollID(pollId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pollId** | [**String**](.md)| Poll ID | 

### Return type

[**PoolItem**](PoolItem.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="searchPolls"></a>
# **searchPolls**
> [PoolItem] searchPolls()

Lista todas as enquetes

Lista todas as enquetes disponiveis na base de dados 

### Example
```javascript
import {ApiServerlessDeEnquetes} from 'api_serverless_de_enquetes';

let apiInstance = new ApiServerlessDeEnquetes.PollsApi();
apiInstance.searchPolls((error, data, response) => {
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

[**[PoolItem]**](PoolItem.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

