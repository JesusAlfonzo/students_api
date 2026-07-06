# 1. Esta línea es la que instala Node y npm mágicamente
FROM node:20-alpine

WORKDIR /app

COPY package.json package-lock.json* ./
RUN npm install

COPY . .

EXPOSE 5173

# 2. Aquí ejecuta npm, pero ya existe gracias a la primera línea
CMD ["npm", "run", "dev", "--", "--host"]