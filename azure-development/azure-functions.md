## Concepts

Azure Functions are a serverless offering from Microsoft that allows developers to focus on writting code to run in the cloud without having to worry about provisioning infrastructure or managing servers.

Azure functions are triggered by events and they typically address orchestration logic and workflows.

They leverage the consumption-based model very well and you are only being charged wwhen the function runs.

The serveless compute is also referred to as Function As a Service (FaaS).

Terminology:

- trigger: an event that starts the function (e.g.: receiving and Http request, a message being added to a queue)
- binding: a declarative way to connect data and services to your function; the code reads data from **input bindings ** and writes data to ** output bindings **

Limitations to be aware of when using functions:

- they have a timeout of 5 mins which can be extended to 10 mins; ** Durable Functions **, however, let you execute multiple functions orchestration without any timeout
- execution frequency: only one function app instance can be created every 10 seconds, for up to 200 total instances

## Typical uses cases

- executing a workflow on a trigger; the workflow is best suited for a "code-first" approach rather than "design-first" (e.g. using a tool like Azure Logic Apps)

## Sample projects and how-tos

There are multiple ways to create Azure functions:

1. Create the function directly in the Azure portal; this will work only for supported languages like JavaScript, PowerShell, Python, and C# Script (.csx)
2. Create the function in your favorite IDE (e.g. Visual Studio Code) and publish it to Azure
3. Create the function using the Azure Core tools. Here is a Microsoft walkthrough on how to do this: [https://learn.microsoft.com/en-us/training/modules/develop-test-deploy-azure-functions-with-core-tools/]

### Process of linking an Azure function with a GitHub repository

Azure functions can be setup to receive payloads from a GitHub webhook. The webhook gets triggered by specific events in the configured GitHub repository.

### Process of publishing an Azure function from the CLI with Azure Functions Core tools

### Process of creating and publishing a function from Visual Studio

### Procees of creating and publishing a function from VS Code

## Useful links and resources

Microsoft Azure Functions implementation: [https://learn.microsoft.com/en-us/training/paths/implement-azure-functions/]

Azure functions in Azure CLI : [https://learn.microsoft.com/en-us/azure/azure-functions/create-first-function-cli-csharp?tabs=macos%2Cazure-cli]
