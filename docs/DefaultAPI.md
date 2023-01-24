# DefaultAPI

All URIs are relative to *https://api.chatonmac.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**queryBalance**](DefaultAPI.md#querybalance) | **GET** /balance | 
[**queryChat**](DefaultAPI.md#querychat) | **GET** /chat | 


# **queryBalance**
```swift
    open class func queryBalance(receipt: String, completion: @escaping (_ data: QueryBalance200Response?, _ error: Error?) -> Void)
```



### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import ChatOnMacWeb

let receipt = "receipt_example" // String | 

DefaultAPI.queryBalance(receipt: receipt) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt** | **String** |  | 

### Return type

[**QueryBalance200Response**](QueryBalance200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **queryChat**
```swift
    open class func queryChat(prompt: String, receipt: String, completion: @escaping (_ data: QueryChat200Response?, _ error: Error?) -> Void)
```



### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import ChatOnMacWeb

let prompt = "prompt_example" // String | 
let receipt = "receipt_example" // String | 

DefaultAPI.queryChat(prompt: prompt, receipt: receipt) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **prompt** | **String** |  | 
 **receipt** | **String** |  | 

### Return type

[**QueryChat200Response**](QueryChat200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

