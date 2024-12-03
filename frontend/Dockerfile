# Base image
FROM node:16-alpine

# Set working directory
WORKDIR /app

# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install

# Copy application source code
COPY . .

# Build application
RUN npm run build

# Expose port 3000
EXPOSE 3000

# Start application
CMD ["npm", "start"]
