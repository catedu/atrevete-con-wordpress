#### OPCION 2 - MANUAL \(más lenta y costosa\)

Esta es la opción 2 para instalar Wordpress en 000webhost de forma manual. Esta opción es más laboriosa, pero con mayor control y aprendizaje sobre la instalación de un sitio Wordpress desde cero. Es recomendado utilizar la opción 1, ya que todos los pasos de instalación manual no tienen nada que ver con el manejo de un Wordpress, sino más con la administración de un sitio web. Los pasos a realizar en una instalación manual son similares en caso de instalar Wordpress manualmente en otro servidor. A modo de visión general, y teniendo en cuenta que este proceso puede realizarse de diversas formas, los pasos a realizar son:

1. Crear una base de datos en el servidor de hosting
2. Descargar y descomprimir el código fuente de Wordpress en nuestro PC
3. Subir el código fuente al servidor de hosting
4. Modificar la configuración de Wordpress para que se conecte con la Base de Datos

#### 1º Crear una base de datos en el servidor de hosting

Acceder al “Menú de usuario – Mis sitios web”

![](/assets/hosting10-acceder-listado-sitios-web.png)

Clic en “Administrar sitio web”

![](/assets/hosting11-admin-sitio-web.png)

Clic en “Administrar bases de datos”

![](/assets/hosting12-acceso-bd.png)

Clic en “Nueva Base de Datos”

![](/assets/hosting13-nueva-bd.png)

La Base de Datos \(para simplificar se denomina BD\) es el almacén donde se guardarán todas las entradas de texto que escribamos en nuestro blog. Cada Wordpress necesita disponer de una BD, junto con su usuario de BD y contraseña. Para evitar problemas, el nombre de la BD y el usuario de la BD convienen que estén en minúsculas, sin espacios ni caracteres extraños.

![](/assets/hosting14-crear-bd.png)

En este ejemplo se han introducido los siguientes datos, aunque puedes escoger los que quieras:

* Nombre de la BD: wordpressbd
* Nombre de usuario de la base de datos: usuariobd
* Contraseña: passwordbd

Una vez termine el proceso, la web nos muestra el nombre de Base de Datos y el nombre de Usuario definitivos, ya que el sistema de 000webhost modifica nuestros datos y les añade un número identificativo delante. En el caso del ejemplo, la web muestra los siguientes datos:

![](/assets/hosting14bis-datos-bd-reales.png)

Por lo tanto los datos finales que obtenemos son los siguientes:

* Nombre de la BD: id3443825\_wordpressbd
* Nombre de usuario de la base de datos: id3443825\_usuariobd
* Contraseña: passwordbd

Apúntate estos últimos datos que aparezcan en tu proceso de creación de la BD ya que se necesitarán posteriormente.

##### 2º Descargar y descomprimir el código fuente de Wordpress e nuestro PC

