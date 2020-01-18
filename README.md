# win-blueprints

See this [repository](https://github.com/Azure/azure-blueprints) for details on how to manage Azure Blueprints as code.

#### Azure Pipeline

In order to get the Azure Pipeline working you need to:

- Install [this plugin](https://marketplace.visualstudio.com/items?itemName=nepeters.azure-blueprints&ssr=false) in the DevOps environment in order for the pipeline to know about the 'CreateBlueprint' and 'AssignBlueprint' tasks.
- Add 'spnName' and 'subscriptionId' to Pipelines Library Variable Groups as group named 'subscription-info'. Make sure that 'spnName' is equal to the 'Connection name' found on the "Service connections" page (https://dev.azure.com/{organization}/{project}/_settings/adminservices). The 'subscriptionId' should equal to the id of the subscription referenced by the same connection.
