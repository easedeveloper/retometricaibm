FROM node:12

WORKDIR /usr/src/app

COPY . .

RUN npm install

EXPOSE 4000

HEALTHCHECK --interval=5s --timeout=2s CMD curl --fail http://localhost:4000/retoibm/sumar/3/4 || exit 1 

CMD [ "npm" , "start" ]

