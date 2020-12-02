FROM node:lts-alpine
#ATTENTION!!!!!! INSTALLER GIT! car il y a certaine dependances sur git (Résolution not found /app/node_modules)
RUN apk add git
WORKDIR /app
COPY package.json* ./
RUN npm install
COPY . .


EXPOSE 8080

CMD ["npm", "run", "serve"]