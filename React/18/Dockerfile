# Use official Node.js LTS version (can adjust based on your preference)
FROM node:18-alpine

# Set working directory inside container
WORKDIR /app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the app
COPY . .

# Build the app for production
RUN npm run build

# Expose the port React runs on
EXPOSE 3000

# Start the React app
CMD ["npm", "start"]
