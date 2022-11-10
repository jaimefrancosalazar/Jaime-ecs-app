FROM node:lts-alpine
ENV NODE_ENV=production
ENV PORT=3000
WORKDIR /app
COPY . .
COPY ["package.json", "package-lock.json*", "npm-shrinkwrap.json*", "./"]
RUN npm install --silent 
EXPOSE 3000
USER node
CMD ["npm", "start"]
#end
