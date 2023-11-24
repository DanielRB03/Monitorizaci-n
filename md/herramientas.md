## Herramientas propias del sistema.
### PROCESOS

* <b>ps:</b> Muestra información de los procesos activos.
    - ps -aux → para ver los procesos
    - pkill -9 -u “usuario” → elimina los procesos de usuario
    - pkill -9 “proceso” → elimina el proceso
* <b>top:</b> Proporciona una visión en tiempo real de los procesos que consumen más recursos,
como la CPU y la memoria.
* <b>htop:</b> Similar a top, pero con una interfaz más visual y funciones adicionales, como la
capacidad de desplazarse y filtrar procesos de manera más intuitiva.
* <b>atop:</b> Registra e informa de la actividad de todos los procesos del servidor.

|Comando    |Función    |
|----------------|--------------|
|g  |Da información genérica|
|d  |Da información del disco|
|c  |Da información de la CPU|
|m  |Da información de la memoria|
|n  |Da información de la red|
|v  |Muestra las características de varios procesos|
|e  |Da información de la GPU|

### MEMORIA, ESPACIO Y RENDIMIENTO DEL DISCO

* <b>free:</b> Muestra la cantidad de memoria libre y utilizada en el sistema.
    - free -s 3 → da información de la memoria cada 3 segundos
    - free -c 3 → da info 3 veces
* <b>df:</b> Muestra el espacio utilizado y disponible en los sistemas de archivos montados.
    - df -h → muestra lo que está montado y su capacidad
    - df -hT → muestra además el sistema de archivos
* <b>du:</b> Muestra el espacio ocupado por un fichero o directorio.
    - du -h → Muestra el uso del espacio en formato legible para el usuario
* <b>iostat:</b> Se utiliza para rastrear los problemas de rendimiento de los dispositivos de
almacenamiento.

### TRÁFICO DE LA RED

* <b>tcpdump:</b> Analiza el tráfico que circula por la red.
    - tcpdump -i “interfaz” → para ver el tráfico de una tarjeta de red específica.
    - tcpdump -n → muestra las ips.
    - tcpdump net “red” → para ver el tráfico de esa red.
* <b>tcptrack:</b> Nos muestra las conexiones establecidas, su origen, destino, estado, el tiempo
de iddle y la velocidad de transferencia.
* <b>iptraf:</b> Intercepta paquetes en la red y muestra información sobre el tráfico.
* <b>bandwidthd:</b> una herramienta específica de monitorización del ancho de banda
