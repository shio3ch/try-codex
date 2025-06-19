FROM node:20
WORKDIR /app
COPY package.json tsconfig.json ./
COPY prisma ./prisma
RUN corepack enable && pnpm install && pnpm run prisma:generate
COPY src ./src
EXPOSE 3001
CMD ["pnpm", "run", "start:dev"]
