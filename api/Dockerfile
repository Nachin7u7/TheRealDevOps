# Usa una imagen de Node.js como imagen base
FROM node:14

# Establece el directorio de trabajo
WORKDIR /app/api

# Copia los archivos de la API a la imagen
COPY ./ ./

# Instala las dependencias
RUN npm install

# Expone el puerto en el que se ejecutará la API
EXPOSE 27017

# Inicia la API
CMD ["npm", "start"]
