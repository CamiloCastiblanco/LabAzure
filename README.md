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



