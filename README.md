# Examen-tercer-trimestre-Examen
---
INTRODUCCION
Docker es un sistema operativo para contenedores. Parecido a una máquina virtual virtualiza el hardware del servidor,por ello los contenedores virtualizan el sistema operativo de un servidor.

- Configurar el archivo docker-compose.yml

Un archivo docker compose es basicamente un archivo con extension .yml por tanto primero debemos crearlo y editar su contenido. con el comando:
touch docker-compose.yml

Al haber puesto este comando nos aparecera algo parecido a lo siguiente que es lo que deberemos modificar:

![image](https://user-images.githubusercontent.com/72273897/172452461-8d2bc5bc-82aa-4cf1-9a2c-0e32a03e19a8.png)

Esto es lo que deberiamos modificar segun lo que queramos hacer .

- Pasos para el despliegue de la aplicación.
Para realizar el despliegue de una aplicacione en Docker debemos seguir los pasos siguientes:
1. En la consola de comandos creamos un fichero llamado ‘docker-compose.yml’ el cual modificaremos como en el anterior parte.

2. una vez dentro de este modificamos los datos para el contenedor de ‘WordPress‘ y el de la base de datos ‘MariaDB‘;
3. Con el comando docker-compose up -d crearemos nuestro contenedor.
4. Al terminar este processo , utilizaremos el comando docker ps -a para comprobar que todo va bien.

- Preparación y subida de la imagen a dockerhub.
Para preparar y subir una imagen se realizaria de la siguiente manera:

1. Utilizamos docker loguin para iniciarlo.
- ![image](https://user-images.githubusercontent.com/72273897/172455140-f453b5c1-988e-4c2b-a0e7-fb5e4cb4375d.png)
2. Una vez iniciada la sesion en docker procedemos a utilizar :
nombre_de_usuario/nombre_del_repositorio:etiqueta.
 
3. Para preparar la imagen para que tenga el formato correcto y sea aceptada dentro de este registro.
para ello utilizamos el comando docker tag.

4. Ya tenemos nuestra imagen que cumple con el formato y podemos subirla al repositorio , para subirlo usaremos el comando:
docker push nombre_del_repositorio/ubuntu-git:1.0.
Deberia aparecer algo asi:
![image](https://user-images.githubusercontent.com/72273897/172455931-8e0e04c9-4a0e-47c1-9c0b-41e04e5afb6c.png)

5.Una vez terminado este paso, podremos comprobar en hub.docker.com que nuestra imagen ha sido publicada.

- Annexos.
Despues de perder el tiempo en intentar hacer funcionar las maquinas virtuales que nunguna de ellas me han funcionado y al solo tener una hora mas, he decidido hacerlo utilizando capturas que ya habia hecho entre otras herramientas. E intentar explicarlo lo mejor posible con lo que se.
- ![image](https://user-images.githubusercontent.com/72273897/172453055-206076a2-044a-486f-ae47-7b00cdad3aa7.png)

