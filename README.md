
# Getting Started with APIMATIC Calculator

## Introduction

Simple calculator API hosted on APIMATIC

## Install the Package

Install the SDK by adding the following dependency in your project's pom.xml file:

```xml
<dependency>
  <groupId>io.sdks</groupId>
  <artifactId>calcu-java-sdk</artifactId>
  <version>1.2.69</version>
</dependency>
```

You can also view the package at:
https://central.sonatype.com/artifact/io.sdks/calcu-java-sdk/1.2.69

## Test the SDK

The generated code and the server can be tested using automatically generated test cases.
JUnit is used as the testing framework and test runner.

In Eclipse, for running the tests do the following:

1. Select the project APIMATICCalculatorLib from the package explorer.
2. Select `Run -> Run as -> JUnit Test` or use `Alt + Shift + X` followed by `T` to run the Tests.

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/calcu-java-java-sdk/tree/1.2.69/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| `environment` | `Environment` | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| `httpClientConfig` | [`Consumer<HttpClientConfiguration.Builder>`](https://www.github.com/Syed-Subtain/calcu-java-java-sdk/tree/1.2.69/doc/http-client-configuration-builder.md) | Set up Http Client Configuration instance. |

The API client can be initialized as follows:

```java
APIMATICCalculatorClient client = new APIMATICCalculatorClient.Builder()
    .httpClientConfig(configBuilder -> configBuilder
            .timeout(0))
    .environment(Environment.PRODUCTION)
    .build();
```

## List of APIs

* [Simple Calculator](https://www.github.com/Syed-Subtain/calcu-java-java-sdk/tree/1.2.69/doc/controllers/simple-calculator.md)

## Classes Documentation

* [Utility Classes](https://www.github.com/Syed-Subtain/calcu-java-java-sdk/tree/1.2.69/doc/utility-classes.md)
* [HttpRequest](https://www.github.com/Syed-Subtain/calcu-java-java-sdk/tree/1.2.69/doc/http-request.md)
* [HttpResponse](https://www.github.com/Syed-Subtain/calcu-java-java-sdk/tree/1.2.69/doc/http-response.md)
* [HttpStringResponse](https://www.github.com/Syed-Subtain/calcu-java-java-sdk/tree/1.2.69/doc/http-string-response.md)
* [HttpContext](https://www.github.com/Syed-Subtain/calcu-java-java-sdk/tree/1.2.69/doc/http-context.md)
* [HttpBodyRequest](https://www.github.com/Syed-Subtain/calcu-java-java-sdk/tree/1.2.69/doc/http-body-request.md)
* [HttpCallback Interface](https://www.github.com/Syed-Subtain/calcu-java-java-sdk/tree/1.2.69/doc/http-callback-interface.md)
* [Headers](https://www.github.com/Syed-Subtain/calcu-java-java-sdk/tree/1.2.69/doc/headers.md)
* [ApiException](https://www.github.com/Syed-Subtain/calcu-java-java-sdk/tree/1.2.69/doc/api-exception.md)
* [Configuration Interface](https://www.github.com/Syed-Subtain/calcu-java-java-sdk/tree/1.2.69/doc/configuration-interface.md)
* [HttpClientConfiguration](https://www.github.com/Syed-Subtain/calcu-java-java-sdk/tree/1.2.69/doc/http-client-configuration.md)
* [HttpClientConfiguration.Builder](https://www.github.com/Syed-Subtain/calcu-java-java-sdk/tree/1.2.69/doc/http-client-configuration-builder.md)

