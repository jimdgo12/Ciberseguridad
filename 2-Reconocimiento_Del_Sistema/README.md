# Reconocimiento Del Sistema

|     NUM    |     COMANDO                                                                 |     DESCRIPCION                                                                                                                             |
|------------|-----------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------|
|     1      |     `uname -a`                                                          |     Sirve para   obtener la información completa del sistema incluyendo versión del Kernel y   distribución Linux en un solo parámetro.     |
|     2      |     `cat  /proc/sys/kernel/hostname`                                    |     Con el siguiente comando se puede obtener el nombre   del host de la máquina.                                                           |
|     3      |     `echo  ”$USER"`                                                     |     El   comando echo sirve para imprimir en pantalla una cadena de texto echo “hello   world”.                                             |
|     4      |     `pwd`                                                               |     El   comando pwd sirve para ver en que parte del sistema estas ubicado, es decir,   que muestra la ruta de donde estas.                 |
|     5      |     `ifconfig wifi0`                                                    |     Este   comando sirve para ver en consola la información de las especificaciones de   la red.                                            |
|     6      |     `ip route \| grep default`                                     |     Este   comando sirve para para ver la dirección IP del router a la cual el pc está   conectado.                                         |
|     7      |     `curl ifconfig.me`                                                 |     Este   comando sirve para ver la IP publica con la que el computador está conectado   a internet.                                       |
|     8      |     `ping -ac  10 8.8.8.8`                                              |     Este   comando sirve saber el tiempo que toma enviar y recibir respuestas de una red.                                                   |
|     9      |     `ping -c  10 1.1.1.1`                                               |     Este   comando sirve para verificar si hay rutas alcanzables entre el origen y el   destino.                                            |
|     10     |     `route -n`                                                          |     Este   comando sirve para mostrar la tabla de enrutamiento en forma numérica   completa.                                                |
|     11     |     `route.exe  print`                                                  |     Este   comando sirve para imprimir en consola la tabla de enrutamiento.                                                                 |
|     12     |     `tracert.exe  8.8.8.8`                                              |     Este   comando sirve para trazar la ruta de un paquete entrante que viene desde el   host o punto de red hasta el ordenador.            |
|     13     |     `arp.exe -a`                                                       |     Este   comando sirve para mostrar las tablas de las diferentes direcciones IP que se   han almacenado.                                  |
|     14     |     `netstat.exe  -nt`                                                  |     Este comando   sirve para mostrar en consola las conexiones de red.                                                                     |
|     15     |     `netstat.exe  -nat \| grep -c 'ESTABLISHED'`                    |     Este comando   sirve para contar las direcciones IP establecidas.                                                                       |
|     16     |     `netstat.exe -nao \| grep 'LISTEN' > cat > ports_up.txt`    |     Este comando   sirve para guardar dentro de un archivo todo lo que contenga la palabra seleccionada.                                    |
|     17     |     `cat ports_up.txt`                                                  |     Este comando sirve para mostrar el   contenido de un archivo en la terminal o consola.                                                  |


**a.** El comando 6 de la lista anterior ejecuta una tubería compuesta por dos comandos del sistema operativo 
Linux en WSL lo que es el comportamiento esperado y también funcionaria en una máquina virtual huésped 
o en un anfitrión con Linux; el comando 12 es un comando del sistema operativo Windows que no se puede 
ejecutar en sistemas Linux, pero si se puede ejecutar en WSL, Explique

**R/.** Tracert.exe 8.8.8.8 este comando no funciona en Linux, porque la extensión .exe es netamente de Windows, es por esto que no funciona en Linux.

**b.** La línea 15 describe una tubería que ejecuta un comando Windows y lo canaliza a la entrada de un comando 
que no existe en Windows, explique. 

**R/.** Con el wsl se puede acceder al comando de Windows como también a los de Linux, ya que estos se conectan gracias a la unión del kernel de Linux

**c.** La línea 16 y 17 describen la situación anterior pero adicionalmente accede al sistema de archivos de 
Windows para crear un archivo, explique. 

**R/.**	En los comandos 16, 17 permite ejecutar los comandos de Linux gracias a su kernel, porque al estar instalado en Windows por medio del wsl este puede acceder, crear, visualizar etc. los archivos del sistema operativo Windows.


## **Mas Información**

* [Uso del comando netstat en Linux][1_0]

[1_0]:https://geekflare.com/es/netstat/
