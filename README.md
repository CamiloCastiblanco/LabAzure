# LabAzure
## Prerrequisitos:

- Se crea un proyecto en Azure y que se llame PartsUnlimited, en mi caso se llama PartsUnlimited2 ya que hubo un error a lo largo del proceso del laboratorio y opté por crear uno nuevo 

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/PreReq.png)

##Comienzo laboratorio

### Task 1:

- Se crea una base de datos en sql llamada partsunlimited

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/baseParts.png)

- Se crean 2 App Services, uno para QA y otro para Produccion

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/AppServices.png)

- A pesar de que la configuración de firewalls, que hay en el laboratorio, ya no existe, Windows Defender nos da la posibilidad de implementar este servicio en nuestra base 

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/Firewalls.png)

### Task 2:

- Vamos ahora a los pipelines del proyecto de Azure DevOps

- Borramos el pipeline que existe y creamos uno nuevo que se llame PUL-CICD

- Creamos un stage que se llame QA y lo configuramos

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/Stage_Config.png)

- Nos queda un artifact y un stage en el pipeline

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/Artifact_Stage.png)

- Habilitamos el Continuous deployment del proyecto

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/CD.png)

### Task 3:

- Vamos a la base de datos de SQL en el Azure DevOps y revisamos los connection Strings

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/conecctionStrings.png)

- Ahora vamos a la configuración del servicio de QA y lo dejamos de la siguiente manera

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/connectionQA.png)

### Task 4:

- Ahora vamos a los files del repo

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/Files.png)

- Buscamos un archivo llamado _Layout.cshtml

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/Layout.png)

- Lo editamos

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/LayoutModified.png)

- Hacemos commit a los cambios y esperamos a que se complete el build del proyecto

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/FollowinRunning.png)

- Vamos a los releases del proyecto y confirmamos que si se completó el proceso 

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/releaseFinish.png)

- Se desplegó en el servidor pero ocurrió un error

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/serverError.png)

### Task 5:

- Clonamos el stage

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/CloneQA.png)

- Configuramos el stage QA que teniamos 

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/ConfigQA1.png)


![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/ConfigQA2.png)

- Vamos a la security de los queries 

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/SecurityQueries.png)

- Le damos permiso de lectura al proyecto

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/ReadPerm.png)

- Cambiamos el nombre de la copia de QA al de Prod

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/QAtoProd.png)

- Habilitamos la pre aprobación para el despliegue y la configuramos

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/PreDeploy.png)

- Vamos a la configuración del stage de Prod y le damos un nuevo App service

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/ConfigProd.png)

- Nuevamente vamos al Layout para cambiar su version a 3.0

![Image text](}https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/Layout3.0.png)

- Se obtuvo un error en QA, por lo que nuevamente debemos ir a los Queries y encontrar el bug que se llama Decline in orders noticed

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/DeclineInOrders.png)

- Cambiamos el estado del bug para solucionarlo

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/bugDone.png)

- Esperamos a que nuevamente corra el pipeline y le damos permisos a prod para que pueda desplegarse, sin embargo, no me deja ya que yo mismo lo solicité

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/AprobacionDeploy.png)

### Task 6:

- Vamos a los deployments slots del  service de produccion en el portal azure

- Agregamos un slot nuevo y lo configuramos

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/newSlot.png)

- Vamos nuevamente al azure devops y entramos al stage de prod para seleccionar la app de deploy de azure y lo configuramos

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/NewServiceName.png)

 - Nuevamente vamos al Layout y dejamos la versión en 4.0

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/Layout4.0.png)

- Nuevamente no me deja aprobar la solicitud de despliegue por yo haber creado el release, sin embargo, fui al portal azure y le hice swap a los slots como paso final 

![Image text](https://github.com/CamiloCastiblanco/LabAzure/blob/main/imgAzure/Swap.png)


## Sitio deplegado

https://brayan-castiblanco-prod.azurewebsites.net




