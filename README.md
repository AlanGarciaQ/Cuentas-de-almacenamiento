# Cuentas de almacenamiento
**Objetivo:** Conocer y utilizar los diferentes recursos de almacenamiento que nos proporciona Azure.     

![](/imagenes/nube_.jpg)

**Requisitos**
- Cuenta de Azure con una suscripción activa
- Equipo de cómputo con sistema operativo: Windows, Linux o MacOs.

**Pasos**  
Se inicia sesión en Portal.Azure.com  
En la barra de búsqueda escribimos “Cuentas de almacenamiento” y lo seleccionamos.  
Damos clic en el apartado crear.

En la pestaña datos básicos, llenamos lo siguiente:  

**En Detalles del proyecto**  
Suscripción: La suscripción que queramos utilizar.  
Grupo de recursos: Podemos crear uno o seleccionar uno ya existente.  
![Imagen 1](/imagenes/Imagen1.png)

**En Detalles de Instancia**  
Nombre de la cuenta de almacenamiento: Ponemos el que queramos.  
Región: Podemos escoger cualquiera, pero si no queremos que haya mucha latencia escogemos uno cercano a donde vivimos.  
Rendimiento: Seleccionamos Estándar.  
Redundancia: Seleccionamos Almacenamiento con redundancia local.  
![](/imagenes/Imagen2.png)

A continuación, en la pestaña Redes, hacemos lo siguiente:

**En conectividad de red**  
Acceso de red: Seleccionamos la opción de habilitar el acceso público desde todas las redes.

**En Enrutamiento de red**  
Preferencia de enrutamiento: Seleccionamos Enrutamiento de red de Microsoft.

Estas configuraciones las necesitamos para realizar esta práctica.  
Para terminar, damos clic en el botón de revisar y crear, y luego en crear.  
![](/imagenes/Imagen3.png)

Cuando se termine de crear nuestro recurso, daremos clic en el botón de ir al recurso.  
En el menú de la parte de la izquierda le damos clic en la opción de contenedores.  
En el menú de la parte de arriba que apareció seleccionamos el apartado de contenedor.  
En el apartado de Nuevo contenedor, llenamos los siguiente:  
Nombre: Pondremos el nombre que queramos que tenga nuestro contendedor.  
Nivel de acceso público: Seleccionamos contenedor.  
Damos clic en el botón crear.  
![](/imagenes/Imagen4.png)

Damos clic en el contenedor que acabamos de crear para ingresar a este.  
Damos clic en el apartado de cargar.  
En el apartado de la izquierda llamado Cargar Blob, en la opción de files, damos clic en el dibujo de la carpeta.  
Seleccionamos de nuestra computadora cualquier tipo de archivo que queramos guardar en el blob.  
Cuando se termine de subir nuestro archivo le daremos clic en el botón de cargar.  
![](/imagenes/Imagen5.png)

Damos doble clic en el archivo que acabamos de subir, en las opciones que nos aparecen a la izquierda de este, copiamos la url que esta y la ponemos en el navegador, con esto podremos consultar lo que subamos a través de internet.  
![](/imagenes/Imagen6.png)

Esta es una forma de poder subir una página web, pero esta será estática, no le podremos modificar nada. Lo que acabamos de hacer es el tipo de almacenamiento llamado Blob Storage, en el que puedes subir cualquier tipo de archivo.  

---------------------------------------------------------------------------------------------------------------

A continuación, utilizaremos el tipo de almacenamiento llamado File Storage, para esto tendremos que salir de la opción de habíamos seleccionado anteriormente la de contendedores, y en su lugar seleccionaremos la opción de Recursos Compartidos de Archivos.  
En el menú de la parte de arriba que apareció seleccionamos el apartado de recurso compartido de archivo.  
En el apartado de Nuevo recurso compartido de archivos, llenamos los siguiente:  
Nombre: Pondremos el nombre que queramos que tenga nuestro recurso compartido.  
Nivel: Seleccionamos el que queramos, esto depende de que tanto se use el archivo que subiremos.

Damos clic en el botón crear.  
![](/imagenes/Imagen7.png)

