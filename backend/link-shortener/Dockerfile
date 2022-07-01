FROM node:16


COPY package*.json /app/package.json
COPY tsconfig.json /app/tsconfig.json
COPY src /app/src
COPY . /app
WORKDIR /app

RUN ["npm","install","global","@nestjs/cli"]
RUN ["npm", "install", "redis@4.1.0" ]
RUN ["npm", "install"]

EXPOSE 3000

CMD ["npm", "run", "start:dev"]
