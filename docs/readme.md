**Antoni Cabida Sales**

Sistemas de control de versiones

¿Qué es Git? ¿Qué metodología usaré? ¿Por qué utilizaré esa metodología?

Git es un sistema de control de versiones distribuido ampliamente utilizado en el desarrollo de software. Permite a los equipos de desarrollo colaborar de manera eficiente en proyectos, rastreando los cambios en el código fuente y coordinando el trabajo de múltiples desarrolladores. Cada desarrollador tiene una copia local completa del repositorio, lo que facilita el trabajo sin conexión y la integración de cambios.

La metodología de desarrollo que utilizaré en este proyecto es GitFlow. GitFlow es un modelo de ramificación popular que define un conjunto de reglas para la gestión de ramas en un repositorio Git. Está diseñado para facilitar el desarrollo colaborativo y el mantenimiento del código, especialmente en proyectos con lanzamientos regulares.

Debido a su estructura clara y su capacidad para gestionar proyectos con múltiples versiones y características en desarrollo simultáneo. GitFlow separa las ramas para nuevas características, lanzamientos y correcciones de errores, lo que simplifica el seguimiento de los cambios y la gestión del flujo de trabajo. Además, proporciona un marco establecido para el control de versiones y la colaboración entre equipos de desarrollo.

Al adoptar GitFlow, espero mejorar la organización del proyecto, reducir los conflictos de código y facilitar la implementación de nuevas características y correcciones de errores de manera ordenada y eficiente.

Esta metodología nos permite mantener una rama de producción estable (main) y una rama de desarrollo (develop), asegurando que los cambios se integren y prueben de manera adecuada antes de ser lanzados a producción.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Aquí comenzaré con los pasos a seguir para la práctica.

El usuario 1 abrirá GitHub en su navegador y creará un nuevo repositorio. Asignará un nombre al repositorio y una descripción opcional. Una vez creado, copiará la URL del repositorio.

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.001.jpeg)

Una vez creado, ell usuario 1 abrirá su terminal, navegará al directorio donde desea clonar el repositorio y ejecutará el siguiente comando para clonar el repositorio:

“git clone https://github.com/acabidasales/control\_de\_versiones.git”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.002.png)El usuario 1, instalará la boilerplate proporcionada con los siguientes comandos: “npm install html5-boilerplate”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.003.png)

Y una vez instalado, introduciremos el siguiente comando para iniciar un nuevo sitio con el boilerplate:

“npm init html5-boilerplate nuevo-sitio”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.004.png)

Entrará en la carpeta creada y usará “npm install” para instalar las dependencias correspondientes.

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.005.jpeg)

Una vez hecho esto, el usuario 1 creará las ramas iniciales según la metodología GitFlow tras salir del directorio anterior.

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.006.png)

Ahora, el usuario 1 modifica el archivo index.html quedando de la siguiente forma:

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.007.jpeg)Tras eso, el usuario 1 agregará, confirmará y subirá los cambios al repositorio con los siguientes comandos:

“git add .” (Imposible añadir captura debido al gran contenido de la carpeta node\_modules) “git commit -m "Implementada la estructura inicial"”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.008.jpeg)

“git push origin develop”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.009.jpeg)

“git push origin main”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.010.png)

Y podremos comprobar en github las ramas y el contenido.

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.011.png)

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.012.jpeg)

El Usuario 2 abrirá su terminal y clonará el repositorio de forma local. Tras eso navegará al directorio del repositorio clonado.

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.013.jpeg)

Creará una nueva rama para la feature de la sección "Modificar contenido HTML" a partir de la rama develop usando el comando:

“git checkout -b feature/modificar\_contenido\_HTML develop”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.014.png)

El usuario 2 modificará el archivo index.html y lo requerido para realizar la implementación de la sección "Modificar contenido HTML", haciéndola también útil para cambiar el texto al hacer clic sobre el botón.

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.015.jpeg)

Agregará y confirmará los cambios regularmente mientras trabaja en la feature:

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.016.png)

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.017.png)

El Usuario 2 creará una nueva rama para la feature de la sección "Modificar atributos HTML" a partir de la rama develop usando el comando:

“git checkout -b feature/modificar\_atributos\_HTML develop”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.018.png)

El Usuario 2 modificará el archivo index.html y lo requerido para realizar la implementación de la sección "Modificar atributos HTML", haciéndola también útil para cambiar los atributos del texto al hacer clic sobre el botón.

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.019.jpeg)

Agregará y confirmará los cambios de la feature con los siguientes comandos: “git add .”

“git commit -m "Agregar sección Modificar atributos HTML"”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.020.jpeg)El Usuario 2 subirá ambas ramas al repositorio de github con los siguientes comandos: “git push origin feature/modificar\_contenido\_HTML”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.021.jpeg)

“git push origin feature/modificar\_atributos\_HTML”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.022.jpeg)

Una vez que ambas features estén listas, el Usuario 2 fusionará las ramas de las features a la rama develop con los siguientes comandos:

“git checkout develop”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.023.png)

“git merge feature/modificar\_contenido\_HTML”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.024.jpeg)

