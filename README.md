# Deploy a web application in IBM Cloud Cloud Foundry

> Slides [Introducción a Cloud Foundry](https://ibm.box.com/v/cf-ppt)

This tutorial will tell you how to deploy an IBM Cloud Cloud Foundry web application using the command window. Once the application is deployed, it will be accessible from any web browser.

## Included services
* [IBM Cloud - Cloud Foundry](https://www.ibm.com/cloud/cloud-foundry): Cloud service that runs source code on a platform as a service (PaaS). Open source, serverless and highly scalable.

## Basic requirements
* Command window as `Terminal` o `PowerShell`
* Text or code editor as `Notepad++` o `Visual Studio Code`
* Active account of [IBM Cloud](https://console.bluemix.net)

## 1. Create, test and configure the web application
Review each of the following tutorials to configure a web application according to the language / framework of your preference:
* Angular: https://github.com/afforeroc/angular-cf
* Express: https://github.com/afforeroc/express-cf
* Flask: https://github.com/afforeroc/flask-cf
* PHP: https://github.com/afforeroc/php-cf
* React: https://github.com/afforeroc/react-cf
* Vue.js: https://github.com/afforeroc/vuejs-cf

## 2. Install IBM Cloud CLI
Install according to your operating system
* Install on Mac / Linux: `$ curl -sL https://ibm.biz/idt-installer | bash`
* Install on Windows: https://clis.ng.bluemix.net/download/bluemix-cli/latest/win64
* Verify the CLI version: `$ ibmcloud -v`

## 3. Sign in with IBM Cloud CLI
Follow the interactive instructions of the CLI at each step
* Sign in to IBM Cloud: `$ ibmcloud login`
* Target to the Cloud Foundry workspace: `$ ibmcloud target --cf`
* If you want to make changes to your session: `$ ibmcloud target -r <REGION> -o <ORG> -s <SPACE>`

## 4. Deploy the application using the CLI
* Position yourself in the root folder of the web application
* Upload the application to IBM Cloud Cloud Foundry: `$ ibmcloud app push`
* View your web application by accessing the [Dashboard de IBM Cloud](https://console.bluemix.net/dashboard/apps)

## Links of interest
* IBM Cloud CLI documentation: https://console.bluemix.net/docs/cli/reference/ibmcloud/bx_cli.html#ibmcloud_cli
* Cloud Foundry Documentation: https://docs.cloudfoundry.org/