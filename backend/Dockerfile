FROM node:20
EXPOSE 8080
ENV DB_HOST=mysql 
RUN adduser expense 
RUN mkdir /opt/server
RUN chown -R expense:expense /opt/server
WORKDIR /opt/server
COPY  package.json .
COPY  *.js . 
RUN npm install 
CMD [ "node","index.js" ]