“git merge feature/modificar\_atributos\_HTML”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.025.jpeg)Aquí podemos ver un conflicto, también visto desde visual estudio en ambos archivos: index.html (Aceptaré ambos cambios)

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.026.png)

Solución:

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.027.png)

App.js (Aceptaré ambos cambios)

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.028.png)

Solución

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.029.png)

Añadimos otra vez los archivos con git add:

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.030.jpeg)

Y hacemos un commit:

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.031.png)Después de resolver los conflictos y confirmar los cambios, mando los cambios a github con el siguiente comando:

“git push origin develop”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.032.jpeg)

Ahora, el Usuario 3 abrirá su terminal y clonará el repositorio de forma local. Tras eso navegará al directorio del repositorio clonado.

“git clone <https://github.com/acabidasales/control_de_versiones.git>”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.033.jpeg)

Creará una nueva rama para la feature de la sección "Modificar estilos CSS" a partir de la rama develop usando el siguiente comando:

“git checkout -b feature/modificar\_estilos\_CSS develop”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.034.png)

El Usuario 3 modificará el archivo index.html y lo requerido para realizar la implementación de la sección "Modificar estilos CSS", haciéndola también útil para cambiar los estilos del texto al hacer clic sobre el botón.

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.035.jpeg)Agregará y confirmará los cambios de la feature con los siguientes comandos: “git add .”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.036.png)

“git commit -m "Agregar sección Modificar estilos CSS"”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.037.png)

El Usuario 3 subirá la rama de la feature al repositorio remoto con el siguiente comando: “git push origin feature/modificar\_estilos\_CSS”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.038.jpeg)

Y una vez la feature esté lista, cambia de rama a la develop y la fusionará usando el siguiente comando:

“git merge feature/modificar\_estilos\_CSS”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.039.jpeg)

Y subirá los cambios al repositorio remoto:

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.040.png)Ahora, con todos los cambios preparados en la rama develop, el usuario 1 mandará todos los cambios, tras comprobar que todas las features funcionan, primero actualizando su repositorio, a la rama main con el siguiente comando:

“git pull origin develop”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.041.jpeg)

“git checkout main”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.042.png)

“git merge develop”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.043.png)

Ahora hace un commit para confirmar la fusión con el siguiente comando: “git commit -m "Integrados los cambios de la rama develop a la rama main"”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.044.jpeg)

Y lo sube al repositorio remoto: “git push origin main”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.045.png)

Ahora creará la etiqueta de la versión del repositorio con el siguiente comando: “git tag v1.0”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.046.png)

El Usuario 1 creará una nueva rama llamada test, que será utilizada por los testers para probar el desarrollo antes de implementarlo en producción (Dado a que no hay testers, se ha incorporado directamente anteriormente):

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.047.png)Una vez realizados los pasos anteriores, el Usuario 1 subirá la rama test y las etiquetas (v1.0) al repositorio remoto con los siguientes comandos:

“git push origin test”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.048.png)

“git push origin v1.0”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.049.png)

El Usuario 1 creará una carpeta en el proyecto llamada gitHooks donde se almacenarán los scripts de los hooks, aparte de la integrada en el archivo .git. Ahí creará un archivo llamado “post-checkout” con el siguiente contenido:

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.050.png)

Que nos asegurará instalar las dependencias. No necesito dar permisos de ejecución ya que estoy sobre windows.

Ahora configurará git para usar los hooks con el siguiente comando: “git config core.hooksPath gitHooks”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.051.png)

Ahora creará dentro de esa carpeta un archivo llamado “commit-msg” con el siguiente contenido:

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.052.jpeg)Y también dentro de esa carpeta, creará un archivo llamado “pre-commit” con el siguiente contenido, que verificará los carácteres extraños.

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.053.png)

Ahora usaremos los siguientes comandos para instalar el plugin eslint: “npm install -g eslint”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.054.png)

“npm install --save-dev eslint-plugin-html”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.055.jpeg)

Ahora, el usuario 1 también añadirá al hook “pre-commit” el siguiente contenido para revisar el formato HTML:

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.056.png)

También añadiré los nuevos cambios hechos por el plugin y lo añadiré con un commit siguiendo el formato:

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.057.png)

Añadirá los hooks al área de preparación y hará un commit usando los siguientes comandos:

“git add gitHooks/post-checkout gitHooks/commit-msg gitHooks/pre-commit”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.058.png)“git commit -m "MOTIVO DEL COMMIT: Subir hooks IMPLEMENTACIÓN: Carpeta de hooks"” (Asi comprobaré si funcionan los hooks)

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.059.jpeg)

Añado los cambios al repositorio remoto:

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.060.jpeg)

Ahora creo la rama gh-pages con el siguiente comando: “git checkout -b gh-pages”

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.061.png)

Añado el documento nuevo con la documentación a y hago el commit.

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.062.jpeg)

Y lo subo al directorio remoto:

![](Aspose.Words.e18a8b85-5ae4-498e-9b7e-c5b2b9a220d8.063.jpeg)

(Vuelve a darme un error en el deploy de github pages) sin entender el porqué
