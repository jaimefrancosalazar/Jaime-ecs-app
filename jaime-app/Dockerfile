FROM node:lts-alpine
ENV NODE_ENV=production
ENV PORT=80
WORKDIR /app
COPY . .
COPY ["package.json", "package-lock.json*", "npm-shrinkwrap.json*", "./"]
RUN npm install --silent 
EXPOSE 80
RUN chown -R node /usr/src/app
USER node
CMD ["npm", "start"]
