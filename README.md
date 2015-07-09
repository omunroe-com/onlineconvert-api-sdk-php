# Online Convert API2 php SDK

This SDK provides a code base to interact with the API2 for [Online Convert](http://www.online-convert.com/). 

Since the API2 follows the [Swagger specs](http://swagger.io/) this code has been generated using the [swagger codegenerator](https://github.com/swagger-api/swagger-codegen).

## Installation

The QaamGo Online Convert PHP SDK can be installed with [Composer](https://getcomposer.org/). Add the QaamGo Online Convert PHP SDK package to your `composer.json` file.

    {
        "require": {
            "online-convert-php-sdk": "~1.0"
        }
    }

## Usage

Simple GET status and conversions from API information.

    require '../vendor/autoload.php';
    use SwaggerClient\InformationApi;
    
    $information_api = new InformationApi();
    $conversions = $information_api->conversionsGet('archive', '', 1);
    
    $information_api = new InformationApi();
    $status = $information_api->statusesGet();
    
    print_r($conversions);
    print_r($status);
    
## Samples

Included in the SDK there are a few samples ready to work.