# Use official Node LTS (adjust to node:18-alpine or node:20 if needed)
FROM node:18-alpine

# Set working directory inside the container
WORKDIR /app

# Copy package files separately to leverage Docker cache
COPY package*.json ./

# Install global Nest CLI (optional for development inside container)
RUN npm install -g @nestjs/cli

# Install dependencies
RUN npm install

# Copy the full project
COPY . .

# Build the NestJS app
RUN npm run build

# Expose the port NestJS app runs on (default: 3000)
EXPOSE 3000

# Start the app in production mode
CMD ["npm", "run", "start:prod"]
