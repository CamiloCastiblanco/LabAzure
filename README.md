# LabAzure
## Prerrequisitos:

- Se crea un proyecto en Azure y que se llame PartsUnlimited, en mi caso se llama PartsUnlimited2 ya que hubo un error a lo largo del proceso del laboratorio y opté por crear uno nuevo 

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)

##Comienzo laboratorio

### Task 1:

- Se crea una base de datos en sql llamada partsunlimited

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)

- Se crean 2 App Services, uno para QA y otro para Produccion

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)

### Task 2:

- Vamos ahora a los pipelines del proyecto de Azure DevOps

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)

- Borramos el pipeline que existe y creamos uno nuevo que se llame PUL-CICD

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)

- Creamos un stage que se llame QA y lo configuramos

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)

- Nos queda un artifact y un stage en el pipeline

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)

- Habilitamos el Continuous deployment del proyecto

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)

### Task 3:

- Vamos a la base de datos de SQL en el Azure DevOps y revisamos los connection Strings

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)

- Ahora vamos a la configuración del servicio de QA y lo dejamos de la siguiente manera

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)

### Task 4:

- Ahora vamos a los files del repo

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)

- Buscamos un archivo llamado _Layout.cshtml

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)

- Lo editamos

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)

- Hacemos commit a los cambios y esperamos a que se complete el build del proyecto

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)

- Vamos a los releases del proyecto y confirmamos que si se completó el proceso 

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)

- Se desplegó en el servidor pero ocurrió un error

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)

### Task 5:

- Clonamos el stage

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)

- Configuramos el stage QA que teniamos 

![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)


![Image text](https://github.com/CamiloCastiblanco/Lab5/blob/master/img/telnet1.png)



