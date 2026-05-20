## Que es Docker?
Es un programa de terceros o no nativa (no viene instalado de fabrica) que instalamos en el user space o nuestra maquina original como lo puede ser Java o mi editor de codigo. Es un programa de infraestructura, ya que ayuda en estandarizar y preparar un entorno para ejecutar algo, no?

Cuando se intala, se descargan dos componentes: 
El motor de Docker(Docker engine o Daemon): Es el nucleo real del programa. Se ejecuta en la memoria RAM y se comunica constantemente con el Kernel. 
CLiente Docker(Docker CLI): La linea de comando con la interactuo con el motor de Docker, no? 

>El Docker Desktop es el programa o aplicacion de escritorio con interfaz grafica y botons, es solo la capa vistual para no usar la terminal

### para que sirve Docker?
Sirve para que haya consistencia en la preparacion y ejecucion de cualquier proyecto.

### como sucede? 
Docker empaqueta todo lo necesario para ejecutar nuestro programa, como: dependencias, herramientas, sus versiones, etc. 
A este paquete se le llama Ïmagen(Docker Image).
Es un archivo o conjunto d archivos que contiene todo para que funcione algo, excepto el kernel del OS. Contiene los archivos binarios reales ya instalados.
Las instrucciones estan en una archivo aparte.

Es Read-only, o de solo lectura. 
Una imagen es estrictamente inmutable. Nadie puede modificar la imagen cuando Docker la termina de compilar (no se que es eso, pense qu java era el unico que hacia eso)
Si se edita esta imagen, seria una totalmente diferente con esos nuevos cambios (parecido a lo que pasa con git y el codigo hash de cualquier commit sin importar que solo se cambio un punto y coma)