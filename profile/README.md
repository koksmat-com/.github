### Koksmat: An Open Source Framework for Custom Apps on Microsoft 365

# [Get Started](https://github.com/new?template_name=tutorial-gettingstarted&template_owner=koksmat-com)


# Or read more ...
A guide for developers and administrators who want to leverage the power of MACH architecture and citizen development

### What is Koksmat?

Koksmat is an open source framework that enables you to create, deploy, and manage custom apps on Microsoft 365. It is based on the MACH (Microservices, API-first, Cloud-native, and Headless) architecture, which offers flexibility, scalability, and performance for modern web applications. Koksmat is designed to be accessible and user-friendly for both developers and administrators, as well as citizen developers who want to build apps without coding.
Why use Koksmat?

### Koksmat offers several advantages over traditional app development methods on Microsoft 365, such as:

-	It allows you to use any front-end technology of your choice, such as React, Angular, Vue, or Blazor, to create rich and interactive user interfaces.
-	It provides a set of reusable and configurable microservices that handle common app functionalities, such as authentication, authorization, data storage, notifications, workflows, and analytics.
-	It exposes a consistent and secure API layer that connects your app to Microsoft 365 services, such as SharePoint, Teams, Graph, Power Platform, and Azure.
-	It supports a cloud-native approach that enables you to deploy and scale your app on any cloud platform, such as Azure, AWS, or Google Cloud.
-	It simplifies the app lifecycle management by providing tools and best practices for testing, debugging, monitoring, and updating your app.

### How to get started with Koksmat?

To get started with Koksmat, you need to have a Microsoft 365 subscription and an account on GitHub, where you can access the Koksmat repository and documentation. You also need to install the Koksmat CLI, which is a command-line tool that helps you create, configure, and run your app. You can follow these steps to create your first app with Koksmat:

-	Clone the Koksmat repository from GitHub and install the dependencies.
-	Use the `Koksmat Bridge` (UI) to create a new app project and choose a front-end technology.
-	Add the microservices that you need for your app and configure them with the Koksmat CLI.
-	Write your app logic and UI code using your preferred code editor and framework.
-	Use the `Koksmat Bridge` to test, build, and deploy your app to the cloud.
-	Use the `Koksmat Bridge` dashboard to manage and monitor your app.

For more details and examples, please refer to the Koksmat documentation and tutorials on GitHub.

### Get started by using this template

[https://github.com/new?template_name=tutorial-gettingstarted&template_owner=koksmat-com](https://github.com/new?template_name=tutorial-gettingstarted&template_owner=koksmat-com)


The core of Koksmat Bridge is enabled by adding a file **.devcontainer/devcontainer.json**
```json 
{
	"name": "Koksmat",
	"image": "ghcr.io/koksmat-com/ui:v1.0.0.koksmat-9",
	"features": {
		"ghcr.io/devcontainers/features/azure-cli:1": {
			"version": "latest"
		},
		"forwardPorts": [
			3001
		],
		"containerEnv": {
			"HOMEPAGE": "koksmat",
			"NEXTAUTH_SECRET": "na",
			"KOKSMATROOT": "/usr/src/app/apps/www/",
			"KITCHENROOT": "/usr/src/app/apps/kitchens/"
		},
		"postCreateCommand": "cd /usr/src/app/apps/www  &&  npm run start"
	}

```


## What is Koksmat all about?

Your helping hand in our digital Kitchen. The word
Koksmat is danish and means the helping hand to the chef in the kitchen
of a ship.

### The Bridge
The `Bridge` is a web interface that supports you and your guest on the journey through a great digital menu of tastefull digital dishes. 
