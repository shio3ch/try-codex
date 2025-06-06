FROM node:20
WORKDIR /app
COPY package.json tsconfig.json ./
COPY prisma ./prisma
RUN npm install && npm run prisma:generate
COPY src ./src
EXPOSE 3001
CMD ["npm", "run", "start:dev"]
