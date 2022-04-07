# Swagger\Client\ApplicationAccessApi

All URIs are relative to *https://api.avito.ru/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getAccessTokenAuthorizationCode**](ApplicationAccessApi.md#getaccesstokenauthorizationcode) | **POST** /token‎ | Получение access token
[**refreshAccessTokenAuthorizationCode**](ApplicationAccessApi.md#refreshaccesstokenauthorizationcode) | **POST** /token‎‎ | Обновление access token

# **getAccessTokenAuthorizationCode**
> \Swagger\Client\Model\InlineResponse2001 getAccessTokenAuthorizationCode($client_id, $client_secret, $code, $grant_type)

Получение access token

Получения временного ключа для авторизации запроса от лица пользователя

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ApplicationAccessApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$client_id = "client_id_example"; // string | 
$client_secret = "client_secret_example"; // string | 
$code = "code_example"; // string | 
$grant_type = "grant_type_example"; // string | 

try {
    $result = $apiInstance->getAccessTokenAuthorizationCode($client_id, $client_secret, $code, $grant_type);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ApplicationAccessApi->getAccessTokenAuthorizationCode: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **client_id** | **string**|  | [optional]
 **client_secret** | **string**|  | [optional]
 **code** | **string**|  | [optional]
 **grant_type** | **string**|  | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse2001**](../Model/InlineResponse2001.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **refreshAccessTokenAuthorizationCode**
> \Swagger\Client\Model\InlineResponse2002 refreshAccessTokenAuthorizationCode($client_id, $client_secret, $grant_type, $refresh_token)

Обновление access token

Обновление временного ключа для авторизации запроса от лица пользователя

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ApplicationAccessApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$client_id = "client_id_example"; // string | 
$client_secret = "client_secret_example"; // string | 
$grant_type = "grant_type_example"; // string | 
$refresh_token = "refresh_token_example"; // string | 

try {
    $result = $apiInstance->refreshAccessTokenAuthorizationCode($client_id, $client_secret, $grant_type, $refresh_token);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ApplicationAccessApi->refreshAccessTokenAuthorizationCode: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **client_id** | **string**|  | [optional]
 **client_secret** | **string**|  | [optional]
 **grant_type** | **string**|  | [optional]
 **refresh_token** | **string**|  | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse2002**](../Model/InlineResponse2002.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

