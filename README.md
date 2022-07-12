## AzureWebApp

The goal of this project is to develop and deploy an end to end web application on Azure with a frontend,a backend,
a database and some user authentication using Azure Static Web Apps, Cosmos DB, VSCode and GitHub Actions!

# Prerequisites

* Basic JavaScript knowledge
* A Microsoft Azure account
* A GitHub account
* Visual Studio Code (VSCode)
* Node.js 14 or 16 installed

# What is Azure Static Web Apps

Azure Static Web Apps is a service that enables developers to deploy their web applications on Azure in a seamless way.
This means developers can focus on their code and spend less time administering servers!

So, with Azure Static Web Apps (aka SWA), developers can not only deploy frontend static apps and their serverless backends
but they can also benefit from features like Custom domains, pre-prod environments, authentication providers, custom routing and more.

## Who is it for?

Azure Static Web Apps is for every developer who wants to spend more time in their code editor than they do managing resources in the cloud.

If you are a so-called "Full stack developer", then you probably want to deploy both your frontend and your backend to the cloud,
ideally with limited administration and configuration management.

## Front end developers

Azure Static Web Apps supports many frameworks and static site generators out of the box.
If you are using a framework like Angular, React, Vue.js, a site generator like Gatsby,
Hugo or one of the many solutions Azure Static Web Apps supports, then you don't have to take care of the deployment.
If you have a specific need to customise the build for your app, you can configure it yourself very easily!

## Backend developers

Azure Static Web Apps relies on Azure Functions for your application backend.
So, if you are developing in JavaScript, Java, Python or .NET, SWA makes it very easy to deploy your backend as well!

You can find the official Static Web Apps documentation here: https://aka.ms/swadocs

# Test your project locally

## The Static Web App CLI

The Static Web Apps Command Line Interface, also known as the SWA CLI,
serves as a local development tool for Azure Static Web Apps. In our case, we will use the CLI to:

* Serve static app assets
* Serve API requests
* Emulate authentication and authorization
* Emulate Static Web Apps configuration, including routing

You can install the CLI via npm.
````shell
npm install -g @azure/static-web-apps-cli
````

## Run your project locally

The CLI offers many options, but in our case we want it to serve both our API located in our api folder
and our web application located in our www folder.

In your terminal, type the following command to start your project:
````shell
swa start www --open --api-location api
````
A local web server will be started at http://localhost:4280 to run your app.
