# Deploy a web app using Cloud Foundry of IBM Cloud
Tutorial to learn how to deploy (step by step) a web app directly using Cloud Foundry service of IBM Cloud.
Once the application is deployed, this will be accessible from any web browser.
> Slides [Introducción a Cloud Foundry](https://ibm.box.com/v/cf-ppt)

## Tutorial
This tutorial was designed to be done on a personal computer.<br> 
Most every steps require using of console commands except when is indicated.

### Included services
* [IBM Cloud - Cloud Foundry](https://www.ibm.com/cloud/cloud-foundry): Cloud service runs source code on a platform as a service (PaaS). Open source, serverless and highly scalable service.

### Basic requirements
* Command prompt like Terminal(Linux) or PowerShell(Windows).
* Text editor like Notepad++, Visual Studio Code, etc.
* Active account of [IBM Cloud](https://console.bluemix.net).

### 1. Create and configure a web app to deploy on Cloud Foundry
Review each of these following tutorials according to the language or framework of your preference.
* [Create and configure an Express app to deploy on Cloud Foundry](https://github.com/afforeroc/express-cf)
* [Create and configure a Flask app to deploy on Cloud Foundry](https://github.com/afforeroc/flask-cf)


### 2. Install IBM Cloud CLI
Install on respective operating system.
* Install on Mac/Linux. 
```
curl -sL https://ibm.biz/idt-installer | bash
```

* Install on Windows.<br>
Download [here](https://clis.ng.bluemix.net/download/bluemix-cli/latest/win64)

* Verify IBM Cloud CLI version. 
```
ibmcloud -v
```

### 3. Sign in with IBM Cloud CLI
Follow interactive instructions of CLI.
* Sign in to IBM Cloud.
```
ibmcloud login
```

* Target to the Cloud Foundry workspace.
```
ibmcloud target --cf
```

* If you want to make changes to your session.
```
ibmcloud target -r <REGION> -o <ORG> -s <SPACE>
```

### 4. Deploy the app using the CLI
* Position yourself in root folder of the web app. 
> e.g.
```
cd flask-app\
```


* Upload the app to IBM Cloud Cloud Foundry.
```
ibmcloud app push
```

* View your web application by accessing the [Dashboard de IBM Cloud](https://console.bluemix.net/dashboard/apps).

## Reference links
* [IBM Cloud CLI documentation](https://console.bluemix.net/docs/cli/reference/ibmcloud/bx_cli.html#ibmcloud_cli)
* [Cloud Foundry Documentation](https://docs.cloudfoundry.org/)
