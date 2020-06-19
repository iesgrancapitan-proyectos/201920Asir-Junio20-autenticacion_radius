# Autenticación de clientes inalámbricos a través de un servidor Radius
## Proyecto Integrado CFGS ASIR
# Autor: Jorge Rodríguez Mora

1. Establecer la arquitectura de la infraestructura.

2. Instalación de FreeRadius en el servidor.

3. Configuración del punto de acceso en modo WPA2-Enterprise con la dirección IP del servidor y una clave secreta.

4. Indicar el punto de acceso en el archivo clients.conf junto con la dirección ip del punto de acceso así como la clave secreta.

5. Crear un usuario en la base de datos local sguiendo la sintaxis, todo ello en el archivo users.

6. Modificar el archivo mods-enabled/sql para permitir el uso de la base de datos mysql y descomentar las líneas sql en el archivo sites-    enabled/default e inner-tunnel.

7. Modificar el archivo mods-enabled/ldap para permitir el uso de la base de datos OpenLDAP y descomentar las líneas ldap en el archivo       sites-enabled/default e inner-tunnel.

8. Crear usuarios en la base de datos de mysql y ldap y comprobar el acceso a la red con el comando radtest.

9. En el directorio certs, cambiar la configuracion que estimemos oportuna de los archivo ca.cnf server.cnf y client.cnf, luego            ejecutaremos el comando make para la creacion de los certificados.

10. Modificar el archivo /mods-enabled/eap en el que introducermos la ruta de los certificados que creamos anteriormente.

11. Comprobar desde un sistema android o linux que el cliente puede conectarse luego de haber instalado los certificados ca.der y           client.p12.

