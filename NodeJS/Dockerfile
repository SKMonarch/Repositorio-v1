# Usamos una imagen base de Node.js
FROM node:18.18.0

# Establecemos el directorio de trabajo en el contenedor
WORKDIR /app

# Copiamos el archivo package.json y package-lock.json al directorio de trabajo
COPY package*.json ./

# Instalamos las dependencias del proyecto
RUN npm install

# Copiamos el resto de los archivos de la aplicación al directorio de trabajo
COPY . .

# Exponemos el puerto en el que la aplicación va a escuchar (ajústalo según tus necesidades)
EXPOSE 3000

# Comando para iniciar la aplicación cuando se ejecute el contenedor
CMD ["node", "app.js"]

