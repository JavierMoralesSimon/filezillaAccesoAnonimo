# Configuración de acceso anónimo en FileZilla

## Creación del usuario anónimo
En el protocolo FTP, el acceso anónimo se logra creando un usuario con el nombre específico "anonymous". Los pasos son:
  * Abrir FileZilla Server Administration.
  * Ir a la sección "Server - Configure - Users".
  * Damos a "Add" para crear un usuario.
  * Le damos de nombre "anonymous".
  * Ponemos que no se requiera de autenticación.
  * Limitamos el directorio accesible diciendole al servidor a qué carpeta física del sistema debe de entrar el usuario.Esto se hace en la sección "Mount points" dando a "Add" y poniendo "/" en la columna "Virtual Path" lo cual indica que cuando el usuario entre, verá esa carpeta como su raíz, y poniendo la ruta completa de la carpeta en la columna "Native Path".
  * Por último, establecemos permisos solo de lectura en "Mount options -  Access mode" y desmarcamos todo lo demás.
![](https://github.com/JavierMoralesSimon/filezillaAccesoAnonimo/blob/main/Capturas/1.png)

## Conexión como usuario anónimo desde un cliente
* Abrir FileZilla Client.
* En la barra de arriba:
 * En servidor escribimos la IP de nuestra máquina.
 * En el nombre de usuario escribimos "anonymous".
 * Contraseña lo dejamos vacío.
 * En puerto ponemos el 21.
 * Hacemos clic en "Conexión rápida".
![](https://github.com/JavierMoralesSimon/filezillaAccesoAnonimo/blob/main/Capturas/2.1.png)
* Nos salta un aviso en el cual marcamos el checkbox de abajo y aceptamos.
![](https://github.com/JavierMoralesSimon/filezillaAccesoAnonimo/blob/main/Capturas/2.2.png)
* Finalmente, hemos creado la conexión.
![](https://github.com/JavierMoralesSimon/filezillaAccesoAnonimo/blob/main/Capturas/2.3.png)
