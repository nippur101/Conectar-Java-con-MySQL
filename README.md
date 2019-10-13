# Conectar-Java-con-MySQL
Metodo para crear una conexion entre java y MySQL y como leer una tabla desde la base de datos

-En Libraries debe esta instalado MySQL JDBC Drivers-mysql-connectors....

-en Class.forName("org.gjt.mm.mysql.Driver"); debe estar la direccion correcta de los drivers de acuerdo a la version

-en servidor="jdbc:mysql://localhost:3306/pruebarol"; habitualmente es localhost:3306/ (NOMBRE DE LA BASE DE DATOS)

-en ResultSet rs = s.executeQuery ("select * from (NOMBRE DE LA TABLA)");

