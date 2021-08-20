# Multi Client Application Example
Example of Multiple WASM Client in Blazor project.

## Description
This application demonstrate the use of **Multiple Client Application** in a Blazor WASM project.  

Each application will running on a different port or host name.  
The Blazor Server project, via the Web API controllers, will provide the data for both projects.

From original question by _alexsey bobrovitch_ on [Stackoverflow](https://stackoverflow.com/questions/68837851/file-framework-blazor-webassembly-js-is-not-found-in-hosted-application)

How to
------

Select **MultiClientApplicationWasmExample.Server** as startup method.  
The Client WASM applications are both hosted via Blazor Server project.  
The first application is hosted via TCP port 5001, the second via TCP port 5002.

Try to switch between the two client application.  
You can see that the WeatherForecast controller working as expected from both the client applications.  
Take a look to the `Route` controller configuration.

This project is based on the original documentation from Microsoft: [Hosted deployment with multiple Blazor WebAssembly apps](https://docs.microsoft.com/en-us/aspnet/core/blazor/host-and-deploy/webassembly?view=aspnetcore-5.0#hosted-deployment-with-multiple-blazor-webassembly-apps-1)
