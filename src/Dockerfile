FROM node:18-slim

WORKDIR  /mutating-webhook

COPY . /mutating-webhook

RUN npm install -g typescript
RUN npm install
RUN tsc --build

EXPOSE 1337
CMD [ "node", "server" ]