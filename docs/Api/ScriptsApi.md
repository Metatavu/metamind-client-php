# Metatavu\Metamind\ScriptsApi

All URIs are relative to *https://localhost/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createScript**](ScriptsApi.md#createScript) | **POST** /scripts | Posts new script


# **createScript**
> \Metatavu\Metamind\Api\Model\Script createScript($body)

Posts new script

Posts new script

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure HTTP basic authorization: basicAuth
$config = Metatavu\Metamind\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new Metatavu\Metamind\Api\ScriptsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Metatavu\Metamind\Api\Model\Script(); // \Metatavu\Metamind\Api\Model\Script | Payload

try {
    $result = $apiInstance->createScript($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScriptsApi->createScript: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Metatavu\Metamind\Api\Model\Script**](../Model/Script.md)| Payload |

### Return type

[**\Metatavu\Metamind\Api\Model\Script**](../Model/Script.md)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json;charset=utf-8
 - **Accept**: application/json;charset=utf-8

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

