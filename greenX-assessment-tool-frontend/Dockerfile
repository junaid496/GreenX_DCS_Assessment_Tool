FROM node:18-alpine

WORKDIR /app

# Copy dependency files first for caching
COPY package*.json ./

RUN npm install --legacy-peer-deps

# Copy rest of the app
COPY . .

EXPOSE 3000

# Start React app
CMD ["npm", "start"]

