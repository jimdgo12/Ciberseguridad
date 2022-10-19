# **Jhon the ripper**

Esta es una herramienta muy utilizada para desarrollar auditorias, recuperación y cracking de contraseñas, esta es una herramienta de alto desempeño, cabe mencionar que es muy flexible, en otras palabras, esta herramienta permite configurar el parámetro de las letras, símbolos o números con los que se desea intentar descifrar una contraseña. Sin embargo, esta herramienta también es muy utilizada por diferentes paginas web a la hora de verificar la seguridad de las claves que proporcionan los usuarios, donde les muestra el nivel de seguridad de sus claves, si la clave es muy débil o débil les sugiere a los usuarios   que la contraseña debe contener mayúsculas, minúsculas símbolos o número para hacer que esta se vuelva más segura.

Además, esta herramienta es muy utilizada por los analistas de sistemas, donde esta permite determinar la robustez de una contraseña frente a ataques de fuerza bruta, funciona en las diferentes arquitecturas y sistemas operativos.


|     26    |     `sudo apt install John`    |     Este comando sirve para instalar la herramienta   John the Ripper en el wsl de Kali Linux    |
|---|---|---|
|     27    |     `ls /usr/share/john/`    |     Este comando sirve para listar los archivos que   están dentro de la ruta.    |
|     28    |     `cat   /usr/share/john/password.lst`    |     Este comando sirve para ver el contenido de un   archivo existente, que en este caso es password.lst    |
|     29    |     `sudo useradd -m test`    |     Este comando sirve para crear un usuario llamado   test en el directorio home, ya que se cuenta con los permisos de super usuario   otorgados por el comando sudo.    |
|     30    |     `sudo passwd test`    |     Este comando sirve para crear o cambiar   contraseñas de los usuarios mediante el hashing para cifrar la nueva   contraseña.    |
|     31    |     `sudo tail /etc/shadow`    |     Este comando sirve para mostrar los 10 últimos números   o colas del archivo shadow    |
|     32    |     `sudo john --wordlist=/usr/share/john/password.lst   /etc/shadow`    |     Este comando sirve para descifrar las contraseñas   ingresadas por el usuario, mediante la comparación del hash con un   diccionario de contraseñas, que en este caso es el password.list. mostrando   también el tiempo de crackeo.     |
|     33    |     `sudo passwd test`    |     Este comando sirve para crear o cambiar contraseñas de los usuarios   mediante el hashing para cifrar la nueva contraseña.    |
|     34    |     `sudo john /etc/shadow`    |     Este comando sirve para llevar a cabo un ataque de   fuerza bruta y lograr crackear una contraseña.    |

