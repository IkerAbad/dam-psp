# FTP_Entrega_PSP

Entrega de la asignatura de PSP (Programación de Servicios y Procesos) del ciclo de DAM, abril de 2023. Cliente FTP en Java por consola, con un menú, hecho con Apache Commons Net.

## Qué hay

`MainMenu.java` se conecta a un servidor FTP, hace login y ofrece un menú para:

- listar los archivos y carpetas del directorio actual, diferenciando el tipo;
- cambiar de directorio;
- crear archivos y directorios;
- borrar directorios;
- renombrar;
- subir archivos o directorios;
- descargar archivos o directorios.

Compila con Java 17 y Maven. No lo he probado contra un servidor FTP, solo he comprobado que compila.

## Cómo probarlo

El servidor, el usuario y la clave se leen de las variables de entorno `FTP_HOST`, `FTP_USER` y `FTP_PASS`. Si no existen, usa `192.168.1.233` (un servidor de mi red local de entonces) y credenciales vacías.

```
mvn compile
mvn exec:java -Dexec.mainClass=org.jesuitasrioja.MainMenu
```

## Licencia

MIT, ver [LICENSE](LICENSE).

---

# FTP_Entrega_PSP (English)

Assignment for the PSP (Services and Processes Programming) subject of my DAM vocational course, April 2023. A console FTP client in Java with a menu, built with Apache Commons Net.

## What's inside

`MainMenu.java` connects to an FTP server, logs in and offers a menu to:

- list the files and folders in the current directory, telling their type apart;
- change directory;
- create files and directories;
- delete directories;
- rename;
- upload files or directories;
- download files or directories.

It builds with Java 17 and Maven. I have not tested it against an FTP server, I only checked that it compiles.

## Trying it

The server, user and password are read from the `FTP_HOST`, `FTP_USER` and `FTP_PASS` environment variables. If they are missing it uses `192.168.1.233` (a server on my local network back then) and empty credentials.

```
mvn compile
mvn exec:java -Dexec.mainClass=org.jesuitasrioja.MainMenu
```

## License

MIT, see [LICENSE](LICENSE).
