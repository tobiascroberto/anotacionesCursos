# Guia para usar GIT (ATL Academy por Lucas Moy)

Es un repositorio de código, creado por Linus Torvalds. 

Git está construido por ramas. 

Ramas principal (master)

Los programadores pueden hacer copias del proyecto en distintas partes del tiempo.

Ir a github y registrarse. 

# En el navegador. 

* Crear una cuenta, con tu email y contraseña. 
* Crear repositorio.
* Crear un nuevo archivo 

* Commit, cuando subes un cambio y te comprometes que esta bien. 

# Instalar GItHub desktop. 

Descargar con click y seguir los pasos. 

# Configurar en la computadora las variables locales del  git

* Configurar las variables locales: 

    * El nombre:  git config --global user.name "Roberto Tobias Castillo"
    * El correo electrónico: git config --global user.email "tobiasc.roberto@gmail.com" 

* Si hay un error para cambiarlo se vuelve a ejecutar la instrucción con el dato erronéo. 

* Mostrar las configuracion globales:

git config --list 

* Se mostrarán todas las configuraciones globales, entre ellas las del nombre y correo. 

* También puedes ver la configuración especifica del valor clave : 
** Nombre: git config --global user.name 

## Obtiendo ayuda de los comandos de git 

* git help '\<verb>'
* git \<verb> --help
* man git-\<verb> man es de manual

# Inicializando un proyecto en Git. 

* Se debe de crear una carpeta en la maquina para subir los archivos. 

* mkdir "nombreCarpeta" 

* Luego entrar en la carpeta y poner el comando de 

** git init  # esto creará una instancia de git para el proyecto. 

* Si ya existen documentos en la carpeta, se debe de agregar al stage add para luego hacer el commit y luego subir a github

** git add "archivo1" "archivo2" 

** git add . # subir todos los archivos en el github

** Comando importante: git status 

** Luego escribir: git commit -m "comentario de la actualización"

** git push origin main


# Ver lo que hay en origin and remote 

* git remote -v 
* git origin -v

# 

* Cambiar el origin en el remote: 

** git remote set-url origin https://github.com/tobiascroberto/anotacionesCursos.git 

* git branch -M main 
git remote add origin  https://github.com/tobiascroberto/anotacionesCursos.git 

git push -u origin main

* Verificar el nombre de la rama: gir remote -v 



# Creacion de ramas 

* ver ramas existentes: 
** git branch (la que tiene asterisco es la rama actual)

*crear ramas: 

** git branch nombre_rama

* cambiar entre ramas: 

** checkout nombre_rama

* crear y cambiar de rama en un paso: 

** git checkout -b nombre_rama

* subir rama al repositorio remoto
** git push -u origin nueva_rama

* Eliminar una rama local 

** git branch -d nombre_rama (elminina la rama si fue fusionada con otra)

** git branch -D nombre_rama (D mayúscula fuerza la eliminación aunque no este fusionada.)

* Eliminar rama remota
** git push origin --delete nombre_rama



## Configuración para push (jal)



