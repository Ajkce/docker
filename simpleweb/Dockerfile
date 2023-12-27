FROM node:alpine

#Specify the directory inside the docker image on where to install and run this project
WORKDIR /app

#This will copy the package.json file first and install dependencies again only if the package.json is changed
COPY ./package.json ./



RUN npm install

#We copy all the other remainig files after node moduels are installed or used from previous build
COPY ./ ./

CMD ["npm", "start"]