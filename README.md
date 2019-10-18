# Conectar-Java-con-MySQL
Metodo para crear una conexion entre java y MySQL y como leer una tabla desde la base de datos

-Este este ejemplo tiene una base de datos en MySQL con nombre "pruebarol" y con una tabla "monstruos" (7 columnas)

-En Libraries debe esta instalado MySQL JDBC Drivers-mysql-connectors....

-En Class.forName("org.gjt.mm.mysql.Driver"); debe estar la direccion correcta de los drivers de acuerdo a la version

-En servidor="jdbc:mysql://localhost:3306/pruebarol"; habitualmente es localhost:3306/ (NOMBRE DE LA BASE DE DATOS)

-En ResultSet rs = s.executeQuery ("select * from (NOMBRE DE LA TABLA)");


ERRORES AL INTENTAR CONECTAR

ERROR
-java.math.BigInteger cannot be cast to java.lang.long?

SOLUCION

-primero se elimina archivo mysql-connector-java de la ruta C:\Program Files\NetBeans 8.2\ide\modules\ext 
-bajar el driver https://dev.mysql.com/downloads/connector/j/5.1.html, descomprime el archivo, y copia el archivo mysql-connector-java-5.1.46-bin en la ruta C:\Program Files\NetBeans 8.2\ide\modules\ext en el netbeans en prestaciones, 
-en controladores selecciona Mysql (Connector/J driver) clic derecho y en personalizar agregar el driver.

ERROR
-caching_sha2_password

SOLUCION

Usar el comando en MySQL

ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY '1234';

Donde USER:root   Password:1234


