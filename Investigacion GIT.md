# Investigacion GIT  
![GIT](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e0/Git-logo.svg/640px-Git-logo.svg.png)  
**Presentado por:** Jose Andres Marquez Morataya
Desarrollo de investigacion sobre el funcionamiento de git  
La herramienta de GIT es sumamente usada por los desarrolladores de software para llevar el control de cambios y el compartir el codigo de una manera facil  
## Control de versiones  
El control de versiones es un sistema que registra los cambios en un archivo o conjunto de archivos a lo largo del tiempo para que pueda 
recuperar versiones específicas más adelante. Entonces,idealmente, podemos colocar cualquier archivo en la computadora en el control de versiones.  
Un Sistema de control de versiones (VCS) le permite revertir los archivos a un estado anterior, revertir todo el proyecto a un estado anterior, revisar 
los cambios realizados a lo largo del tiempo, ver quién modificó por última vez algo que podría estar causando un problema, quién introdujo un problema 
y cuando, y más informacion que ayuda a la identificacion del codigo y al orden.  
**Git** es un sistema de control de versiones distribuido . Entonces, Git no depende necesariamente de un servidor central para almacenar todas las versiones 
de los archivos de un proyecto. En cambio, cada usuario “clona” una copia de un repositorio (una colección de archivos) y tiene el historial completo 
del proyecto en su propio disco duro. Este clon tiene todos los metadatos del original, mientras que el original en sí se almacena en un servidor 
autohospedado o en un servicio de alojamiento de terceros como GitHub.  
## Principales Comandos  
1. Git clone   
Git clone es un comando para descargarte el código fuente existente desde un repositorio remoto (como Github, por ejemplo). 
En otras palabras, Git clone básicamente realiza una copia idéntica de la última versión de un proyecto en un repositorio y la guarda en tu ordenador.  
  
git clone < link-con-nombre-del-repositorio >  

2. Git branch   
Las ramas (branch) son altamente importantes en el mundo de Git. Usando ramas, varios desarrolladores 
pueden trabajar en paralelo en el mismo proyecto simultáneamente. Podemos usar el comando git branch para crearlas,
 listarlas y eliminarlas.  
 Creando una nueva rama: git branch  
  
Visualización de ramas: git branch git branch --list  
  
Borrar una rama: git branch -d  
  
3. Git checkout   
Este es también uno de los comandos más utilizados en Git. 
Para trabajar en una rama, primero tienes que cambiarte a ella.
 Usaremos git checkout principalmente para cambiarte de una rama a otra. 
 También lo podemos usar para chequear archivos y commits. git checkout  

Hay también un comando de acceso directo que te permite crear y cambiarte a esa rama al mismo tiempo: git checkout -b

4. Git status   
El comando de git status nos da toda la información necesaria sobre la rama actual.   
git status  
Podemos encontrar información como:   
Si la rama actual está actualizada   
Si hay algo para confirmar, enviar o recibir (pull).   
Si hay archivos en preparación (staged), sin preparación(unstaged) o que no están recibiendo seguimiento (untracked) 
Si hay archivos creados, modificados o eliminados

5. Git add   
Cuando creamos, modificamos o eliminamos un archivo, estos cambios suceden en local y no se incluirán en el 
siguiente commit (a menos que cambiemos la configuración). Necesitamos usar el comando git add para incluir los 
cambios del o de los archivos en tu siguiente commit.  
  
>Añadir un único archivo: git add  
  
>Añadir todo de una vez: git add -A  
  
  
6. Git commit Este sea quizás el comando más utilizado de Git. Una vez que se llega a cierto punto en el desarrollo, queremos guardar nuestros cambios (quizás después de una tarea o asunto específico).
Git commit es como establecer un punto de control en el proceso de desarrollo al cual puedes volver más tarde si es necesario. También necesitamos escribir un mensaje corto para explicar qué hemos desarrollado o modificado en el código fuente.

  git commit -m "mensaje de confirmación"

  7. Git push Después de haber confirmado tus cambios, el siguiente paso que quieres dar es enviar tus cambios al servidor remoto. Git push envía tus commits al repositorio remoto. git push

De todas formas, si tu rama ha sido creada recientemente, puede que tengas que cargar y subir tu rama con el siguiente comando:   git push --set-upstream or git push -u origin

  8. Git pull El comando git pull se utiliza para recibir actualizaciones del repositorio remoto. Este comando es una combinación del git fetch y del git merge lo cual significa que cundo usemos el git pull recogeremos actualizaciones del repositorio remoto (git fetch) e inmediatamente aplicamos estos últimos cambios en local (git merge). git pull

  9. Git revert A veces, necesitaremos deshacer los cambios que hemos hecho. Hay varias maneras para deshacer nuestros cambios en local y/o en remoto (dependiendo de lo que necesitemos), pero necesitaremos utilizar cuidadosamente estos comandos para evitar borrados no deseados.

Una manera segura para deshacer nuestras commits es utilizar git revert. Para ver nuestro historial de commits, primero necesitamos utilizar el git log -- oneline: Entonces, solo necesitamos especificar el código de comprobación que encontrarás junto al commit que queremos deshacer: git revert 332184

La ventaja de utilizar git revert es que no afecta al commit histórico. Esto significa que puedes seguir viendo todos los commits en tu histórico, incluso los revertidos.

Otra medida de seguridad es que todo sucede en local a no ser que los enviemos al repositorio remoto. 
Por esto es que git revert es más seguro de usar y es la manera preferida para deshacer los commits.  
10. Git merge Cuando ya hayas completado el desarrollo de tu proyecto en tu rama y todo funcione correctamente, el último paso es fusionar la rama con su rama padre (dev o master). Esto se hace con el comando git merge. Git merge básicamente integra las características de tu rama con todos los commits realizados a las ramas dev (o master). Es importante que recuerdes que tienes que estar en esa rama específica que quieres fusionar con tu rama de características.
  Por ejemplo, cuando quieres fusionar tu rama de características en la rama dev:  Primero, debes cambiarte a la rama dev: git checkout dev  
    Antes de fusionar, debes actualizar tu rama dev local: git fetch    Por último, puedes fusionar tu rama de características en la rama dev: git merge  
  
  ## Hoja de Comandos para GIT  
  Otros Comandos que se pueden utilizar en GIT  
  ![Comandos git](https://res.cloudinary.com/practicaldev/image/fetch/s--w-UEE2WQ--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/8cl1lotlaikqp8vhhr6i.png)