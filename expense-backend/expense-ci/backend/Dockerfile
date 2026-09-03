FROM node:20-alpine3.21
RUN addgroup -S expense && adduser -S expense -G expense
WORKDIR /opt/server
COPY DbConfig.js .
COPY index.js .
COPY package.json .
COPY TransactionService.js .
RUN npm install .
RUN chown -R expense:expense /opt/server
ENV DB_HOST="mysql"
USER expense
CMD ["node","index.js"]
