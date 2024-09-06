PRACTICA Contenedores: más que VMs DOCKER

#Version 2
* Imagenes: node:22.8.0-alpine3.20, mongo:5.0.28-focal
* Plantilla: Vite + React {de Nicolas S.}
* Capas: Backend: app[p:5173, usr: nodeapp], Frontend: api[p:3000, usr: react], Base de datos: db[p:27017]
* Volumes: ./backend/app:/app/app, ./frontend/src:/app/src, gamify:/data/db
* Enviroment: VITE_API_URL: http://localhost:3000


#Prueba
* Instalar Docker.
* Descargar archivos de GIT en dirtectorio de prueba.
* Desde el directorio de prueba, en la consola de comandos ejecutar el comando: docker compose up
* Abrir navegador y ejecutar: localhost
* Para detener la ejecucion, en la consola de comandos teclear CTL+C
* Revision de logs, en la consola de comandos ejectuando el comando: docker compose logs
