FROM node:10-alpine
COPY ./* ./
RUN npm install
COPY --chown=node:node . .
USER node
EXPOSE 8080
CMD ["node","index.js"]
