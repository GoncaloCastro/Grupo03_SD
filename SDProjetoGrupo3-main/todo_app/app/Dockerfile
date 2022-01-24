FROM node:12-alpine
RUN apk add --no-cache python2 g++ make
WORKDIR /app
COPY . .
RUN yarn config set "strict-ssl" false -g
RUN yarn install --production
CMD ["node", "src/index.js"]
