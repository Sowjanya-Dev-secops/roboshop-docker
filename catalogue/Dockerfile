FROM node:20.19.6-alpine3.21 AS build
WORKDIR /opt/server
#current directory
COPY package.json . 
COPY *.js .
RUN npm install
ENV MONGO="true"\
    MONGO_URL="mongodb://mongodb:27017/catalogue"
CMD ["node","server.js"]


# FROM node:20
# WORKDIR /opt/server
# #current directory
# COPY package.json . 
# COPY *.js .
# RUN npm install
# ENV MONGO="true"\
#     MONGO_URL="mongodb://mongodb:27017/catalogue"
# CMD ["node","server.js"]