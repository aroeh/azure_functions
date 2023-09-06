# azure_functions
This repository will contain code specifically for Azure functions with the goal of learning basics and best practices around them.

# Tools
- Visual Studio 2022 or Visual Studio Code
- .Net6 SDK
- Azure Functions Core Tools v4 - [x64 Windows Download](https://go.microsoft.com/fwlink/?linkid=2174087)
- Powershell 7


# Getting Started
Instructions for running the functions will use Powershell

1. Change to the directory containing the .csproj

2. Build the project to ensure that the code compiles `dotnet build`
```
dotnet build
```

3. Run the API using the command `func host start`
```
func host start
```

4. Validate that the API is running and to view the OpenApi Spec
```
http://localhost:7071/api/swagger/ui
```

# OpenApi Spec
Swagger and OpenApi specs can be viewed by using the following urls

```
http://localhost:7071/api/swagger.json
```

```
localhost:7071/api/openapi/v3.json
```

# References
- [Azure Functions OpenApi Extension Repo](https://github.com/Azure/azure-functions-openapi-extension/tree/main)
- [Enable OpenApi on In-Process Functions](https://github.com/Azure/azure-functions-openapi-extension/blob/main/docs/enable-open-api-endpoints-in-proc.md)
- [Azure Functions Core Tools](https://learn.microsoft.com/en-us/azure/azure-functions/functions-run-local?WT.mc_id=dotnet-0000-juyoo&tabs=windows%2Cisolated-process%2Cnode-v4%2Cpython-v2%2Chttp-trigger%2Ccontainer-apps&pivots=programming-language-csharp)