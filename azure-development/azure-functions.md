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

## Sample project

## Useful links and resources

Microsoft Azure Functions implementation: [https://learn.microsoft.com/en-us/training/paths/implement-azure-functions/]
