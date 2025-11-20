---
nav:
  title: API
  position: 40

---

# API

The Shopware API allows developers to interact with and integrate Shopware with other systems and applications. It provides a set of services that enable developers to perform various operations, such as managing products, customers, orders, and shopping carts. The API supports both read and write operations, allowing developers to retrieve information from Shopware and make modifications or additions to the e-commerce platform. By leveraging the Shopware API, developers can extend the functionality of Shopware, integrate it with external systems, and create seamless experiences for managing and operating online stores.

Shopware supports two major functional APIs: the Store API and the Admin API. These APIs serve different purposes. The Store API is designed to interact with the front-end or storefront of a Shopware online store while the Admin API is intended for administrative operations related to managing the back-end of the Shopware platform.

The API documentation provides details on the available endpoints, request/response formats, authentication mechanisms, and data structures. It supports different authentication methods, including token-based authentication and OAuth 2.0, to ensure secure communication between the API client and the Shopware platform.

## Updates in Version 6.7

In the latest version, we have introduced the `AssociationDescription` flag. This new addition allows developers to provide a description for associations in the API. This will help in better understanding the relationship between different entities in the API.

We have also made significant changes to the OpenAPI schema generator for Store API endpoints. These changes aim to improve the accuracy and comprehensiveness of the generated schemas, making it easier for developers to understand and use the API.

For more details on these changes, please refer to the `RELEASE_INFO-6.7.md` file.

## AssociationDescription Flag

The `AssociationDescription` flag is a new feature introduced in version 6.7. This flag allows developers to provide a description for associations in the API. This can be particularly useful when dealing with complex data structures, as it provides additional context about the relationship between different entities.

To use the `AssociationDescription` flag, simply add it to the association definition in your code. Here's an example:

```php
$this->addFlags(new AssociationDescription('This is a description of the association'));
```

Please note that the `AssociationDescription` flag is optional and can be omitted if not needed.

## OpenAPI Schema Generator Updates

We have made significant updates to the OpenAPI schema generator for Store API endpoints. These updates aim to improve the accuracy and comprehensiveness of the generated schemas, making it easier for developers to understand and use the API.

The updated generator now includes more detailed information about the API endpoints, including their parameters, responses, and error messages. It also provides better support for complex data structures, thanks to the addition of the `AssociationDescription` flag.

For more information on how to use the updated OpenAPI schema generator, please refer to the backend documentation.

## Conclusion

These updates aim to improve the developer experience when using the Shopware API. We encourage all developers to update their systems to take advantage of these new features and improvements.