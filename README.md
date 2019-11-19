# Java: Azure Functions Dev in a remote container

## Developing inside a container

[VS Code Docs for developing inside a container](https://code.visualstudio.com/docs/remote/containers?WT.mc_id=functions-github-shboyer)

## Reference Links

[Azure Functions Java developer guide](https://docs.microsoft.com/azure/azure-functions/functions-reference-java?WT.mc_id=functions-github-shboyer)

### Simple example tutorial 

[Azure Functions HTTP triggers and bindings](https://docs.microsoft.com/azure/azure-functions/functions-bindings-http-webhook?tabs=java&WT.mc_id=functions-github-shboyer)

### Event Hub trigger and Azure Cosmos DB tutorial 

[Create a function in Java with an Event Hub trigger and an Azure Cosmos DB output binding](https://docs.microsoft.com/azure/azure-functions/functions-event-hub-cosmos-db?WT.mc_id=functions-github-shboyer)

### Base Docker Images for Java

[Azul Zulu for Azure](https://www.azul.com/downloads/azure-only/zulu/?&version=java-8-lts&architecture=x86-64-bit&package=jdk)

For local development of Java function apps, download and use the [Azul Zulu Enterprise for Azure](https://assets.azul.com/files/Zulu-for-Azure-FAQ.pdf) Java 8 JDKs from [Azul Systems](https://www.azul.com/downloads/azure-only/zulu/). Azure Functions uses the Azul Java 8 JDK runtime when you deploy your function apps to the cloud.