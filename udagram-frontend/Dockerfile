FROM node:13

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 8083

RUN npm install -g @ionic/cli

RUN ionic build

CMD ["ionic","serve"]
