# Desplegar una aplicación web en Cloud Foundry de IBM Cloud

> Presentación [Introducción a Cloud Foundry](https://ibm.box.com/v/cf-ppt)

Este tutorial te indicará como desplegar una aplicación web sobre Cloud Foundry de IBM Cloud usando la ventana de comandos. Una vez la aplicación este desplegada, esta será accesible desde cualquier navegador web. 

## Servicios Incluidos
* [IBM Cloud - Cloud Foundry](https://www.ibm.com/cloud/cloud-foundry): Servicio en la nube que ejecuta código fuente en una plataforma como servicio (PaaS). Open source, serverless y altamente escalable.

## Requisitos básicos
* Ventana de comandos como `Terminal` o `PowerShell`
* Editor de texto/código como `Notepad++` o `Visual Studio Code`
* Cuenta activa de [IBM Cloud](https://console.bluemix.net)

## 1. Crear, probar y configurar la aplicación web
Revisa cada uno de los siguientes tutoriales para configurar una aplicación web según el lenguaje/framework de tu preferencia:
* Angular: https://github.com/afforeroc/angular-cf
* Express: https://github.com/afforeroc/express-cf
* Flask: https://github.com/afforeroc/flask-cf
* PHP: https://github.com/afforeroc/php-cf
* React: https://github.com/afforeroc/react-cf
* Vue.js: https://github.com/afforeroc/vuejs-cf

## 2. Instalar IBM Cloud CLI
Instala según tu sistema operativo
* Instala en Mac/Linux: `$ curl -sL https://ibm.biz/idt-installer | bash`
* Instala en Windows: https://clis.ng.bluemix.net/download/bluemix-cli/latest/win64
* Verifica la versión del CLI: `$ ibmcloud -v`

## 3. Iniciar sesión con IBM Cloud CLI
Sigue las instrucciones interactivas del CLI en cada paso 
* Inicia sesión en IBM Cloud: `$ ibmcloud login`
* Apunta al espacio de trabajo de Cloud Foundry: `$ ibmcloud target --cf`
* Si deseas hacer cambios a tu sesión: `$ ibmcloud target -r <REGION> -o <ORG> -s <SPACE>`

## 4. Desplegar la aplicación usando el CLI
* Posicionate en la carpeta raíz de la aplicación web
* Sube la aplicación a Cloud Foundry de IBM Cloud: `$ ibmcloud app push`
* Visualiza tu aplicación web accediendo al [Dashboard de IBM Cloud](https://console.bluemix.net/dashboard/apps)

## Links de interés:
* Documentación de IBM Cloud CLI: https://console.bluemix.net/docs/cli/reference/ibmcloud/bx_cli.html#ibmcloud_cli
* Documentación de Cloud Foundry: https://docs.cloudfoundry.org/