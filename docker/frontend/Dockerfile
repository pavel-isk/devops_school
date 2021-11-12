FROM node:13
WORKDIR /usr/src/app
COPY package*.json ./
COPY src ./src
COPY public ./public
RUN npm install
RUN npm install -g serve
RUN npm run build
CMD ["serve","-s","build"]
