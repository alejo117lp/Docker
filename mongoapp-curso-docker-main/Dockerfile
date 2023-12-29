# Todas las imagenes se basan en otras, indicamos que se base en node y su versión
FROM node:20

# Crear carpeta para código fuente de la app, es una ruta dentro del mismo contenedor
RUN mkdir -p /home/app

#indicamos de donde va a sacar el código fuente de la app
#No usamos RUN sino COPY para que funcione en en windows
# ruta del sistema operativo anfitrion + destino
COPY . /home/app

#Exponer puerto para poderse conectar
EXPOSE 3000

#Comando a ejecutar para que la app corra
#Comando + argumentos + ruta completa
CMD ["node", "/home/app/index.js"]
