#Version: 2
FROM node:22.8.0-alpine3.20
RUN addgroup nodeapp && adduser -S -G nodeapp nodeapp
USER nodeapp
WORKDIR /app/
COPY --chown=nodeapp package*.json .
RUN npm install
COPY --chown=nodeapp . .
EXPOSE 3000
CMD ["npm", "start"]