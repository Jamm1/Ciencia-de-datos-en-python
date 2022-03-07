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
-Si la rama actual está actualizada   
-Si hay algo para confirmar, enviar o recibir (pull).   
--Si hay archivos en preparación (staged), sin preparación(unstaged) o que no están recibiendo seguimiento (untracked) 
Si hay archivos creados, modificados o eliminados

5. Git add   
Cuando creamos, modificamos o eliminamos un archivo, estos cambios suceden en local y no se incluirán en el 
siguiente commit (a menos que cambiemos la configuración). Necesitamos usar el comando git add para incluir los 
cambios del o de los archivos en tu siguiente commit.  
  
Añadir un único archivo: git add  
  
Añadir todo de una vez: git add -A  
  
  
