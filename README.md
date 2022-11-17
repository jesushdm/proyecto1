## creacion de repo
git init

## añadir un fichero
git add <nombre_fichero>   # añadir un fichero
git add *                  # añadir todos los ficheros del directorio (NO incluye ocultos)
git add .                  # añadir todos los ficheros del directorio (SI incluye ocultos)
Empezar a controlar el fichero = Pasar el fichero al área de STAGING

# ¿Qué guarda Git?
Sólo guarda ficheros, NO GUARDA DIRECTORIOS

# OBJETOS EN GIT
## Workspace
La carpeta en la que tengo mi proyecto, en la que trabajo
## Staging
Es un fichero dentro de la carpeta .git, que va anotando los cambios que se van a mandar al REPO desde el área de STAGING
## Repositorio
La carpeta .git

## Informacion de estado del proyecto
git status

## ¿Que es un commit?
-Un """paquete de cambios""" que se registra en el repo
-Se aplican de forma INCREMENTAL (es decir, los cambios producidos en cada archivo, no el archivo en sí mismo)

## Sacar un fichero del área de STAGING
git rm --cached <nombre_fichero>

## Borra el fichero...¿de donde? De todos los sitios
- WORKSPACE
- en el STAGING se le dice qeu en el proximo "paquete de cambios", se elimine el fichero
git rm  <nombre_fichero> 

FileAv1 ---> Repo ---> Modif FileAv2 ---> Repo
FileBv1 ---> C1                      C2 --------------> rm FileBv1 --------> C3 -------------->
                                        ^FOTO: FileAv2                          ^FOTO: FileAv2 
                                               FileBv1