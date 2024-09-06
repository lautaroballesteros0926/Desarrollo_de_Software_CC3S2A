# Usa la imagen oficial de Node.js como imagen base
FROM node:14

# Establece el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copia los archivos package.json y package-lock.json
COPY package*.json ./

# Instala las dependencias de la aplicación
RUN npm install

# Copia el resto de los archivos de la aplicación
COPY . .

# Expone el puerto 3000 para la aplicación
EXPOSE 3000

# Comando para iniciar la aplicación
CMD ["node", "src/app.js"]