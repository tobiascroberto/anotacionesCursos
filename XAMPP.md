
# XAMPP 

XAMPP es un entorno popular de desarrollo con PHP, contiene Apache+MariaDB+PHP+Perl

## Instalar en Windows 

* Instalar el primer resulktado en Google, apachefriends.org/es/index.html

* descargar el instalador para windows. 

** Click derecho e instalar como administrador. 

** Dar click a todo, tomcat(revisar). 

** El más importante es el myAdmind que esta creado en myAdmin. 

** XAMPP estará instalado en el disco C:/xampp 

* Cuando se ejecute XAMPP solo seleccionar redes privadas.

*  Configurar para que corra en el puerto 8012 
**  ya que puede haber otras aplicaciones que usen el puerto 80. 

* Para configurar el puerto 8012:

** Detener el servidor, luego dar click en configurar.
** Seleccionar el archivo httppd.conf 
** Luego ir y buscar la linea: 
** Listen y cambiar por Listen 8012 (el de arriba esta como comentario.)
** Luego cambiar el serverName localhost:8012, para que no tenga interferencia con otros programas

* Luego modificar el archivo httpd-ssl.conf en el boton del programa de iniciación de XAMPP.  Protocolo seguro 

** Buscar la linea Listen 443, y modificarla agregando un 1 adelante. 
** Quedaría como Listen 1443

** Luego buscar donde dice <VirtualHost_default_:443> y cambiarlo por <VirtualHost_default_:443> agregando un uno al 443. 

** Cambiar la linea de severeName más abajo por 1443 en vez 443. 

* Luego iniciar mySql en el puerto 3306.

##  Para iniciar Apache y mySql como servicios(inicio al atomatico al iniciar windows)

* Tener detenido xampp en el sistema. 

* Ir a la carperta de xampp en C:// 

* Luego buscar xampp-control. 

** Seleccionar los dos primeros para marcar las casillas con palomitas verdes.




