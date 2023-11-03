# Usa una imagen de Node.js como imagen base
FROM node:14

# Establece el directorio de trabajo
WORKDIR /TheRealDevOps/client

# Copia los archivos de la aplicación React.js a la imagen
COPY ./ ./

# Instala las dependencias
RUN npm install

# Compila la aplicación React.js
RUN npm run build

# Expose the port donde se ejecutará la aplicación React.js (por defecto 80)
EXPOSE 7003

# Inicia un servidor web para servir la aplicación React.js
CMD ["npx", "serve", "-s", "-l", "7003", "build"]
