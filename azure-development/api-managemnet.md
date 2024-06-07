## Concepts

API Managemnet is a managed Azure cloud service that can be used to publish, secure,maintain and monitor APIs.

You can apply policies at the APi Management level.

As per Microsoft best practices, it is preferred to use an API gateway that sits in between a cleint app and your microservices network. The API Gateway pattern is also referred to as Backend For Frontend (BFF). Please refer to this [link](https://learn.microsoft.com/en-us/dotnet/architecture/microservices/architect-microservice-container-applications/direct-client-to-microservice-communication-versus-the-api-gateway-pattern) for more information.

## Use-cases

- exposing Azure Functions as API endpoints using API Management
- exposing microservices through API Management to avoid client to microservice direct interaction