Damos clic en el recurso compartido que acabamos de crear para ingresar a este.  
Damos clic en el apartado de cargar.  
En el apartado de la izquierda llamado Cargar archivos, en la opción de files, damos clic en el dibujo de la carpeta.  
Seleccionamos de nuestra computadora cualquier tipo de archivo que queramos guardar en el blob.
Cuando se termine de subir nuestro archivo le daremos clic en el botón de cargar.
![](/imagenes/Imagen8.png)

Al archivo que acabamos de subir lo podremos conectar a nuestra computadora, podemos agregar una carpeta, actualizarlo, eliminarlo y cambiarle el nivel que le pusimos anteriormente.  
Para conectarlo a nuestra computadora seleccionamos el apartado conectar.  
En el apartado de la izquierda llamado Conectar, seleccionamos el sistema operativo de nuestra computadora.  
En método de autentificación seleccionamos clave de la cuenta de almacenamiento, la otra opción de Active directory solo funciona si la cuenta que tenemos en nuestra computadora es la misma que utilizamos para ingresar a Azure.  
Copiaremos el comando que se nos muestra.  
En nuestra computadora abrimos power Shell y pegamos el comando que copiamos y damos enter. Se nos mostrara que se conectó correctamente.  
![](/imagenes/Imagen9.png)

Con esto habremos utilizado el tipo de almacenamiento llamado File Storage.

---------------------------------------------------------------------------------------------------------------

A continuación, utilizaremos el tipo de almacenamiento llamado Queo Storage (Cola), para esto tendremos que salir de la opción de habíamos seleccionado anteriormente la de Recursos Compartidos de Archivos, y en su lugar seleccionaremos la opción de Colas.  
En el menú de la parte de arriba que apareció seleccionamos el apartado de Cola.  
En el apartado de Agregar cola, llenamos los siguiente:  
Nombre de la cola: Pondremos el nombre que queramos que tenga nuestra cola.

Damos clic en aceptar.  
![](/imagenes/Imagen10.png)

Damos doble clic en la cola que acabamos de crear, podremos actualizarla, crear mensajes, quitar mensajes y quitar la cola.  
Para agregar mensaje seleccionamos el apartado agregar mensaje.  
Escribimos el mensaje que queramos agregar.  
Seleccionar en cuanto tiempo expira o seleccionar que nunca expire.  
Damos clic en aceptar.  
![](/imagenes/Imagen11.png)

Se agregará el mensaje que acabamos de crear a la cola.  
![](/imagenes/Imagen12.png)

Con esto habremos utilizado el tipo de almacenamiento llamado Queo Storage (Cola).

---------------------------------------------------------------------------------------------------------------

A continuación, utilizaremos el tipo de almacenamiento llamado Tablas, para esto tendremos que salir de la opción de habíamos seleccionado anteriormente la de Colas, y en su lugar seleccionaremos la opción de Tablas.  
En el menú de la parte de arriba que apareció seleccionamos el apartado de Tablas.  
En el apartado de Agregar tabla, llenamos los siguiente:  
Nombre de la tabla: Pondremos el nombre que queramos que tenga nuestra tabla.

Damos clic en aceptar.  
![](/imagenes/Imagen13.png)

Si queremos editar la tabla que acabamos de crear tenemos que buscar en el menú de la izquierda la opción de Explorador de almacenamiento (Versión preliminar).  
En el menú nuevo que se abrió buscamos Tablas y en el lado derecho se nos mostrara nuestra tabla y la seleccionaremos.  
![](/imagenes/Imagen14.png)

Seleccionamos el apartado de agregar entidad.  
Damos clic en agregar propiedad, ahí llenamos lo siguiente:  
nombre de la propiedad: Escribimos el nombre que queramos que tenga nuestra propiedad.  
Tipo: Escribiremos el tipo que es nuestra entidad.  
Valor: Escribimos el valor que tenga nuestra entidad.  
Damos clic en insertar.  
![](/imagenes/Imagen15.png)

Se nos mostrara la entidad que creamos. Podemos crear tantas entidades como deseemos, esto dependerá de los datos que queramos guardar en nuestra tabla.
![](/imagenes/Imagen16.png)

Con esto habremos utilizado el tipo de almacenamiento llamado Tabla.