Ir a la web de Wordpress en castellano [https://es.wordpress.org/](https://es.wordpress.org/) y descargar el código fuente de Wordpress.

![](/assets/hosting15-descargaWP.png)

Descomprimir el archivo ZIP que hemos descargado. Para ello se recomienda tener descargado e instalado el programa 7-Zip, el cual puede descargarse en [http://www.7-zip.org](http://www.7-zip.org). También se podría utilizar WinZIP, WinRAR, etc. Una vez que tengas instalado 7-Zip, clic con el botón derecho del ratón en “wordpress-4.8.2-es\_ES.zip” - Extraer aquí. Como resultado aparecerá en nuestro PC una carpeta llamada wordpress  
.

![](/assets/hosting16-descomprimir.png)

##### 3º Subir el código fuente al servidor de hosting

El objetivo de estos pasos es conseguir **desplegar **el contenido del código fuente de Wordpress en la carpeta **public\_html** del servidor.  
 Para ello, accede a la zona de administración del sitio web en la página de 000webhost.com en “Menú de usuario -&gt; Mis sitios web -&gt; Administrar sitio web -&gt; Administrador de Archivos -&gt; Carga archivos ahora”

![](/assets/hosting17-acceso-archivos.png)

Seleccionar la carpeta /  y luego clic en el icono para subir ficheros que tiene forma de nube con una flecha, en nuestro PC seleccionar el fichero wordpress-4.8.2-es\_ES.ZIP que hemos descargado de [https://es.wordpress.org/](https://es.wordpress.org/) y subirlo con el botón Upload.

![](/assets/hosting18-uploadfile.png)

Descomprimir el archivo wordpress-4.8.2-es\_ES.ZIP que acabamos de subir al servidor con "botón derecho del ratón - Extract" y se creará una carpeta llamada wordpress.

![](/assets/hosting19-descomprimir.png)

Entrar en la carpeta wordpress que se ha creado y seleccionar todos los archivos. Para seleccionar todos:

1. Seleccionar el primero de todos haciendo clic sobre él.
2. Deslizarse hasta visualizar el último de todos los archivos.
3. Presionar y mantener presionada la tecla “shift” \(la tecla de mayúsculas, cuyo dibujo es una flecha que apunta hacia arriba, y que está en el teclado a la izquierda de la tecla Z, y también debajo de la tecla Intro\) y hacer clic sobre el último archivo. Y quedarán seleccionados todos los archivos
   .

Una vez que estén todos seleccionados, clic sobre la selección con el "botón derecho del ratón", y opción “Move”

![](/assets/hosting20-mover.png)

Haciendo clic en Change, cambiaremos la carpeta de destino a mover y seleccionaremos la carpeta **public\_html**, y finalmente clic en el botón "Select This".  
".

![](/assets/hosting21-cambiar carpeta destino.png)

![](/assets/hosting22-cambiar-carpeta.png)

![](/assets/hosting23-carpeta-public_html.png)

Ahora podremos borrar el archivo wordpress-4.8.2-es\_ES.ZIP y también podremos borrar la carpeta wordpress-4.8.2-es\_ES  
 haciendo clic con el botón derecho del ratón - Delete.

![](/assets/hosting25-delete.png)

##### 4º Modificar la configuración de Wordpress para que se conecte con la Base de Datos

Entrar en la carpeta **public\_html**, y ahí cambiar el nombre del archivo **wp-config-sample.php** por** wp-config.php**, dándole al “botón derecho del ratón – Rename”

![](/assets/hosting26-rename.png)

![](/assets/hosting27-rename2.png)

Clic en wp-config.php con el “botón derecho del ratón – Edit”

![](/assets/hosting28-edit.png)

Habrá que modificar en el archivo el nombre de la Base de Datos, el usuario de la Base de Datos y su password con los datos que nos habíamos apuntado en uno de los pasos anteriores. Siguiendo los datos de este paso a paso, las líneas a modificar quedarían así:

`define('DB_NAME', 'id3443825_wordpressbd');`

`define('DB_USER', 'id3443825_usuariobd');`

`define('DB_PASSWORD', ' passwordbd');`

**¡POR FIN!              
**

Si hemos realizado todo correctamente, ahora ya podemos acceder a la dirección web de nuestro sitio, que en el caso de este ejemplo sería [http://cursowpaularagon.000webhostapp.com](http://cursowpaularagon.000webhostapp.com) y veremos la página de instalación de Wordpress, en la cual vamos a poner el título principal de nuestro blog \(más tarde podremos cambiarlo\) y a crear un usuario ADMINISTRADOR de nuestro sitio web, con una contraseña y nuestro email. Evitaremos que el nombre de usuario sea admin, ya que es un problema de seguridad.

![](/assets/hosting29-instalar-wp.png)

Ahora podremos entrar al Escritorio de Administración de nuestro blog Wordpress a través de esta dirección:

[https://cursowpaularagon.000webhostapp.com/wp-login.php  ](https://cursowpaularagon.000webhostapp.com/wp-login.php)

o de esta otra:

[https://cursowpaularagon.000webhostapp.com/wp-admin/](https://cursowpaularagon.000webhostapp.com/wp-admin/)

