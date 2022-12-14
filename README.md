# An谩lisis de datos en tiempo real usando la versi贸n preliminar de _Azure Synapse Data Explorer_

## Welcome aboard! :octocat:

馃挜En este repo encontrar谩n recursos y la gu铆a para el taller t茅cnico "El mundo de Synapse dentro del universo de Azure" impartido para la comunidad de Colombia . Aqu铆 podr谩n encontrar los elementos necesarios para poder trabajar con esta herramientos. Adem谩s, m谩s abajo podr谩n encontrar recursos extras si est谩n interesados en el mundo de la data.馃挜 

馃挕 _En este link pueden consultar la  [presentaci贸n online](https://www.canva.com/design/DAFTqOkijyE/HT6Mj7NaAov4jhz59hSCCg/view?utm_content=DAFTqOkijyE&utm_campaign=designshare&utm_medium=link&utm_source=publishpresent )._

<details><summary><h2> Creaci贸n de recursos. 馃懢 <h/2></summary>

**Pasos a seguir:**

馃搶 Contar con una cuenta en [Azure Portal](https://portal.azure.com/).
  
馃搶 En la p谩gina de inicio de hacemos clic en el bot贸n de _Crear_.
  
  ![ ](DataExplorer/1-crear.png)
  
馃搶 En el buscador colocamos _Azure Synapse Analytics_.
  
  ![ ](DataExplorer/2-buscar.png)  
  
馃搶 Le asignamos una configuraci贸n de la siguiente manera.
  
**Suscripci贸n:**
  
      suscripci贸n de Azure 
  
**Grupo de recursos:**
  
      synapse-rg
      
Grupo de recursos administrado: 
  
      synapse-managed-rg 
      
Nombre del 谩rea de trabajo:
  
      synapse-ws-universo
      
**Regi贸n:** Seleccionamos la regi贸n donde ser谩 consumido por el cliente final.    
      
**Seleccionar Data Lake Storage Gen 2:** en la suscripci贸n.
  
**Nombre de cuenta:**
  
      datalakeuniverse
  
**Nombre del sistema de archivos:** 
  
      fsuniverse
  
   ![ ](DataExplorer/3-configuracion.png)     
   
馃搶 Una vez configurado hacemos clic en el bot贸n de _Revisar y Crear_ y si todo sale bien hacemos clic en el bot贸n de _Crear_ para poder obtener los recursos que usaremos, esto puede demorar un tiempo aproximado de 5 minutos. 

馃搶 Una vez que se haya completado la implementaci贸n se podr谩n observar 2 recursos, hacemos clic en el recurso de Synapse que nos redirigir谩 hacia _Synapse Studio_ mostrandonos una interfaz como la siguiete.
  
   ![ ](DataExplorer/4-abrirSynapseStudio.png)
   
</details>

<details><summary> <h2>  Creaci贸n de un grupo de Data Explorer :octocat: <h/2></summary>
   
馃搶 Dentro de _Synapse Studio_ nos dirigiremos a la siguiente ruta.
      
      Administrar > Grupos de Data Explorer > Nuevo

馃搶 Asignaremos la siguiente configuraci贸n.

**Nombre del grupo de Data Explorer:**
  
      dxpool
      
**Carga de trabajo:**
  
      optimizado para proceso

**Tama帽o:**
  
      extra peque帽o (2 n煤cleos)

馃搶 En la pesta帽a de _configuraci贸n adicional_ habilitaremos la opci贸n de _ingesta de streaming_.

馃搶 Finalmente, seleccionamos el bot贸n de _Revisar y crear_ para crear el grupo, esto puede demorar hasta 15 minutos.

</details>

<details><summary> <h2> Creaci贸n de BD y consumo de datos. 馃懢 <h/2></summary>

馃搶 Dentro de _Synapse Studio_ seleccionaremos la etiqueta de _Datos_ en la opci贸n de _Base de Datos de Data Explorer_ donde deber铆a aparecer _dxpool_

馃搶 En el panel Datos, hacemos clic en el s铆mbolo 锛? para crear una base de datos de Data Explorer nueva en el grupo dxpool con el nombre.

     iot-data

馃搶 Dentro de _Synapse Studio_ nos dirigimos al _men煤_, a la nuesv BD que nombramos  iot-data, abrimos  _Azure Data Explorer y seleccionamos _Ingerir datos nuevos_ donde insertaremos los datos que simulan un servicio de IoT.

  * El descargable se encuentra [aqu铆 en .csv](https://github.com/LizzyLucas/AzureSynapseDataExplorer-workshop/blob/main/Resources/devices.csv).

Nota: _Al finalizar no olviden eliminar todos los recursos creados y el grupo de recursos tambi茅n._

</details>

<details><summary><h2> Recomendaciones extra. 馃挕 <h/2></summary>


  鈽侊笍  [Lecci贸n gu铆a para esta taller](https://learn.microsoft.com/es-es/training/modules/explore-fundamentals-stream-processing/9-exercise-data-explorer).
  鈽侊笍  [Microsoft Learn](https://learn.microsoft.com/es-es/).
  鈽侊笍  [Azure Days](https://mvtd.events.microsoft.com/?language=Espa%C3%B1ol).
  鈽侊笍  [Ruta de aprendizaje para el DP-900](https://learn.microsoft.com/es-es/certifications/azure-data-fundamentals/).

</details>

##

**隆Bievenidas contribuciones!** :octocat: Built by _Lizzie Lucas_ 馃洜锔?



