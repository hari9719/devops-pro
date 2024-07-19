FROM node:14

WORKDIR /app

COPY index.js /app/index.js 
COPY package.json /app/package.json 
COPY views/index.ejs /app/views/index.ejs
COPY models/sequelize/user.model.js /app/models/sequelize/user.model.js
COPY db/sequelize.js /app/db/sequelize
RUN npm install
ENV MYSQL_USERNAME=admin
ENV MYSQL_ROOT_PASSWORD=hariharan7
ENV MYSQL_DATABASE=clab
ENV MYSQL_HOST=database-1.czwgmomcga5y.ap-southeast-1.rds.amazonaws.com
ENV MYSQL_LOCAL_PORT=3306
ENV MYSQL_DOCKER_PORT=3306
ENV NODEJS_LOCAL_PORT=3000
ENV NODEJS_DOCKER_PORT=3000
EXPOSE 3000

CMD [ "npm", "start" ]
